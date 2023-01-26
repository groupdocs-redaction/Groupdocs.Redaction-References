---
title: AddAdvancedOption
second_title: GroupDocs.Redaction for .NET API Reference
description: You can use this method to register an advanced rasterization option to apply.
type: docs
weight: 70
url: /net/groupdocs.redaction.options/rasterizationoptions/addadvancedoption/
---
## AddAdvancedOption(AdvancedRasterizationOptions) {#addadvancedoption}

You can use this method to register an advanced rasterization option to apply.

```csharp
public void AddAdvancedOption(AdvancedRasterizationOptions optionType)
```

| Parameter | Type | Description |
| --- | --- | --- |
| optionType | AdvancedRasterizationOptions | Provides information about the selected effect type (grayscale, border, etc.) |

### Examples

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

### See Also

* enum [AdvancedRasterizationOptions](../../advancedrasterizationoptions)
* class [RasterizationOptions](../../rasterizationoptions)
* namespace [GroupDocs.Redaction.Options](../../rasterizationoptions)
* assembly [GroupDocs.Redaction](../../../)

---

## AddAdvancedOption(AdvancedRasterizationOptions, Dictionary&lt;string, string&gt;) {#addadvancedoption_1}

You can use this method to register an advanced rasterization option to apply.

```csharp
public void AddAdvancedOption(AdvancedRasterizationOptions optionType, 
    Dictionary<string, string> parameters)
```

| Parameter | Type | Description |
| --- | --- | --- |
| optionType | AdvancedRasterizationOptions | Provides information about the selected effect type (grayscale, border, etc.) |
| parameters | Dictionary`2 | Parameters for the given effect, such as rotation angle |

### Examples

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

* enum [AdvancedRasterizationOptions](../../advancedrasterizationoptions)
* class [RasterizationOptions](../../rasterizationoptions)
* namespace [GroupDocs.Redaction.Options](../../rasterizationoptions)
* assembly [GroupDocs.Redaction](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.redaction.dll -->
