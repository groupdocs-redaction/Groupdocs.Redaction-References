---
title: "PageInfo"
second_title: "GroupDocs.Redaction för .NET API-referens"
description: "Representerar kort information om en sida."
type: docs
weight: 480
url: /sv/net/groupdocs.redaction/pageinfo/
---
## PageInfo class

Representerar kort information om en sida.

```csharp
public class PageInfo
```

## Konstruktörer

| Namn | Beskrivning |
| --- | --- |
| [PageInfo](pageinfo)() | Standardkonstruktorn. |

## Egenskaper

| Namn | Beskrivning |
| --- | --- |
| [Height](../../groupdocs.redaction/pageinfo/height) { get; set; } | Hämtar eller anger sidans höjd. |
| [PageNumber](../../groupdocs.redaction/pageinfo/pagenumber) { get; set; } | Hämtar eller anger sidnummer. |
| [Width](../../groupdocs.redaction/pageinfo/width) { get; set; } | Hämtar eller anger sidans bredd. |

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
