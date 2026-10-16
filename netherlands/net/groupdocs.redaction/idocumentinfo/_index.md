---
title: "IDocumentInfo"
second_title: "GroupDocs.Redaction voor .NET API-referentie"
description: "Definieert methoden die nodig zijn om basisdocumentinformatie op te halen."
type: docs
weight: 100
url: /nl/net/groupdocs.redaction/idocumentinfo/
---
## IDocumentInfo interface

Definieert methoden die nodig zijn om basisdocumentinformatie op te halen.

```csharp
public interface IDocumentInfo
```

## Properties

| Naam | Beschrijving |
| --- | --- |
| [FileType](../../groupdocs.redaction/idocumentinfo/filetype) { get; } | Haalt de bestandsformaatbeschrijving op. |
| [PageCount](../../groupdocs.redaction/idocumentinfo/pagecount) { get; } | Haalt het totale paginatelling op. |
| [Pages](../../groupdocs.redaction/idocumentinfo/pages) { get; } | Haalt de lijst met [`PageInfo`](../pageinfo) paginainformatie op. |
| [Size](../../groupdocs.redaction/idocumentinfo/size) { get; } | Haalt de documentgrootte in bytes op. |

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
