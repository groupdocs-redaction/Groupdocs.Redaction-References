---
title: "GetDocumentInfo"
second_title: "GroupDocs.Redaction voor .NET API-referentie"
description: "Haalt de algemene informatie over het document op, zoals grootte, paginatelling, enz."
type: docs
weight: 50
url: /nl/net/groupdocs.redaction/redactor/getdocumentinfo/
---
## Redactor.GetDocumentInfo method

Haalt de algemene informatie over het document op - grootte, paginatelling, enz.

```csharp
public IDocumentInfo GetDocumentInfo()
```

### Retourwaarde

Een instantie van IDocumentInfo

### Voorbeelden

Het volgende voorbeeld toont hoe de algemene documentinformatie kan worden opgehaald met behulp van [`IDocumentInfo`](../../idocumentinfo).

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

* interface [IDocumentInfo](../../idocumentinfo)
* class [Redactor](../../redactor)
* namespace [GroupDocs.Redaction](../../../groupdocs.redaction)
* assembly [GroupDocs.Redaction](../../../)

<!-- NIET BEWERKEN: gegenereerd door xmldocmd voor GroupDocs.Redaction.dll -->
