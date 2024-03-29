---
title: AddAdvancedOption
second_title: GroupDocs.Redaction for .NET API 参考
description: 您可以使用此方法注册要应用的高级光栅化选项
type: docs
weight: 70
url: /zh/net/groupdocs.redaction.options/rasterizationoptions/addadvancedoption/
---
## AddAdvancedOption(AdvancedRasterizationOptions) {#addadvancedoption}

您可以使用此方法注册要应用的高级光栅化选项。

```csharp
public void AddAdvancedOption(AdvancedRasterizationOptions optionType)
```

| 范围 | 类型 | 描述 |
| --- | --- | --- |
| optionType | AdvancedRasterizationOptions | 提供有关所选效果类型（灰度、边框等）的信息 |

### 例子

以下示例演示如何使用默认设置应用高级光栅化选项。

```csharp
    using (Redactor redactor = new Redactor(@"C:\sample.docx"))
    {
      // 使用默认选项保存文档（将页面转换为图像，另存为 PDF）
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

### 也可以看看

* enum [AdvancedRasterizationOptions](../../advancedrasterizationoptions)
* class [RasterizationOptions](../../rasterizationoptions)
* 命名空间 [GroupDocs.Redaction.Options](../../rasterizationoptions)
* 部件 [GroupDocs.Redaction](../../../)

---

## AddAdvancedOption(AdvancedRasterizationOptions, Dictionary&lt;string, string&gt;) {#addadvancedoption_1}

您可以使用此方法注册要应用的高级光栅化选项。

```csharp
public void AddAdvancedOption(AdvancedRasterizationOptions optionType, 
    Dictionary<string, string> parameters)
```

| 范围 | 类型 | 描述 |
| --- | --- | --- |
| optionType | AdvancedRasterizationOptions | 提供有关所选效果类型（灰度、边框等）的信息 |
| parameters | Dictionary`2 | 给定效果的参数，例如旋转角度 |

### 例子

以下示例演示如何使用默认设置应用高级光栅化选项。

```csharp
    using (Redactor redactor = new Redactor(@"C:\sample.docx"))
    {
      // 使用默认选项保存文档（将页面转换为图像，另存为 PDF）
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

以下示例演示如何使用自定义设置应用边框高级光栅化选项。

```csharp
    using (Redactor redactor = new Redactor(@"C:\sample.docx"))
    {
      // 保存带有自定义边框的文档
      var so = new SaveOptions();
      so.Rasterization.Enabled = true;
      so.RedactedFileSuffix = "_scan";
      so.Rasterization.AddAdvancedOption(AdvancedRasterizationOptions.Border, new Dictionary<string, string>() { { "border", "10" } });
      redactor.Save(so);
    }
```

以下示例演示如何使用自定义设置应用噪声高级光栅化选项。

```csharp
    using (Redactor redactor = new Redactor(@"C:\sample.docx"))
    {
      // 使用噪声效果的自定义数量和大小保存文档
      var so = new SaveOptions();
      so.Rasterization.Enabled = true;
      so.RedactedFileSuffix = "_scan";
      so.Rasterization.AddAdvancedOption(AdvancedRasterizationOptions.Noise, 
          new Dictionary<string, string>() { { "maxSpots", "150" }, { "spotMaxSize", "15" } });
      redactor.Save(so);
    }
```

以下示例演示了如何使用自定义设置应用倾斜高级光栅化选项。

```csharp
    using (Redactor redactor = new Redactor(@"C:\sample.docx"))
    {
      // 保存带有自定义倾斜效果的文档
      var so = new SaveOptions();
      so.Rasterization.Enabled = true;
      so.RedactedFileSuffix = "_scan";
      so.Rasterization.AddAdvancedOption(AdvancedRasterizationOptions.Tilt, 
          new Dictionary<string, string>() { { { "minAngle", "85" }, { "randomAngleMax", "5" } });
      redactor.Save(so);
    }
```

### 也可以看看

* enum [AdvancedRasterizationOptions](../../advancedrasterizationoptions)
* class [RasterizationOptions](../../rasterizationoptions)
* 命名空间 [GroupDocs.Redaction.Options](../../rasterizationoptions)
* 部件 [GroupDocs.Redaction](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Redaction.dll -->
