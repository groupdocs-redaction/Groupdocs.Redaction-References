---
title: "IRedactionCallback"
second_title: "GroupDocs.Redaction για .NET API Reference"
description: "Ορίζει μεθόδους που απαιτούνται για τη λήψη πληροφοριών για κάθε αλλαγή διαγραφής και προαιρετικά την αποτροπή της."
type: docs
weight: 620
url: /el/net/groupdocs.redaction.redactions/iredactioncallback/
---
## IRedactionCallback interface

Ορίζει μεθόδους που απαιτούνται για τη λήψη πληροφοριών για κάθε αλλαγή διαγραφής και προαιρετικά την αποτροπή της.

```csharp
public interface IRedactionCallback
```

## Μέθοδοι

| Όνομα | Περιγραφή |
| --- | --- |
| [AcceptRedaction](../../groupdocs.redaction.redactions/iredactioncallback/acceptredaction)(RedactionDescription) | Αυτή η κλήση ενεργοποιείται ακριβώς πριν την εφαρμογή οποιασδήποτε διαγραφής στο έγγραφο και επιτρέπει την καταγραφή ή την απαγόρευσή της. |

### Παρατηρήσεις

**Learn more**

* More details about implementing IRedactionCallback interface: [Use redaction callback](https://docs.groupdocs.com/redaction/net/use-redaction-callback/)

### Παραδείγματα

Το παρακάτω παράδειγμα δείχνει πώς να υλοποιήσετε λεπτομερή καταγραφή για τη διαδικασία διαγραφής.

```csharp
public class RedactionDump : IRedactionCallback
{
    public RedactionDump()
    {
    }

    public bool AcceptRedaction(RedactionDescription description)
    {
        Console.Write("{0} redaction, {1} action, item {2}. ", description.RedactionType, description.ActionType, description.OriginalText);
        if (description.Replacement != null)
        {
            Console.Write("Text {0} is replaced with {1}. ", description.Replacement.OriginalText, description.Replacement.Replacement);
        }
        Console.WriteLine();
        // μπορείτε να επιστρέψετε "false" εδώ για να αποτρέψετε συγκεκριμένη αλλαγή κατά τη διαδικασία διαγραφής
        return true;
    }
}

...

// Αναθέστε μια παρουσία πριν χρησιμοποιήσετε το Redactor
Redactor.RedactionCallback = new RedactionDump();
```

### Δείτε επίσης

* namespace [GroupDocs.Redaction.Redactions](../../groupdocs.redaction.redactions)
* assembly [GroupDocs.Redaction](../../)

<!-- ΜΗΝ ΕΠΕΞΕΡΓΑΣΕΤΕ: δημιουργήθηκε από το xmldocmd για το GroupDocs.Redaction.dll -->
