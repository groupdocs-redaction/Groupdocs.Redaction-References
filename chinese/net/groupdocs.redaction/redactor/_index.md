---
title: "Redactor"
second_title: "GroupDocs.Redaction 适用于 .NET 的 API 参考"
description: "表示控制文档删除过程的主类，允许打开、删除和保存文档。"
type: docs
weight: 820
url: /zh/net/groupdocs.redaction/redactor/
---
## Redactor class

表示控制文档编辑过程的主类，允许打开、编辑和保存文档。

```csharp
public sealed class Redactor : IDisposable, IPreviewable
```

## 构造函数

| 名称 | 描述 |
| --- | --- |
| [Redactor](redactor#constructor)(Stream) | 使用流初始化 [`Redactor`](../redactor) 类的新实例。 |
| [Redactor](redactor#constructor_3)(string) | 使用文件路径初始化 [`Redactor`](../redactor) 类的新实例。 |
| [Redactor](redactor#constructor_1)(Stream, LoadOptions) | 使用流为受密码保护的文档初始化 [`Redactor`](../redactor) 类的新实例。 |
| [Redactor](redactor#constructor_4)(string, LoadOptions) | 使用其路径为受密码保护的文档初始化 [`Redactor`](../redactor) 类的新实例。 |
| [Redactor](redactor#constructor_2)(Stream, LoadOptions, RedactorSettings) | 使用流和设置为受密码保护的文档初始化 [`Redactor`](../redactor) 类的新实例。 |
| [Redactor](redactor#constructor_5)(string, LoadOptions, RedactorSettings) | 使用其路径和设置为受密码保护的文档初始化 [`Redactor`](../redactor) 类的新实例。 |

## 方法

| 名称 | 描述 |
| --- | --- |
| [Apply](../../groupdocs.redaction/redactor/apply#apply)(Redaction) | 对文档应用遮蔽。 |
| [Apply](../../groupdocs.redaction/redactor/apply#apply_1)(RedactionPolicy) | 对文档应用遮蔽策略。 |
| [Apply](../../groupdocs.redaction/redactor/apply#apply_2)(Redaction[]) | 对文档应用一组遮蔽。 |
| [Dispose](../../groupdocs.redaction/redactor/dispose)() | 释放资源。 |
| [GeneratePreview](../../groupdocs.redaction/redactor/generatepreview)(PreviewOptions) | 生成特定页面的预览图像，使用给定的图像格式。 |
| [GetDocumentInfo](../../groupdocs.redaction/redactor/getdocumentinfo)() | 获取文档的一般信息——大小、页数等。 |
| [Save](../../groupdocs.redaction/redactor/save#save)() | 将文档保存到文件，并使用以下选项：AddSuffix = true，RasterizeToPDF = true。 |
| [Save](../../groupdocs.redaction/redactor/save#save_1)(SaveOptions) | 将文档保存到文件。 |
| [Save](../../groupdocs.redaction/redactor/save#save_3)(Stream, SaveOptions) | 将文档保存到指定的流。 |

### 备注

**Learn more**

* More details about applying redactions: [Redaction basics](https://docs.groupdocs.com/redaction/net/redaction-basics/)
* More advanced redaction topics: [Advanced usage](https://docs.groupdocs.com/redaction/net/advanced-usage/)

### 示例

以下示例演示了对文档应用单个遮蔽。

```csharp
using (Redactor redactor = new Redactor(@"D:\\test.docx"))
{
   RedactorChangeLog result = redactor.Apply(new RegexRedaction(LookupStrings.SSNRegexPattern, new ReplacementOptions("[ssn]")));
   if (result.Status != RedactionStatus.Failed)
   {
      redactor.Save();
   };
}
```

以下示例演示了对文档应用遮蔽列表。

```csharp
using (Redactor redactor = new Redactor(@"D:\\test.docx"))
{
var redactionList = new Redaction[]
{
new ExactPhraseRedaction(LookupStrings.ClientName, new ReplacementOptions("[client]")),
new ExactPhraseRedaction(LookupStrings.ClientAddress, new ReplacementOptions(GroupDocs.Redaction.Options.Drawing.Color.Red)),
new RegexRedaction(LookupStrings.SSNRegexPattern, new ReplacementOptions("[ssn]")),
new RegexRedaction(LookupStrings.BankCardRegexPattern, new ReplacementOptions(GroupDocs.Redaction.Options.Drawing.Color.Blue)),
// ... 其他遮蔽
new DeleteAnnotationRedaction("(?im:(use|show|describe))"),
new EraseMetadataRedaction(MetadataFilter.Author),
new MetadataSearchRedaction(LookupStrings.CompanyName, "--company--")
};
RedactorChangeLog result = redactor.Apply(redactionList);
// false，如果至少有一个遮蔽失败
if (result.Status != RedactionStatus.Failed)
{
redactor.Save();
};
}
```

以下示例演示如何将编辑策略应用于给定入站文件夹中的所有文件，并保存到出站文件夹之一——分别用于成功更新的文件和失败的文件。

```csharp
RedactionPolicy policy = RedactionPolicy.Load("RedactionPolicy.xml");
foreach (var fileEntry in Directory.GetFileNames("C:\\Inbound")) 
{
     using (Redactor redactor = new Redactor(Path.Combine("C:\\Inbound\\", fileEntry)))
     {
    	     RedactorChangeLog result = redactor.Apply(policy);
    	     String resultFolder = result.Status != RedactionStatus.Failed ? "C:\\Outbound\\Done\\" : "C:\\Outbound\\Failed\\";
    	     using (Stream fileStream = File.Open(Path.Combine(resultFolder, fileEntry), FileMode.Open, FileAccess.ReadWrite))
   	     {
               redactor.Save(fileStream, new RasterizationOptions() { Enabled = false });
   	     }        
     }
}   
```

以下示例演示了如何使用 LoadOptions 打开受密码保护的文档。

```csharp
LoadOptions loadOptions = new LoadOptions("mypassword");
using (Redactor redactor = new Redactor(@"C:\sample.pdf", loadOptions))
{
    // 这里我们可以使用文档实例执行遮蔽。
}
```

以下示例演示如何使用 SaveOptions 保存文档。

```csharp
    using (Redactor redactor = new Redactor(@"C:\sample.pdf"))
    {
       // 文档脱敏在此处
       // ...
    
       // 使用默认选项保存文档（将页面转换为图像，保存为 PDF）
       redactor.Save();
    
       // 以原始格式保存文档，覆盖原文件
       redactor.Save(new SaveOptions() { AddSuffix = false, RasterizeToPDF = false });
    
       // 以原始格式将文档保存为 "*_Redacted.*" 文件
       redactor.Save(new SaveOptions() { AddSuffix = true, RasterizeToPDF = false });
    
       // 在文件名中不进行光栅化，将文档保存为 "*_AnyText.*"（例如将 "AnyText" 替换为时间戳）
       redactor.Save(new SaveOptions(false, "AnyText"));
    }    
```

### 另见

* interface [IPreviewable](../../groupdocs.redaction.integration/ipreviewable)
* namespace [GroupDocs.Redaction](../../groupdocs.redaction)
* assembly [GroupDocs.Redaction](../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Redaction.dll -->
