---
title: "IDocumentInfo"
second_title: "Référence API de GroupDocs.Redaction pour .NET"
description: "Définit les méthodes nécessaires pour obtenir les informations de base du document."
type: docs
weight: 100
url: /fr/net/groupdocs.redaction/idocumentinfo/
---
## IDocumentInfo interface

Définit les méthodes nécessaires pour obtenir les informations de base du document.

```csharp
public interface IDocumentInfo
```

## Propriétés

| Nom | Description |
| --- | --- |
| [FileType](../../groupdocs.redaction/idocumentinfo/filetype) { get; } | Obtient la description du format de fichier. |
| [PageCount](../../groupdocs.redaction/idocumentinfo/pagecount) { get; } | Obtient le nombre total de pages. |
| [Pages](../../groupdocs.redaction/idocumentinfo/pages) { get; } | Obtient la liste des informations de page [`PageInfo`](../pageinfo). |
| [Size](../../groupdocs.redaction/idocumentinfo/size) { get; } | Obtient la taille du document en octets. |

### Remarques

**Learn more**

* [Get file info](https://docs.groupdocs.com/redaction/net/get-file-info/)

### Exemples

L'exemple suivant montre comment récupérer les informations générales du document en utilisant [`IDocumentInfo`](../idocumentinfo).

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

* namespace [GroupDocs.Redaction](../../groupdocs.redaction)
* assembly [GroupDocs.Redaction](../../)

<!-- NE PAS MODIFIER : généré par xmldocmd pour GroupDocs.Redaction.dll -->
