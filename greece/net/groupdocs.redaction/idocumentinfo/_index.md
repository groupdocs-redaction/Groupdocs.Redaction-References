---
title: IDocumentInfo
second_title: GroupDocs.Redaction για Αναφορά API .NET
description: Καθορίζει μεθόδους που απαιτούνται για τη λήψη βασικών πληροφοριών εγγράφων.
type: docs
weight: 100
url: /el/net/groupdocs.redaction/idocumentinfo/
---
## IDocumentInfo interface

Καθορίζει μεθόδους που απαιτούνται για τη λήψη βασικών πληροφοριών εγγράφων.

```csharp
public interface IDocumentInfo
```

## Ιδιότητες

| Ονομα | Περιγραφή |
| --- | --- |
| [FileType](../../groupdocs.redaction/idocumentinfo/filetype) { get; } | Λαμβάνει την περιγραφή της μορφής αρχείου. |
| [PageCount](../../groupdocs.redaction/idocumentinfo/pagecount) { get; } | Λαμβάνει τον συνολικό αριθμό σελίδων. |
| [Pages](../../groupdocs.redaction/idocumentinfo/pages) { get; } | Λαμβάνει τη λίστα των[`PageInfo`](../pageinfo) πληροφορίες σελίδας. |
| [Size](../../groupdocs.redaction/idocumentinfo/size) { get; } | Λαμβάνει το μέγεθος του εγγράφου σε byte. |

### Παρατηρήσεις

**Μάθε περισσότερα**

* [Λάβετε πληροφορίες αρχείου](https://docs.groupdocs.com/redaction/net/get-file-info/)

### Παραδείγματα

Το ακόλουθο παράδειγμα δείχνει πώς να ανακτήσετε τις γενικές πληροφορίες του εγγράφου χρησιμοποιώντας[`IDocumentInfo`](../idocumentinfo).

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

* χώρος ονομάτων [GroupDocs.Redaction](../../groupdocs.redaction)
* συνέλευση [GroupDocs.Redaction](../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Redaction.dll -->