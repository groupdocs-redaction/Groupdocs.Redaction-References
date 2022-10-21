---
title: Redactor
second_title: GroupDocs.Redaction for .NET API 参考
description: 表示控制文档编辑过程的主类允许打开编辑和保存文档
type: docs
weight: 650
url: /zh/net/groupdocs.redaction/redactor/
---
## Redactor class

表示控制文档编辑过程的主类，允许打开、编辑和保存文档。

```csharp
public sealed class Redactor : IDisposable, IPreviewable
```

## 构造函数

| 姓名 | 描述 |
| --- | --- |
| [Redactor](redactor#constructor)(Stream) | 初始化一个新的实例[`Redactor`](../redactor)使用流的类. |
| [Redactor](redactor#constructor_3)(string) | 初始化一个新的实例[`Redactor`](../redactor)使用文件路径的类. |
| [Redactor](redactor#constructor_1)(Stream, LoadOptions) | 初始化一个新的实例[`Redactor`](../redactor)使用 stream. 的受密码保护文档的类 |
| [Redactor](redactor#constructor_4)(string, LoadOptions) | 初始化一个新的实例[`Redactor`](../redactor)使用其路径的受密码保护文档的类. |
| [Redactor](redactor#constructor_2)(Stream, LoadOptions, RedactorSettings) | 初始化一个新的实例[`Redactor`](../redactor)使用流和设置的受密码保护文档的类。 |
| [Redactor](redactor#constructor_5)(string, LoadOptions, RedactorSettings) | 初始化一个新的实例[`Redactor`](../redactor)使用其路径和设置的受密码保护文档的类。 |

## 方法

| 姓名 | 描述 |
| --- | --- |
| [Apply](../../groupdocs.redaction/redactor/apply#apply)(Redaction) | 对文档应用编辑。 |
| [Apply](../../groupdocs.redaction/redactor/apply#apply_1)(RedactionPolicy) | 对文档应用密文策略。 |
| [Apply](../../groupdocs.redaction/redactor/apply#apply_2)(Redaction[]) | 对文档应用一组密文。 |
| [Dispose](../../groupdocs.redaction/redactor/dispose)() | 释放资源。 |
| [GeneratePreview](../../groupdocs.redaction/redactor/generatepreview)(PreviewOptions) | 以给定的图像格式生成特定页面的预览图像。 |
| [GetDocumentInfo](../../groupdocs.redaction/redactor/getdocumentinfo)() | 获取有关文档的一般信息 - 大小、页数等。 |
| [Save](../../groupdocs.redaction/redactor/save#save)() | 使用以下选项将文档保存到文件中：AddSuffix = true, RasterizeToPDF = true. |
| [Save](../../groupdocs.redaction/redactor/save#save_1)(SaveOptions) | 将文档保存到文件中。 |
| [Save](../../groupdocs.redaction/redactor/save#save_2)(Stream, RasterizationOptions) | 将文档保存到流中，包括自定义位置。 |

### 评论

**学到更多**

* 有关应用编辑的更多详细信息： [编辑基础知识](https://docs.groupdocs.com/redaction/net/redaction-basics/)
* 更高级的修订主题： [高级用法](https://docs.groupdocs.com/redaction/net/advanced-usage/)

### 例子

以下示例演示了对文档应用单个编辑。

以下示例演示了将密文列表应用于文档。

以下示例演示如何将编辑策略应用于给定入站文件夹中的所有文件，并保存到出站文件夹之一 - 用于成功更新的文件和失败的文件。

下面的示例演示如何使用 LoadOptions 打开受密码保护的文档。

以下示例演示如何使用 SaveOptions 保存文档。

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

```csharp
using (Redactor redactor = new Redactor(@"D:\\test.docx"))
{
   var redactionList = new Redaction[] 
   {
      new ExactPhraseRedaction(LookupStrings.ClientName, new ReplacementOptions("[client]")),
      new ExactPhraseRedaction(LookupStrings.ClientAddress, new ReplacementOptions(System.Drawing.Color.Red)),
      new RegexRedaction(LookupStrings.SSNRegexPattern, new ReplacementOptions("[ssn]")),
      new RegexRedaction(LookupStrings.BankCardRegexPattern, new ReplacementOptions(System.Drawing.Color.Blue)),
      // ... 其他编辑
      new DeleteAnnotationRedaction("(?im:(use|show|describe))"),
      new EraseMetadataRedaction(MetadataFilter.Author),
      new MetadataSearchRedaction(LookupStrings.CompanyName, "--company--") 
   }; 
   RedactorChangeLog result = redactor.Apply(redactionList);
   // false，如果至少一个编辑失败
   if (result.Status != RedactionStatus.Failed)
   {
      redactor.Save();
   };
}
```

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

```csharp
LoadOptions loadOptions = new LoadOptions("mypassword");
using (Redactor redactor = new Redactor(@"C:\sample.pdf", loadOptions))
{
    // 这里我们可以使用文档实例来执行编辑
}
```

```csharp
    using (Redactor redactor = new Redactor(@"C:\sample.pdf"))
    {
       // 文档编辑在这里
       // ...
    
       // 使用默认选项保存文档（将页面转换为图像，另存为 PDF）
       redactor.Save();
    
       // 以原始格式保存文档覆盖原始文件
       redactor.Save(new SaveOptions() { AddSuffix = false, RasterizeToPDF = false });
    
       // 将文档以原始格式保存到“*_Redacted.*”文件
       redactor.Save(new SaveOptions() { AddSuffix = true, RasterizeToPDF = false });
    
       // 将文档保存到其文件名中的“*_AnyText.*”（例如时间戳而不是“AnyText”），无需光栅化
       redactor.Save(new SaveOptions(false, "AnyText"));
    }    
```

### 也可以看看

* interface [IPreviewable](../../groupdocs.redaction.integration/ipreviewable)
* 命名空间 [GroupDocs.Redaction](../../groupdocs.redaction)
* 部件 [GroupDocs.Redaction](../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Redaction.dll -->
