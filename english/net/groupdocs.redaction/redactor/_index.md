---
title: Redactor
second_title: GroupDocs.Redaction for .NET API Reference
description: Represents a main class that controls document redaction process allowing to open redact and save documents.
type: docs
weight: 690
url: /net/groupdocs.redaction/redactor/
---
## Redactor class

Represents a main class that controls document redaction process, allowing to open, redact and save documents.

```csharp
public sealed class Redactor : IDisposable, IPreviewable
```

## Constructors

| Name | Description |
| --- | --- |
| [Redactor](redactor#constructor)(Stream) | Initializes a new instance of [`Redactor`](../redactor) class using stream. |
| [Redactor](redactor#constructor_3)(string) | Initializes a new instance of [`Redactor`](../redactor) class using file path. |
| [Redactor](redactor#constructor_1)(Stream, LoadOptions) | Initializes a new instance of [`Redactor`](../redactor) class for a password-protected document using stream. |
| [Redactor](redactor#constructor_4)(string, LoadOptions) | Initializes a new instance of [`Redactor`](../redactor) class for a password-protected document using its path. |
| [Redactor](redactor#constructor_2)(Stream, LoadOptions, RedactorSettings) | Initializes a new instance of [`Redactor`](../redactor) class for a password-protected document using stream and settings. |
| [Redactor](redactor#constructor_5)(string, LoadOptions, RedactorSettings) | Initializes a new instance of [`Redactor`](../redactor) class for a password-protected document using its path and settings. |

## Methods

| Name | Description |
| --- | --- |
| [Apply](../../groupdocs.redaction/redactor/apply#apply)(Redaction) | Applies a redaction to the document. |
| [Apply](../../groupdocs.redaction/redactor/apply#apply_1)(RedactionPolicy) | Applies a redaction policy to the document. |
| [Apply](../../groupdocs.redaction/redactor/apply#apply_2)(Redaction[]) | Applies a set of redactions to the document. |
| [Dispose](../../groupdocs.redaction/redactor/dispose)() | Releases resources. |
| [GeneratePreview](../../groupdocs.redaction/redactor/generatepreview)(PreviewOptions) | Generates preview images of specific pages in a given image format. |
| [GetDocumentInfo](../../groupdocs.redaction/redactor/getdocumentinfo)() | Gets the general information about the document - size, page count, etc. |
| [Save](../../groupdocs.redaction/redactor/save#save)() | Saves the document to a file with the following options: AddSuffix = true, RasterizeToPDF = true. |
| [Save](../../groupdocs.redaction/redactor/save#save_1)(SaveOptions) | Saves the document to a file. |
| [Save](../../groupdocs.redaction/redactor/save#save_2)(Stream, RasterizationOptions) | Saves the document to a stream, including custom location. |

### Remarks

**Learn more**

* More details about applying redactions: [Redaction basics](https://docs.groupdocs.com/redaction/net/redaction-basics/)
* More advanced redaction topics: [Advanced usage](https://docs.groupdocs.com/redaction/net/advanced-usage/)

### Examples

The following example demonstrates applying a single redaction to the document.

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

The following example demonstrates applying a list of redactions to the document.

```csharp
using (Redactor redactor = new Redactor(@"D:\\test.docx"))
{
   var redactionList = new Redaction[] 
   {
      new ExactPhraseRedaction(LookupStrings.ClientName, new ReplacementOptions("[client]")),
      new ExactPhraseRedaction(LookupStrings.ClientAddress, new ReplacementOptions(System.Drawing.Color.Red)),
      new RegexRedaction(LookupStrings.SSNRegexPattern, new ReplacementOptions("[ssn]")),
      new RegexRedaction(LookupStrings.BankCardRegexPattern, new ReplacementOptions(System.Drawing.Color.Blue)),
      // ... other redactions
      new DeleteAnnotationRedaction("(?im:(use|show|describe))"),
      new EraseMetadataRedaction(MetadataFilter.Author),
      new MetadataSearchRedaction(LookupStrings.CompanyName, "--company--") 
   }; 
   RedactorChangeLog result = redactor.Apply(redactionList);
   // false, if at least one redaction failed
   if (result.Status != RedactionStatus.Failed)
   {
      redactor.Save();
   };
}
```

The following example demonstrates how to apply a redaction policy to all files within a given inbound folder, and save to one of outbound folders - for successfully updated files and for failed ones.

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

The following example demonstrates how to open a password-protected documents using LoadOptions.

```csharp
LoadOptions loadOptions = new LoadOptions("mypassword");
using (Redactor redactor = new Redactor(@"C:\sample.pdf", loadOptions))
{
    // Here we can use document instance to perform redactions
}
```

The following example demonstrates how to save a document using SaveOptions.

```csharp
    using (Redactor redactor = new Redactor(@"C:\sample.pdf"))
    {
       // Document redaction goes here
       // ...
    
       // Save the document with default options (convert pages into images, save as PDF)
       redactor.Save();
    
       // Save the document in original format overwriting original file
       redactor.Save(new SaveOptions() { AddSuffix = false, RasterizeToPDF = false });
    
       // Save the document to "*_Redacted.*" file in original format
       redactor.Save(new SaveOptions() { AddSuffix = true, RasterizeToPDF = false });
    
       // Save the document to "*_AnyText.*" (e.g. timestamp instead of "AnyText") in its file name without rasterization
       redactor.Save(new SaveOptions(false, "AnyText"));
    }    
```

### See Also

* interface [IPreviewable](../../groupdocs.redaction.integration/ipreviewable)
* namespace [GroupDocs.Redaction](../../groupdocs.redaction)
* assembly [GroupDocs.Redaction](../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.redaction.dll -->
