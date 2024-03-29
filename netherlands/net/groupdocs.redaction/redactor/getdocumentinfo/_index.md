---
title: GetDocumentInfo
second_title: GroupDocs.Redaction voor .NET API-referentie
description: Krijgt de algemene informatie over het document  grootte aantal paginas etc.
type: docs
weight: 50
url: /nl/net/groupdocs.redaction/redactor/getdocumentinfo/
---
## Redactor.GetDocumentInfo method

Krijgt de algemene informatie over het document - grootte, aantal pagina's, etc.

```csharp
public IDocumentInfo GetDocumentInfo()
```

### Winstwaarde

Een instantie van IDocumentInfo

### Voorbeelden

Het volgende voorbeeld laat zien hoe u de algemene documentinformatie kunt ophalen met behulp van[`IDocumentInfo`](../../idocumentinfo).

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
* naamruimte [GroupDocs.Redaction](../../redactor)
* montage [GroupDocs.Redaction](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Redaction.dll -->
