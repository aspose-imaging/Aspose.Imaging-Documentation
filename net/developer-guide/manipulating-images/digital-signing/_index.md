---
title: Digital signing image
type: docs
weight: 50
url: /net/developer-guide/manipulating-images/digital-signature/
description: A tool that uses the LSB (Least Significant Bit) steganography algorithm embeds a digital signature directly into image pixel data. C# code example provided.
---

## Digital image signature

A digital signature (binary data) is generated from the user provided password.
The signature bits are inserted into the least significant bits of image pixels.
Because only the smallest bit of each color component is changed, visual quality remains almost identical.

The embedded signature can later be  verified to confirm image authenticity.

### API Methods

- [EmbedDigitalSignature](https://reference.aspose.com/imaging/net/aspose.imaging/rasterimage/embeddigitalsignature/)  method from the Aspose.Imaging library. **Embed LSB data** based on provided password into image pixel data. 
  
  The LSB steganography algorithm requires the image to be at least 8 pixels in width and height, with a minimum of 16,384 total pixels. 
  
  Password must be at least 4 characters long.
  
  The image can be saved in any supported format while preserving near-identical visual appearance, with modifications remaining imperceptible to the human eye.
- Check image signing by:
  - [IsDigitalSigned](https://reference.aspose.com/imaging/net/aspose.imaging/rasterimage/isdigitalsigned/). You can **quickly verify** whether an image is digitally signed using the provided password.
      
    The method performs partial data extraction and stops early once the specified threshold is reached (75% probability
    by default). Verification succeeds only when the original password is provided. This approach prevents unauthorized users from determining whether a digital signature exists, thereby protecting the security of the password owner.
  - [AnalyzePercentageDigitalSignature](https://reference.aspose.com/imaging/net/aspose.imaging/rasterimage/analyzepercentagedigitalsignature/).**Precise image check digital signing**. 
    
    Performs full data extraction and returns the probability (0–100%) that the image was signed using the specified password.
    
    This method is useful in scenarios where the image may have undergone minor modifications, allowing evaluation of partial signature consistency rather than a strict binary result.


{{< gist "aspose-com-gists" "517701807ffb1fd41f0c42ba95e5ad16" "AnalyzePercentageDigitalSignature.cs" >}}
