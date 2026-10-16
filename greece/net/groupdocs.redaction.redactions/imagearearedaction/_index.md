---
title: "ImageAreaRedaction"
second_title: "GroupDocs.Redaction για .NET API Reference"
description: "Αντιπροσωπεύει μια διαγραφή που τοποθετεί χρωματιστό ορθογώνιο στην καθορισμένη περιοχή ενός εγγράφου εικόνας."
type: docs
weight: 630
url: /el/net/groupdocs.redaction.redactions/imagearearedaction/
---
## ImageAreaRedaction class

Αντιπροσωπεύει μια διαγραφή που τοποθετεί χρωματιστό ορθογώνιο στην καθορισμένη περιοχή ενός εγγράφου εικόνας.

```csharp
public class ImageAreaRedaction : Redaction
```

## Κατασκευαστές

| Όνομα | Περιγραφή |
| --- | --- |
| [ImageAreaRedaction](imagearearedaction)(Point, RegionReplacementOptions) | Αρχικοποιεί μια νέα παρουσία της κλάσης ImageAreaRedaction για τη διαγραφή συγκεκριμένου μεγέθους περιοχής. |

## Ιδιότητες

| Όνομα | Περιγραφή |
| --- | --- |
| override [Description](../../groupdocs.redaction.redactions/imagearearedaction/description) { get; } | Επιστρέφει μια συμβολοσειρά που περιγράφει το Redaction και τις παραμέτρους του. |
| [Options](../../groupdocs.redaction.redactions/imagearearedaction/options) { get; } | Λαμβάνει τις επιλογές [`RegionReplacementOptions`](../regionreplacementoptions) με χρώμα και παραμέτρους περιοχής. |
| [TopLeft](../../groupdocs.redaction.redactions/imagearearedaction/topleft) { get; } | Λαμβάνει τη θέση πάνω‑αριστερά της περιοχής που θα αφαιρεθεί. |

## Μέθοδοι

| Όνομα | Περιγραφή |
| --- | --- |
| override [ApplyTo](../../groupdocs.redaction.redactions/imagearearedaction/applyto)(DocumentFormatInstance) | Εφαρμόζει το Redaction σε ένα δεδομένο αντικείμενο μορφής. |

### Παρατηρήσεις

**Learn more**

* More details about applying redactions: [Redaction basics](https://docs.groupdocs.com/redaction/net/redaction-basics/)
* More details about image redactions: [Image redactions](https://docs.groupdocs.com/redaction/net/image-redactions/)

### Παραδείγματα

Το παρακάτω παράδειγμα δείχνει την αντικατάσταση μιας περιοχής μέσα στην εικόνα με ένα στερεό χρωματικό ορθογώνιο.

```csharp
    using (Redactor redactor = new Redactor("D:\\test.jpg"))
    {
       GroupDocs.Redaction.Options.Drawing.Point samplePoint = new GroupDocs.Redaction.Options.Drawing.Point(516, 311);
       GroupDocs.Redaction.Options.Drawing.Size sampleSize = new GroupDocs.Redaction.Options.Drawing.Size(170, 35);
       RedactorChangeLog result = redactor.Apply(new ImageAreaRedaction(samplePoint,
                     new RegionReplacementOptions(GroupDocs.Redaction.Options.Drawing.Color.Blue, sampleSize)));
       if (result.Status != RedactionStatus.Failed)
       {
          redactor.Save();
       };
    } 
```

### Δείτε επίσης

* class [Redaction](../../groupdocs.redaction/redaction)
* namespace [GroupDocs.Redaction.Redactions](../../groupdocs.redaction.redactions)
* assembly [GroupDocs.Redaction](../../)

<!-- ΜΗΝ ΕΠΕΞΕΡΓΑΣΕΤΕ: δημιουργήθηκε από το xmldocmd για το GroupDocs.Redaction.dll -->
