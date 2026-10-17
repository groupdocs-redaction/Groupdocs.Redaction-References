---
title: "IDocumentInfo"
second_title: "GroupDocs.Redaction för .NET API-referens"
description: "Definierar metoder som krävs för att hämta grundläggande dokumentinformation."
type: docs
weight: 100
url: /sv/net/groupdocs.redaction/idocumentinfo/
---
## IDocumentInfo interface

Definierar metoder som krävs för att hämta grundläggande dokumentinformation.

```csharp
public interface IDocumentInfo
```

## Egenskaper

| Namn | Beskrivning |
| --- | --- |
| [FileType](../../groupdocs.redaction/idocumentinfo/filetype) { get; } | Hämtar beskrivningen av filformatet. |
| [PageCount](../../groupdocs.redaction/idocumentinfo/pagecount) { get; } | Hämtar det totala sidantalet. |
| [Pages](../../groupdocs.redaction/idocumentinfo/pages) { get; } | Hämtar listan med [`PageInfo`](../pageinfo) sidinformation. |
| [Size](../../groupdocs.redaction/idocumentinfo/size) { get; } | Hämtar dokumentets storlek i byte. |

### Anmärkningar

**Learn more**

* [Get file info](https://docs.groupdocs.com/redaction/net/get-file-info/)

### Exempel

Följande exempel visar hur man hämtar den allmänna dokumentinformationen med hjälp av [`IDocumentInfo`](../idocumentinfo).

```csharp
    try
    {
        using (Redactor red = new Redactor(@"C:\Temp\testfile.doc"))
        {
            IDocumentInfo docInfo = red.GetDocumentInfo();
            Console.WriteLine("Document size: {0}", docInfo.Size);
            Console.WriteLine("Document format: {0}", docInfo.FileType.FileFormat);
            Console.WriteLine("Document contains {0} pages", docInfo.PageCount);
            foreach (PageInfo page in docInfo.Pages)
            {
                Console.WriteLine("Page {0} size is {1}x{2}", page.PageNumber, page.Width, page.Height);
            }
        }
    }
    catch (GroupDocs.Redaction.Exceptions.PasswordRequiredException)
    {
        Console.WriteLine("You are trying to access document which is password protected. Please, set the password.");
    }
    catch (GroupDocs.Redaction.Exceptions.IncorrectPasswordException)
    {
        Console.WriteLine("The provided password is not valid.");
    }
```

### Se även

* namespace [GroupDocs.Redaction](../../groupdocs.redaction)
* assembly [GroupDocs.Redaction](../../)

<!-- GÅ INTE ATT REDIGERA: genererad av xmldocmd för GroupDocs.Redaction.dll -->
