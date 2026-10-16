---
title: "PageInfo"
second_title: "Riferimento API di GroupDocs.Redaction per .NET"
description: "Rappresenta una breve informazione di pagina."
type: docs
weight: 480
url: /it/net/groupdocs.redaction/pageinfo/
---
## PageInfo class

Rappresenta una breve informazione di pagina.

```csharp
public class PageInfo
```

## Costruttori

| Nome | Descrizione |
| --- | --- |
| [PageInfo](pageinfo)() | Il costruttore predefinito. |

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [Height](../../groupdocs.redaction/pageinfo/height) { get; set; } | Ottiene o imposta l'altezza della pagina. |
| [PageNumber](../../groupdocs.redaction/pageinfo/pagenumber) { get; set; } | Ottiene o imposta il numero della pagina. |
| [Width](../../groupdocs.redaction/pageinfo/width) { get; set; } | Ottiene o imposta la larghezza della pagina. |

### Osservazioni

**Learn more**

* [Get file info](https://docs.groupdocs.com/redaction/net/get-file-info/)

### Esempi

Il seguente esempio dimostra come recuperare le informazioni generali del documento utilizzando [`IDocumentInfo`](../idocumentinfo).

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

### Vedi anche

* namespace [GroupDocs.Redaction](../../groupdocs.redaction)
* assembly [GroupDocs.Redaction](../../)

<!-- NON MODIFICARE: generato da xmldocmd per GroupDocs.Redaction.dll -->
