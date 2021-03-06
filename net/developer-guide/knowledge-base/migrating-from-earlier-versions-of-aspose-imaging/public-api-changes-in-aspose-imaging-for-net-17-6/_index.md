---
title: Public API Changes in Aspose.Imaging  for .NET 17.6
type: docs
weight: 50
url: /net/public-api-changes-in-aspose-imaging-for-net-17-6/
---

{{% alert color="primary" %}} 

This document describes changes to the Aspose.Imaging API in version 17.6, that may be of interest to module/application developers. It includes not only new and updated public methods, but also a description of any changes in the behavior behind the scenes in Aspose.Imaging.

{{% /alert %}} 
## **Added APIs:**
Class Aspose.Imaging.FileFormats.Jpeg.JpegLsInterleaveMode
Class Aspose.Imaging.FileFormats.Jpeg.JpegLsPresetCodingParameters
Class Aspose.Imaging.FileFormats.Jpeg.SampleRoundingMode
Class Aspose.Imaging.FileFormats.Psd.Layers.LayerResources.Lfx2Resource
Class Aspose.Imaging.FileFormats.Psd.Resources.CaptionDigestResource
Class Aspose.Imaging.FileFormats.Psd.Resources.ColorHalftoneInformationResource
Class Aspose.Imaging.FileFormats.Psd.Resources.ColorTransferFunctionsResource
Class Aspose.Imaging.FileFormats.Psd.Resources.DocumentSpecificIdsResource
Class Aspose.Imaging.FileFormats.Psd.Resources.GlobalAltitudeResource
Class Aspose.Imaging.FileFormats.Psd.Resources.GlobalAngleResource
Class Aspose.Imaging.FileFormats.Psd.Resources.IccUntaggedResource
Class Aspose.Imaging.FileFormats.Psd.Resources.LayerGroupInformationResource
Class Aspose.Imaging.FileFormats.Psd.Resources.LayerGroupsEnabledResource
Class Aspose.Imaging.FileFormats.Psd.Resources.LayerSelectionIdsResource
Class Aspose.Imaging.FileFormats.Psd.Resources.LayerStateInformationResource
Class Aspose.Imaging.FileFormats.Psd.Resources.PixelAspectRatioResource
Class Aspose.Imaging.FileFormats.Psd.Resources.PrintFlagsResource
Class Aspose.Imaging.FileFormats.Psd.Resources.PrintScaleResource
Class Aspose.Imaging.FileFormats.Psd.Resources.QuickMaskInformationResource
Class Aspose.Imaging.FileFormats.Psd.Resources.UnicodeAlphaNamesResource
Class Aspose.Imaging.FileFormats.Psd.Resources.UrlListResource
Class Aspose.Imaging.FileFormats.Psd.Resources.VersionInfoResource
Class Aspose.Imaging.FileFormats.Psd.Resources.WatermarkResource
Class Aspose.Imaging.ImageLoadOptions.PsdLoadOptions
Field/Enum Aspose.Imaging.FileFormats.Jpeg.JpegCompressionMode.JpegLs
Field/Enum Aspose.Imaging.FileFormats.Jpeg.JpegLsInterleaveMode.Line
Field/Enum Aspose.Imaging.FileFormats.Jpeg.JpegLsInterleaveMode.None
Field/Enum Aspose.Imaging.FileFormats.Jpeg.JpegLsInterleaveMode.Sample
Field/Enum Aspose.Imaging.FileFormats.Jpeg.SampleRoundingMode.Extrapolate
Field/Enum Aspose.Imaging.FileFormats.Jpeg.SampleRoundingMode.Truncate
Field/Enum Aspose.Imaging.FileFormats.Psd.Layers.LayerMaskFlags.UserMaskFromRenderingOtherData
Field/Enum Aspose.Imaging.FileFormats.Psd.Layers.LayerResources.Lfx2Resource.TypeToolKey
Method Aspose.Imaging.FileFormats.Dicom.DicomImage.#ctor(System.IO.Stream,Aspose.Imaging.LoadOptions)
Method Aspose.Imaging.FileFormats.Jpeg.JpegLsPresetCodingParameters.#ctor
Method Aspose.Imaging.FileFormats.Psd.Layers.LayerResources.Lfx2Resource.#ctor
Method Aspose.Imaging.FileFormats.Psd.Layers.LayerResources.Lfx2Resource.Save(Aspose.Imaging.StreamContainer,System.Int32)
Method Aspose.Imaging.FileFormats.Psd.Resources.CaptionDigestResource.#ctor
Method Aspose.Imaging.FileFormats.Psd.Resources.ColorHalftoneInformationResource.#ctor
Method Aspose.Imaging.FileFormats.Psd.Resources.ColorTransferFunctionsResource.#ctor
Method Aspose.Imaging.FileFormats.Psd.Resources.DocumentSpecificIdsResource.#ctor
Method Aspose.Imaging.FileFormats.Psd.Resources.GlobalAltitudeResource.#ctor
Method Aspose.Imaging.FileFormats.Psd.Resources.GlobalAngleResource.#ctor
Method Aspose.Imaging.FileFormats.Psd.Resources.IccUntaggedResource.#ctor
Method Aspose.Imaging.FileFormats.Psd.Resources.LayerGroupInformationResource.#ctor
Method Aspose.Imaging.FileFormats.Psd.Resources.LayerGroupsEnabledResource.#ctor
Method Aspose.Imaging.FileFormats.Psd.Resources.LayerSelectionIdsResource.#ctor
Method Aspose.Imaging.FileFormats.Psd.Resources.LayerStateInformationResource.#ctor
Method Aspose.Imaging.FileFormats.Psd.Resources.PixelAspectRatioResource.#ctor
Method Aspose.Imaging.FileFormats.Psd.Resources.PrintFlagsResource.#ctor
Method Aspose.Imaging.FileFormats.Psd.Resources.PrintScaleResource.#ctor
Method Aspose.Imaging.FileFormats.Psd.Resources.QuickMaskInformationResource.#ctor
Method Aspose.Imaging.FileFormats.Psd.Resources.UnicodeAlphaNamesResource.#ctor
Method Aspose.Imaging.FileFormats.Psd.Resources.UrlListResource.#ctor
Method Aspose.Imaging.FileFormats.Psd.Resources.VersionInfoResource.#ctor
Method Aspose.Imaging.FileFormats.Psd.Resources.WatermarkResource.#ctor
Method Aspose.Imaging.ImageLoadOptions.PsdLoadOptions.#ctor
Property Aspose.Imaging.FileFormats.Jpeg.JpegLsPresetCodingParameters.MaximumSampleValue
Property Aspose.Imaging.FileFormats.Jpeg.JpegLsPresetCodingParameters.ResetValue
Property Aspose.Imaging.FileFormats.Jpeg.JpegLsPresetCodingParameters.Threshold1
Property Aspose.Imaging.FileFormats.Jpeg.JpegLsPresetCodingParameters.Threshold2
Property Aspose.Imaging.FileFormats.Jpeg.JpegLsPresetCodingParameters.Threshold3
Property Aspose.Imaging.FileFormats.Psd.Layers.LayerMaskData.ImageDataVector
Property Aspose.Imaging.FileFormats.Psd.Layers.LayerResources.Lfx2Resource.BlendMode
Property Aspose.Imaging.FileFormats.Psd.Layers.LayerResources.Lfx2Resource.Data
Property Aspose.Imaging.FileFormats.Psd.Layers.LayerResources.Lfx2Resource.EffectColor
Property Aspose.Imaging.FileFormats.Psd.Layers.LayerResources.Lfx2Resource.Key
Property Aspose.Imaging.FileFormats.Psd.Layers.LayerResources.Lfx2Resource.Length
Property Aspose.Imaging.FileFormats.Psd.Layers.LayerResources.Lfx2Resource.Opacity
Property Aspose.Imaging.FileFormats.Psd.Layers.LayerResources.Lfx2Resource.PsdVersion
Property Aspose.Imaging.FileFormats.Psd.Layers.LayerResources.Lfx2Resource.Signature
Property Aspose.Imaging.FileFormats.Psd.Resources.CaptionDigestResource.DataSize
Property Aspose.Imaging.FileFormats.Psd.Resources.CaptionDigestResource.Digest
Property Aspose.Imaging.FileFormats.Psd.Resources.CaptionDigestResource.MinimalVersion
Property Aspose.Imaging.FileFormats.Psd.Resources.ColorHalftoneInformationResource.DataSize
Property Aspose.Imaging.FileFormats.Psd.Resources.ColorHalftoneInformationResource.HalftoneData
Property Aspose.Imaging.FileFormats.Psd.Resources.ColorHalftoneInformationResource.MinimalVersion
Property Aspose.Imaging.FileFormats.Psd.Resources.ColorTransferFunctionsResource.ColorTransferData
Property Aspose.Imaging.FileFormats.Psd.Resources.ColorTransferFunctionsResource.DataSize
Property Aspose.Imaging.FileFormats.Psd.Resources.ColorTransferFunctionsResource.MinimalVersion
Property Aspose.Imaging.FileFormats.Psd.Resources.DocumentSpecificIdsResource.DataSize
Property Aspose.Imaging.FileFormats.Psd.Resources.DocumentSpecificIdsResource.Id
Property Aspose.Imaging.FileFormats.Psd.Resources.DocumentSpecificIdsResource.MinimalVersion
Property Aspose.Imaging.FileFormats.Psd.Resources.GlobalAltitudeResource.Altitude
Property Aspose.Imaging.FileFormats.Psd.Resources.GlobalAltitudeResource.DataSize
Property Aspose.Imaging.FileFormats.Psd.Resources.GlobalAltitudeResource.MinimalVersion
Property Aspose.Imaging.FileFormats.Psd.Resources.GlobalAngleResource.DataSize
Property Aspose.Imaging.FileFormats.Psd.Resources.GlobalAngleResource.GlobalAngle
Property Aspose.Imaging.FileFormats.Psd.Resources.GlobalAngleResource.MinimalVersion
Property Aspose.Imaging.FileFormats.Psd.Resources.IccUntaggedResource.DataSize
Property Aspose.Imaging.FileFormats.Psd.Resources.IccUntaggedResource.MinimalVersion
Property Aspose.Imaging.FileFormats.Psd.Resources.IccUntaggedResource.Profile
Property Aspose.Imaging.FileFormats.Psd.Resources.LayerGroupInformationResource.DataSize
Property Aspose.Imaging.FileFormats.Psd.Resources.LayerGroupInformationResource.Groups
Property Aspose.Imaging.FileFormats.Psd.Resources.LayerGroupInformationResource.MinimalVersion
Property Aspose.Imaging.FileFormats.Psd.Resources.LayerGroupsEnabledResource.DataSize
Property Aspose.Imaging.FileFormats.Psd.Resources.LayerGroupsEnabledResource.IDs
Property Aspose.Imaging.FileFormats.Psd.Resources.LayerGroupsEnabledResource.MinimalVersion
Property Aspose.Imaging.FileFormats.Psd.Resources.LayerSelectionIdsResource.Count
Property Aspose.Imaging.FileFormats.Psd.Resources.LayerSelectionIdsResource.DataSize
Property Aspose.Imaging.FileFormats.Psd.Resources.LayerSelectionIdsResource.LayerIds
Property Aspose.Imaging.FileFormats.Psd.Resources.LayerSelectionIdsResource.MinimalVersion
Property Aspose.Imaging.FileFormats.Psd.Resources.LayerStateInformationResource.DataSize
Property Aspose.Imaging.FileFormats.Psd.Resources.LayerStateInformationResource.LayerIndex
Property Aspose.Imaging.FileFormats.Psd.Resources.LayerStateInformationResource.MinimalVersion
Property Aspose.Imaging.FileFormats.Psd.Resources.PixelAspectRatioResource.AspectRatio
Property Aspose.Imaging.FileFormats.Psd.Resources.PixelAspectRatioResource.DataSize
Property Aspose.Imaging.FileFormats.Psd.Resources.PixelAspectRatioResource.MinimalVersion
Property Aspose.Imaging.FileFormats.Psd.Resources.PixelAspectRatioResource.Version
Property Aspose.Imaging.FileFormats.Psd.Resources.PrintFlagsResource.BleedScale
Property Aspose.Imaging.FileFormats.Psd.Resources.PrintFlagsResource.BleedWidth
Property Aspose.Imaging.FileFormats.Psd.Resources.PrintFlagsResource.CenterCropMark
Property Aspose.Imaging.FileFormats.Psd.Resources.PrintFlagsResource.DataSize
Property Aspose.Imaging.FileFormats.Psd.Resources.PrintFlagsResource.MinimalVersion
Property Aspose.Imaging.FileFormats.Psd.Resources.PrintFlagsResource.Version
Property Aspose.Imaging.FileFormats.Psd.Resources.PrintScaleResource.DataSize
Property Aspose.Imaging.FileFormats.Psd.Resources.PrintScaleResource.MinimalVersion
Property Aspose.Imaging.FileFormats.Psd.Resources.PrintScaleResource.Scale
Property Aspose.Imaging.FileFormats.Psd.Resources.PrintScaleResource.Style
Property Aspose.Imaging.FileFormats.Psd.Resources.PrintScaleResource.XLocation
Property Aspose.Imaging.FileFormats.Psd.Resources.PrintScaleResource.YLocation
Property Aspose.Imaging.FileFormats.Psd.Resources.QuickMaskInformationResource.ChannelId
Property Aspose.Imaging.FileFormats.Psd.Resources.QuickMaskInformationResource.DataSize
Property Aspose.Imaging.FileFormats.Psd.Resources.QuickMaskInformationResource.IsMaskEmpty
Property Aspose.Imaging.FileFormats.Psd.Resources.QuickMaskInformationResource.MinimalVersion
Property Aspose.Imaging.FileFormats.Psd.Resources.UnicodeAlphaNamesResource.AlphaNames
Property Aspose.Imaging.FileFormats.Psd.Resources.UnicodeAlphaNamesResource.DataSize
Property Aspose.Imaging.FileFormats.Psd.Resources.UnicodeAlphaNamesResource.MinimalVersion
Property Aspose.Imaging.FileFormats.Psd.Resources.UrlListResource.Count
Property Aspose.Imaging.FileFormats.Psd.Resources.UrlListResource.DataSize
Property Aspose.Imaging.FileFormats.Psd.Resources.UrlListResource.Ids
Property Aspose.Imaging.FileFormats.Psd.Resources.UrlListResource.Longs
Property Aspose.Imaging.FileFormats.Psd.Resources.UrlListResource.MinimalVersion
Property Aspose.Imaging.FileFormats.Psd.Resources.UrlListResource.Texts
Property Aspose.Imaging.FileFormats.Psd.Resources.VersionInfoResource.DataSize
Property Aspose.Imaging.FileFormats.Psd.Resources.VersionInfoResource.FileVersion
Property Aspose.Imaging.FileFormats.Psd.Resources.VersionInfoResource.HasRealMergedData
Property Aspose.Imaging.FileFormats.Psd.Resources.VersionInfoResource.MinimalVersion
Property Aspose.Imaging.FileFormats.Psd.Resources.VersionInfoResource.ReaderName
Property Aspose.Imaging.FileFormats.Psd.Resources.VersionInfoResource.Version
Property Aspose.Imaging.FileFormats.Psd.Resources.VersionInfoResource.WriterName
Property Aspose.Imaging.FileFormats.Psd.Resources.WatermarkResource.DataSize
Property Aspose.Imaging.FileFormats.Psd.Resources.WatermarkResource.IsWatermark
Property Aspose.Imaging.FileFormats.Psd.Resources.WatermarkResource.MinimalVersion
Property Aspose.Imaging.ImageLoadOptions.PsdLoadOptions.DefaultReplacementFont
Property Aspose.Imaging.ImageLoadOptions.PsdLoadOptions.LoadEffectsResource
Property Aspose.Imaging.ImageLoadOptions.PsdLoadOptions.ReadOnlyMode
Property Aspose.Imaging.ImageLoadOptions.PsdLoadOptions.UseDiskForLoadEffectsResource
Property Aspose.Imaging.ImageOptions.JpegOptions.HorizontalSampling
Property Aspose.Imaging.ImageOptions.JpegOptions.JpegLsAllowedLossyError
Property Aspose.Imaging.ImageOptions.JpegOptions.JpegLsInterleaveMode
Property Aspose.Imaging.ImageOptions.JpegOptions.JpegLsPreset
Property Aspose.Imaging.ImageOptions.JpegOptions.SampleRoundingMode
Property Aspose.Imaging.ImageOptions.JpegOptions.VerticalSampling
Property Aspose.Imaging.RasterImage.UseRawData


## **Removed APIs:**
Method Aspose.Imaging.FileFormats.Dicom.DicomImage.#ctor(System.String)
