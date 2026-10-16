---
title: "PageInfo"
second_title: "Référence API de GroupDocs.Redaction pour .NET"
description: "Représente une brève information de page."
type: docs
weight: 480
url: /fr/net/groupdocs.redaction/pageinfo/
---
## PageInfo class

Représente une brève information de page.

```csharp
public class PageInfo
```

## Constructeurs

| Nom | Description |
| --- | --- |
| [PageInfo](pageinfo)() | Le constructeur par défaut. |

## Propriétés

| Nom | Description |
| --- | --- |
| [Height](../../groupdocs.redaction/pageinfo/height) { get; set; } | Obtient ou définit la hauteur de la page. |
| [PageNumber](../../groupdocs.redaction/pageinfo/pagenumber) { get; set; } | Obtient ou définit le numéro de la page. |
| [Width](../../groupdocs.redaction/pageinfo/width) { get; set; } | Obtient ou définit la largeur de la page. |

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
