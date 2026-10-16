---
title: "IAnnotatedDocument"
second_title: "GroupDocs.Redaction για .NET API Reference"
description: "Ορίζει μεθόδους που απαιτούνται για πρόσβαση σε σημειώσεις όπως σχόλια. Πρέπει να υλοποιηθεί από την κλάση DocumentFormatInstance./documentformatinstancederived για την εκτέλεση επεμβάσεων σημειώσεων."
type: docs
weight: 120
url: /el/net/groupdocs.redaction.integration/iannotateddocument/
---
## IAnnotatedDocument interface

Ορίζει μεθόδους που απαιτούνται για πρόσβαση σε σημειώσεις, όπως σχόλια. Πρέπει να υλοποιηθεί από την κλάση [`DocumentFormatInstance`](../documentformatinstance)-derived για την εκτέλεση επεμβάσεων σημειώσεων.

```csharp
public interface IAnnotatedDocument
```

## Μέθοδοι

| Όνομα | Περιγραφή |
| --- | --- |
| [DeleteAnnotations](../../groupdocs.redaction.integration/iannotateddocument/deleteannotations)(Regex) | Διαγράφει όλες τις σημειώσεις που ταιριάζουν με κανονική έκφραση μέσα στο έγγραφο. |
| [RedactAnnotation](../../groupdocs.redaction.integration/iannotateddocument/redactannotation)(Regex, string) | Αντικαθιστά το ταιριαστό κείμενο σε όλες τις σημειώσεις μέσα στο έγγραφο. |

### Παρατηρήσεις

**Learn more**

* More details about applying redactions: [Redaction basics](https://docs.groupdocs.com/redaction/net/redaction-basics/)
* More details about document annotation redactions: [Annotation redactions](https://docs.groupdocs.com/redaction/net/annotation-redactions/)
* More details about implementing custom formats: [Create custom format handler](https://docs.groupdocs.com/redaction/net/create-custom-format-handler/)

### Δείτε επίσης

* namespace [GroupDocs.Redaction.Integration](../../groupdocs.redaction.integration)
* assembly [GroupDocs.Redaction](../../)

<!-- ΜΗΝ ΕΠΕΞΕΡΓΑΣΕΤΕ: δημιουργήθηκε από το xmldocmd για το GroupDocs.Redaction.dll -->
