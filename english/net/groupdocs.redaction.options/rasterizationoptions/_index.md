---
title: RasterizationOptions
second_title: GroupDocs.Redaction for .NET API Reference
description: Provides options for converting files into PDF.
type: docs
weight: 350
url: /net/groupdocs.redaction.options/rasterizationoptions/
---
## RasterizationOptions class

Provides options for converting files into PDF.

```csharp
public class RasterizationOptions
```

## Constructors

| Name | Description |
| --- | --- |
| [RasterizationOptions](rasterizationoptions)() | Initializes a new instance. |

## Properties

| Name | Description |
| --- | --- |
| [Compliance](../../groupdocs.redaction.options/rasterizationoptions/compliance) { get; set; } | Gets or sets the PDF Compliance level. |
| [Enabled](../../groupdocs.redaction.options/rasterizationoptions/enabled) { get; set; } | Gets or sets a value indicating whether all pages in the document need to be converted to images and put in a single PDF file. TRUE by default, set to FALSE in order to avoid rasterization. |
| [HasAdvancedOptions](../../groupdocs.redaction.options/rasterizationoptions/hasadvancedoptions) { get; } | Gets an indicator, which is true if advanced rasterization options are set. |
| [PageCount](../../groupdocs.redaction.options/rasterizationoptions/pagecount) { get; set; } | Gets or sets the number of pages to be converted into PDF. |
| [PageIndex](../../groupdocs.redaction.options/rasterizationoptions/pageindex) { get; set; } | Gets or sets the index of the first page (0-based) to convert into PDF. |

## Methods

| Name | Description |
| --- | --- |
| [AddAdvancedOption](../../groupdocs.redaction.options/rasterizationoptions/addadvancedoption#addadvancedoption)(AdvancedRasterizationOptions) | You can use this method to register an advanced rasterization option to apply. |
| [AddAdvancedOption](../../groupdocs.redaction.options/rasterizationoptions/addadvancedoption#addadvancedoption_1)(AdvancedRasterizationOptions, Dictionary&lt;string, string&gt;) | You can use this method to register an advanced rasterization option to apply. |

### Remarks

**Learn more**

* More details about saving document as a rasterized PDF: [Save in rasterized PDF](https://docs.groupdocs.com/redaction/net/save-in-rasterized-pdf/)
* More details about rasterization options: [Select specific pages for rasterized PDF](https://docs.groupdocs.com/redaction/net/select-specific-pages-for-rasterized-pdf/)

### Examples

The following example demonstrates how to set options for the rasterization process.

```csharp
    using (var redactor = new Redactor("SomePresentation.pptx"))
    {
        // redact sensitive data on the first slide 
    
        var rasterizationOptions = new RasterizationOptions();
        rasterizationOptions.PageIndex = 0;
        rasterizationOptions.PageCount = 1;
        rasterizationOptions.Compliance = PdfComplianceLevel.PdfA1a;
        using (var stream = File.Open(Path.Combine(@"C:\Temp", "PresentationFirstSlide.pdf")))
        {
            redactor.Save(stream, rasterizationOptions);
        }
    }      
```

The following example demonstrates how to apply the advanced rasterization options with default settings.

```csharp
    using (Redactor redactor = new Redactor(@"C:\sample.docx"))
    {
      // Save the document with default options (convert pages into images, save as PDF)
      var so = new SaveOptions();
      so.Rasterization.Enabled = true;
      so.RedactedFileSuffix = "_scan";
      so.Rasterization.AddAdvancedOption(AdvancedRasterizationOptions.Border);
      so.Rasterization.AddAdvancedOption(AdvancedRasterizationOptions.Noise);
      so.Rasterization.AddAdvancedOption(AdvancedRasterizationOptions.Grayscale);
      so.Rasterization.AddAdvancedOption(AdvancedRasterizationOptions.Tilt);
      redactor.Save(so);
    }
```

The following example demonstrates how to apply the border advanced rasterization option with custom settings.

```csharp
    using (Redactor redactor = new Redactor(@"C:\sample.docx"))
    {
      // Save the document with a custom border
      var so = new SaveOptions();
      so.Rasterization.Enabled = true;
      so.RedactedFileSuffix = "_scan";
      so.Rasterization.AddAdvancedOption(AdvancedRasterizationOptions.Border, new Dictionary<string, string>() { { "border", "10" } });
      redactor.Save(so);
    }
```

The following example demonstrates how to apply the noise advanced rasterization option with custom settings.

```csharp
    using (Redactor redactor = new Redactor(@"C:\sample.docx"))
    {
      // Save the document with the custom number and size of noise effects
      var so = new SaveOptions();
      so.Rasterization.Enabled = true;
      so.RedactedFileSuffix = "_scan";
      so.Rasterization.AddAdvancedOption(AdvancedRasterizationOptions.Noise, 
          new Dictionary<string, string>() { { "maxSpots", "150" }, { "spotMaxSize", "15" } });
      redactor.Save(so);
    }
```

The following example demonstrates how to apply the tilt advanced rasterization option with custom settings.

```csharp
    using (Redactor redactor = new Redactor(@"C:\sample.docx"))
    {
      // Save the document with the custom tilt effect
      var so = new SaveOptions();
      so.Rasterization.Enabled = true;
      so.RedactedFileSuffix = "_scan";
      so.Rasterization.AddAdvancedOption(AdvancedRasterizationOptions.Tilt, 
          new Dictionary<string, string>() { { { "minAngle", "85" }, { "randomAngleMax", "5" } });
      redactor.Save(so);
    }
```

### See Also

* namespace [GroupDocs.Redaction.Options](../../groupdocs.redaction.options)
* assembly [GroupDocs.Redaction](../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.redaction.dll -->
