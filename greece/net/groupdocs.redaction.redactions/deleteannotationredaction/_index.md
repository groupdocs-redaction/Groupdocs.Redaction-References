---
title: "DeleteAnnotationRedaction"
second_title: "GroupDocs.Redaction για .NET API Reference"
description: "Αντιπροσωπεύει μια διαγραφή κειμένου που διαγράφει τις σημειώσεις εάν το κείμενο ταιριάζει με την δεδομένη κανονική έκφραση, προαιρετικά διαγράφει όλες τις σημειώσεις."
type: docs
weight: 580
url: /el/net/groupdocs.redaction.redactions/deleteannotationredaction/
---
## DeleteAnnotationRedaction class

Αντιπροσωπεύει μια κειμενική απόκρυψη που διαγράφει τα σχόλια εάν το κείμενο ταιριάζει με τη δεδομένη κανονική έκφραση (προαιρετικά διαγράφει όλα τα σχόλια).

```csharp
public class DeleteAnnotationRedaction : Redaction
```

## Κατασκευαστές

| Όνομα | Περιγραφή |
| --- | --- |
| [DeleteAnnotationRedaction](deleteannotationredaction#constructor)() | Αρχικοποιεί ένα νέο αντικείμενο της κλάσης DeleteAnnotationRedaction, με ρυθμίσεις για διαγραφή όλων των σημειώσεων (που ταιριάζουν με όλα). |
| [DeleteAnnotationRedaction](deleteannotationredaction#constructor_2)(Regex) | Αρχικοποιεί ένα νέο αντικείμενο της κλάσης DeleteAnnotationRedaction, διαγράφοντας τις σημειώσεις που ταιριάζουν με τη δεδομένη έκφραση. |
| [DeleteAnnotationRedaction](deleteannotationredaction#constructor_1)(string) | Αρχικοποιεί ένα νέο αντικείμενο της κλάσης DeleteAnnotationRedaction, διαγράφοντας τις σημειώσεις που ταιριάζουν με τη δεδομένη έκφραση. |

## Ιδιότητες

| Όνομα | Περιγραφή |
| --- | --- |
| override [Description](../../groupdocs.redaction.redactions/deleteannotationredaction/description) { get; } | Επιστρέφει μια συμβολοσειρά που περιγράφει το Redaction και τις παραμέτρους του. |
| [Expression](../../groupdocs.redaction.redactions/deleteannotationredaction/expression) { get; } | Λαμβάνει την κανονική έκφραση για αντιστοίχιση. |

## Μέθοδοι

| Όνομα | Περιγραφή |
| --- | --- |
| override [ApplyTo](../../groupdocs.redaction.redactions/deleteannotationredaction/applyto)(DocumentFormatInstance) | Εφαρμόζει το Redaction σε ένα δεδομένο αντικείμενο μορφής. |

### Παρατηρήσεις

**Learn more**

* More details about applying redactions: [Redaction basics](https://docs.groupdocs.com/redaction/net/redaction-basics/)
* More details about document annotation redactions: [Annotation redactions](https://docs.groupdocs.com/redaction/net/annotation-redactions/)

### Παραδείγματα

Το παρακάτω παράδειγμα δείχνει πώς να αφαιρέσετε όλες τις σημειώσεις που περιέχουν τις λέξεις "use", "show" ή "describe" από το έγγραφο (και να αφήσετε τις άλλες).

```csharp
using (Redactor redactor = new Redactor(@"D:\test.docx"))
{
   redactor.Apply(new DeleteAnnotationRedaction("(?im:(use|show|describe))"));
   redactor.Save()
}
```

### Δείτε επίσης

* class [Redaction](../../groupdocs.redaction/redaction)
* namespace [GroupDocs.Redaction.Redactions](../../groupdocs.redaction.redactions)
* assembly [GroupDocs.Redaction](../../)

<!-- ΜΗΝ ΕΠΕΞΕΡΓΑΣΕΤΕ: δημιουργήθηκε από το xmldocmd για το GroupDocs.Redaction.dll -->
