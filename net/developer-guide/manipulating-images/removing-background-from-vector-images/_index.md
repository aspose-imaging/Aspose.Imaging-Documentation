---
title: Remove background from vector images in C#
linktitle: Remove background from vector images
type: docs
weight: 15
url: /net/removing-background-from-vector-images/
description: Setting some of the pixel values in an image to zero, or some other “background” value is known as Masking. C# Image Processing Library supports the following types of masking.
keywords: remove background from vector images, remove background from EMF, remove background from SVG, remove background from WMF, remove background from CDR
---

<style>
   .frame {
    border: 2px solid darkgray;
    padding: 5px;
    margin: 10px 0 5px 5px;
    background: #f0f0f0;
    align-items: center;
   }
   .container {
    display: flex;
    flex-direction: row;
    align-items: center;
    justify-content: space-around;
   }
    .frame figcaption {
    margin: 0 auto;
    display: flex;
    flex-direction: row;
    justify-content: center;
   }
</style>

<figure class="frame">
<div class="container">
    <div>
        <figcaption>Original image</figcaption>
    </div>
    <div>
        <figcaption>Resulting image</figcaption>
    </div>
</div>
<div class="container">
    <div>
        <img src="./test-with-background.odg.webp" alt="Vector ODG image with background" width="640" height="905"/>
    </div>
    <div>
        <img src="./test-removed-background.odg.webp" alt="Removed background from ODG vector image" width="640" height="905"/>
    </div>
</div>
<figcaption>Removing background from vector image</figcaption>
</figure>

C# code example:

```cs
var fileNames = new string[] { "golfer.emf", "doretree.emf","Test2.wmf", "test.odg",
                                "test.cdr","test.cmx", "hatch.odg", "Halle_2.svg"};
var rbs = new RemoveBackgroundSettings[]
{
    new RemoveBackgroundSettings()
    {
        DetectionLevel = 30
    },
    new RemoveBackgroundSettings()
    {
        Bounds = new RectangleF(0, 1000, 5000, 4000)
    },
    new RemoveBackgroundSettings()
    {
        DetectionLevel = 10
    },
    new RemoveBackgroundSettings()
    {

    },
    new RemoveBackgroundSettings()
    {

    },
    new RemoveBackgroundSettings()
    {

    },
    new RemoveBackgroundSettings()
    {
        Color1 = Color.Blue
    },
    new RemoveBackgroundSettings()
    {

    }
};

for (int i = 0; i < fileNames.Length; i++)
{
    RemoveBackgroundExample(fileNames[i], rbs[i]);
}

private void RemoveBackgroundExample(string fileName, RemoveBackgroundSettings settings)
{
    var baseFolder = "D:\\test\\rb\\";
    var inputFilePath = Path.Combine(baseFolder, fileName);
    var outFilePath = Path.Combine(baseFolder, "output");
    if (!Directory.Exists(outFilePath))
    {
        Directory.CreateDirectory(outFilePath);
    }

    using (var image = Image.Load(inputFilePath))
    {
        var options = new PngOptions()
        {
            ColorType = PngColorType.TruecolorWithAlpha,
            VectorRasterizationOptions = new VectorRasterizationOptions()
            {
                BackgroundColor = Color.Transparent,
                PageSize = image.Size
            }
        };

        var vectorImage = image as VectorImage;
        if (vectorImage != null)
        {
            vectorImage.RemoveBackground(settings);
        }

        image.Save(Path.Combine(outFilePath, fileName+".png"), options);
    }
}
```
