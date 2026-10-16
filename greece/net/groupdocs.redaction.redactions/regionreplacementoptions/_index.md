---
title: "RegionReplacementOptions"
second_title: "GroupDocs.Redaction για .NET API Reference"
description: "Αντιπροσωπεύει τις παραμέτρους χρώματος και περιοχής για αντικατάσταση περιοχής εικόνας. Δείτε το ImageAreaRedaction./imagearearedaction."
type: docs
weight: 760
url: /el/net/groupdocs.redaction.redactions/regionreplacementoptions/
---
## RegionReplacementOptions class

Αντιπροσωπεύει τις παραμέτρους χρώματος και περιοχής για αντικατάσταση περιοχής εικόνας. Δείτε [`ImageAreaRedaction`](../imagearearedaction).

```csharp
public class RegionReplacementOptions
```

## Κατασκευαστές

| Όνομα | Περιγραφή |
| --- | --- |
| [RegionReplacementOptions](regionreplacementoptions#constructor_1)(Color, Size) | Αρχικοποιεί μια νέα παρουσία της κλάσης RegionReplacementOptions. |
| [RegionReplacementOptions](regionreplacementoptions#constructor)(Color, Font, string) | Αρχικοποιεί μια νέα παρουσία της κλάσης RegionReplacementOptions της οποίας το μέγεθος ταιριάζει με το δοσμένο κείμενο. |

## Ιδιότητες

| Όνομα | Περιγραφή |
| --- | --- |
| [FillColor](../../groupdocs.redaction.redactions/regionreplacementoptions/fillcolor) { get; set; } | Αποκτά ή ορίζει το χρώμα για γέμισμα της διαγραμμένης περιοχής. |
| [Size](../../groupdocs.redaction.redactions/regionreplacementoptions/size) { get; set; } | Αποκτά ή ορίζει το ορθογώνιο με πλάτος και ύψος. |

### Παρατηρήσεις

**Learn more**

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

* namespace [GroupDocs.Redaction.Redactions](../../groupdocs.redaction.redactions)
* assembly [GroupDocs.Redaction](../../)

<!-- ΜΗΝ ΕΠΕΞΕΡΓΑΣΕΤΕ: δημιουργήθηκε από το xmldocmd για το GroupDocs.Redaction.dll -->
