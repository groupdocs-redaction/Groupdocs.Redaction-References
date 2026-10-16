---
title: "PageInfo"
second_title: "GroupDocs.Redaction voor .NET API-referentie"
description: "Stelt beknopte paginainformatie voor."
type: docs
weight: 480
url: /nl/net/groupdocs.redaction/pageinfo/
---
## PageInfo class

Stelt beknopte paginainformatie voor.

```csharp
public class PageInfo
```

## Constructors

| Naam | Beschrijving |
| --- | --- |
| [PageInfo](pageinfo)() | De standaardconstructor. |

## Properties

| Naam | Beschrijving |
| --- | --- |
| [Height](../../groupdocs.redaction/pageinfo/height) { get; set; } | Haalt de paginahoogte op of stelt deze in. |
| [PageNumber](../../groupdocs.redaction/pageinfo/pagenumber) { get; set; } | Haalt het paginanummer op of stelt dit in. |
| [Width](../../groupdocs.redaction/pageinfo/width) { get; set; } | Haalt de paginabreedte op of stelt deze in. |

### Opmerkingen

**Learn more**

* [Get file info](https://docs.groupdocs.com/redaction/net/get-file-info/)

### Voorbeelden

Het volgende voorbeeld toont hoe de algemene documentinformatie op te halen met behulp van [`IDocumentInfo`](../idocumentinfo).

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

### Zie ook

* namespace [GroupDocs.Redaction](../../groupdocs.redaction)
* assembly [GroupDocs.Redaction](../../)

<!-- NIET BEWERKEN: gegenereerd door xmldocmd voor GroupDocs.Redaction.dll -->
