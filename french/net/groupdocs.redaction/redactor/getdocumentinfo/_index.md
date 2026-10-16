---
title: "GetDocumentInfo"
second_title: "Référence API de GroupDocs.Redaction pour .NET"
description: "Obtient les informations générales sur le document, taille, nombre de pages, etc."
type: docs
weight: 50
url: /fr/net/groupdocs.redaction/redactor/getdocumentinfo/
---
## Redactor.GetDocumentInfo method

Obtient les informations générales sur le document – taille, nombre de pages, etc.

```csharp
public IDocumentInfo GetDocumentInfo()
```

### Valeur de retour

Une instance de IDocumentInfo

### Exemples

L'exemple suivant montre comment récupérer les informations générales du document en utilisant [`IDocumentInfo`](../../idocumentinfo).

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

### Voir aussi

* interface [IDocumentInfo](../../idocumentinfo)
* class [Redactor](../../redactor)
* namespace [GroupDocs.Redaction](../../../groupdocs.redaction)
* assembly [GroupDocs.Redaction](../../../)

<!-- NE PAS MODIFIER : généré par xmldocmd pour GroupDocs.Redaction.dll -->
