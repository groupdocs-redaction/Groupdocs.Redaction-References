---
title: PageInfo
second_title: Référence de l'API GroupDocs.Redaction pour .NET
description: Représente une brève page dinformations.
type: docs
weight: 380
url: /fr/net/groupdocs.redaction/pageinfo/
---
## PageInfo class

Représente une brève page d'informations.

```csharp
public class PageInfo
```

## Constructeurs

| Nom | La description |
| --- | --- |
| [PageInfo](pageinfo)() | Default_Constructor |

## Propriétés

| Nom | La description |
| --- | --- |
| [Height](../../groupdocs.redaction/pageinfo/height) { get; set; } | Obtient ou définit la hauteur de la page. |
| [PageNumber](../../groupdocs.redaction/pageinfo/pagenumber) { get; set; } | Obtient ou définit le numéro de page. |
| [Width](../../groupdocs.redaction/pageinfo/width) { get; set; } | Obtient ou définit la largeur de la page. |

### Remarques

**Apprendre encore plus**

* [Obtenir des informations sur le fichier](https://docs.groupdocs.com/redaction/net/get-file-info/)

### Exemples

L'exemple suivant montre comment récupérer les informations générales du document à l'aide de[`IDocumentInfo`](../idocumentinfo).

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

### Voir également

* espace de noms [GroupDocs.Redaction](../../groupdocs.redaction)
* Assemblée [GroupDocs.Redaction](../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Redaction.dll -->