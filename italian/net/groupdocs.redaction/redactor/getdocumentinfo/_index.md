---
title: "GetDocumentInfo"
second_title: "Riferimento API di GroupDocs.Redaction per .NET"
description: "Ottiene le informazioni generali sul documento, dimensione, numero di pagine, ecc."
type: docs
weight: 50
url: /it/net/groupdocs.redaction/redactor/getdocumentinfo/
---
## Redactor.GetDocumentInfo method

Ottiene le informazioni generali sul documento - dimensione, numero di pagine, ecc.

```csharp
public IDocumentInfo GetDocumentInfo()
```

### Valore di ritorno

Un'istanza di IDocumentInfo

### Esempi

Il seguente esempio dimostra come recuperare le informazioni generali del documento utilizzando [`IDocumentInfo`](../../idocumentinfo).

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

* interface [IDocumentInfo](../../idocumentinfo)
* class [Redactor](../../redactor)
* namespace [GroupDocs.Redaction](../../../groupdocs.redaction)
* assembly [GroupDocs.Redaction](../../../)

<!-- NON MODIFICARE: generato da xmldocmd per GroupDocs.Redaction.dll -->
