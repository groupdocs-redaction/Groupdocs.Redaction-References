---
title: "PageInfo"
second_title: "GroupDocs.Redaction για .NET API Reference"
description: "Αντιπροσωπεύει σύντομες πληροφορίες σελίδας."
type: docs
weight: 480
url: /el/net/groupdocs.redaction/pageinfo/
---
## PageInfo class

Αντιπροσωπεύει σύντομες πληροφορίες σελίδας.

```csharp
public class PageInfo
```

## Κατασκευαστές

| Όνομα | Περιγραφή |
| --- | --- |
| [PageInfo](pageinfo)() | Ο προεπιλεγμένος κατασκευαστής. |

## Ιδιότητες

| Όνομα | Περιγραφή |
| --- | --- |
| [Height](../../groupdocs.redaction/pageinfo/height) { get; set; } | Λαμβάνει ή ορίζει το ύψος της σελίδας. |
| [PageNumber](../../groupdocs.redaction/pageinfo/pagenumber) { get; set; } | Λαμβάνει ή ορίζει τον αριθμό της σελίδας. |
| [Width](../../groupdocs.redaction/pageinfo/width) { get; set; } | Λαμβάνει ή ορίζει το πλάτος της σελίδας. |

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
