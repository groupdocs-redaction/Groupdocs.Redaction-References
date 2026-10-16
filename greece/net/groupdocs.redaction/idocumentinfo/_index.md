---
title: "IDocumentInfo"
second_title: "GroupDocs.Redaction για .NET API Reference"
description: "Ορίζει μεθόδους που απαιτούνται για την λήψη βασικών πληροφοριών εγγράφου."
type: docs
weight: 100
url: /el/net/groupdocs.redaction/idocumentinfo/
---
## IDocumentInfo interface

Ορίζει μεθόδους που απαιτούνται για την λήψη βασικών πληροφοριών εγγράφου.

```csharp
public interface IDocumentInfo
```

## Ιδιότητες

| Όνομα | Περιγραφή |
| --- | --- |
| [FileType](../../groupdocs.redaction/idocumentinfo/filetype) { get; } | Λαμβάνει την περιγραφή μορφής αρχείου. |
| [PageCount](../../groupdocs.redaction/idocumentinfo/pagecount) { get; } | Λαμβάνει το συνολικό αριθμό σελίδων. |
| [Pages](../../groupdocs.redaction/idocumentinfo/pages) { get; } | Λαμβάνει τη λίστα των πληροφοριών σελίδας [`PageInfo`](../pageinfo). |
| [Size](../../groupdocs.redaction/idocumentinfo/size) { get; } | Λαμβάνει το μέγεθος του εγγράφου σε bytes. |

### Παρατηρήσεις

**Learn more**

* [Get file info](https://docs.groupdocs.com/redaction/net/get-file-info/)

### Παραδείγματα

Το παρακάτω παράδειγμα δείχνει πώς να ανακτήσετε τις γενικές πληροφορίες εγγράφου χρησιμοποιώντας το [`IDocumentInfo`](../idocumentinfo).

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

### Δείτε επίσης

* namespace [GroupDocs.Redaction](../../groupdocs.redaction)
* assembly [GroupDocs.Redaction](../../)

<!-- ΜΗΝ ΕΠΕΞΕΡΓΑΣΕΤΕ: δημιουργήθηκε από το xmldocmd για το GroupDocs.Redaction.dll -->
