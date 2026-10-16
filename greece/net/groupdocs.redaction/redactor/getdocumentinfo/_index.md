---
title: "GetDocumentInfo"
second_title: "GroupDocs.Redaction για .NET API Reference"
description: "Λαμβάνει τις γενικές πληροφορίες σχετικά με το έγγραφο, το μέγεθος, τον αριθμό σελίδων κ.λπ."
type: docs
weight: 50
url: /el/net/groupdocs.redaction/redactor/getdocumentinfo/
---
## Redactor.GetDocumentInfo method

Λαμβάνει τις γενικές πληροφορίες για το έγγραφο - μέγεθος, αριθμό σελίδων, κ.λπ.

```csharp
public IDocumentInfo GetDocumentInfo()
```

### Τιμή Επιστροφής

Μία παρουσία του IDocumentInfo

### Παραδείγματα

Το παρακάτω παράδειγμα δείχνει πώς να ανακτήσετε τις γενικές πληροφορίες του εγγράφου χρησιμοποιώντας [`IDocumentInfo`](../../idocumentinfo).

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

* interface [IDocumentInfo](../../idocumentinfo)
* class [Redactor](../../redactor)
* namespace [GroupDocs.Redaction](../../../groupdocs.redaction)
* assembly [GroupDocs.Redaction](../../../)

<!-- ΜΗΝ ΕΠΕΞΕΡΓΑΣΕΤΕ: δημιουργήθηκε από το xmldocmd για το GroupDocs.Redaction.dll -->
