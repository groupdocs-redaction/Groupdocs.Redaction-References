---
title: "AnnotationRedaction"
second_title: "GroupDocs.Redaction για .NET API Reference"
description: "Αντιπροσωπεύει μια διαγραφή που αντικαθιστά κείμενο σχολίων κ.λπ. που ταιριάζει με μια δεδομένη κανονική έκφραση."
type: docs
weight: 530
url: /el/net/groupdocs.redaction.redactions/annotationredaction/
---
## AnnotationRedaction class

Αντιπροσωπεύει μια απόκρυψη που αντικαθιστά το κείμενο σχολίων (σχόλια, κ.λπ.) που ταιριάζει με μια δεδομένη κανονική έκφραση.

```csharp
public class AnnotationRedaction : Redaction
```

## Κατασκευαστές

| Όνομα | Περιγραφή |
| --- | --- |
| [AnnotationRedaction](annotationredaction#constructor_1)(Regex, string) | Αρχικοποιεί μια νέα παρουσία της κλάσης AnnotationRedaction. |
| [AnnotationRedaction](annotationredaction#constructor)(string, string) | Αρχικοποιεί μια νέα παρουσία της κλάσης AnnotationRedaction. |

## Ιδιότητες

| Όνομα | Περιγραφή |
| --- | --- |
| override [Description](../../groupdocs.redaction.redactions/annotationredaction/description) { get; } | Επιστρέφει μια συμβολοσειρά που περιγράφει το Redaction και τις παραμέτρους του. |
| [Expression](../../groupdocs.redaction.redactions/annotationredaction/expression) { get; } | Λαμβάνει την κανονική έκφραση για αντιστοίχιση. |
| [Replacement](../../groupdocs.redaction.redactions/annotationredaction/replacement) { get; } | Λαμβάνει μια κειμενική αντικατάσταση για το ταιριασμένο κείμενο. |

## Μέθοδοι

| Όνομα | Περιγραφή |
| --- | --- |
| override [ApplyTo](../../groupdocs.redaction.redactions/annotationredaction/applyto)(DocumentFormatInstance) | Εφαρμόζει το Redaction σε ένα δεδομένο αντικείμενο μορφής. |

### Παρατηρήσεις

**Learn more**

* More details about applying redactions: [Redaction basics](https://docs.groupdocs.com/redaction/net/redaction-basics/)
* More details about document annotation redactions: [Annotation redactions](https://docs.groupdocs.com/redaction/net/annotation-redactions/)

### Παραδείγματα

Το παρακάτω παράδειγμα δείχνει πώς να αντικαταστήσετε το όνομα "John" με "[redacted]" σε όλες τις annotations.

```csharp
using (Redactor redactor = new Redactor(@"C:\test.pdf"))
{
   redactor.Apply(new AnnotationRedaction("(?im:john)", "[redacted]"));
   redactor.Save()
}
```

### Δείτε επίσης

* class [Redaction](../../groupdocs.redaction/redaction)
* namespace [GroupDocs.Redaction.Redactions](../../groupdocs.redaction.redactions)
* assembly [GroupDocs.Redaction](../../)

<!-- ΜΗΝ ΕΠΕΞΕΡΓΑΣΕΤΕ: δημιουργήθηκε από το xmldocmd για το GroupDocs.Redaction.dll -->
