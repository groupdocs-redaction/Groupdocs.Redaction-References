---
title: "AdvancedRasterizationOptions"
second_title: "GroupDocs.Redaction για .NET API Reference"
description: "Απαρίθμηση σημαίας για τη διαχείριση των προχωρημένων επιλογών rasterization που θα εφαρμοστούν."
type: docs
weight: 290
url: /el/net/groupdocs.redaction.options/advancedrasterizationoptions/
---
## AdvancedRasterizationOptions enumeration

Απαρίθμηση σημαίας για τη διαχείριση των προχωρημένων επιλογών rasterization που θα εφαρμοστούν.

```csharp
public enum AdvancedRasterizationOptions
```

### Τιμές

| Όνομα | Τιμή | Περιγραφή |
| --- | --- | --- |
| None | `0` | Δεν υπάρχουν προχωρημένες επιλογές προς εφαρμογή. |
| Tilt | `1` | Κλίση για να κλίνετε την αποδοθείσα εικόνα σε τυχαία γωνία. |
| Noise | `2` | Προσθέστε τυχαίες κηλίδες στις αποδοθείσες εικόνες σελίδων. |
| Border | `4` | Προσθέστε γραμμή περιγράμματος για να μιμηθεί το εφέ σάρωσης σελίδας. |
| Grayscale | `8` | Κάντε τις εικόνες σελίδων σε αποχρώσεις του γκρι για να μιμηθεί σάρωση σε γκρι κλίμακα. |

### Παραδείγματα

Το παρακάτω παράδειγμα δείχνει πώς να εφαρμόσετε τις προχωρημένες επιλογές απόδοσης με τις προεπιλεγμένες ρυθμίσεις.

```csharp
    using (Redactor redactor = new Redactor(@"C:\sample.docx"))
    {
      // Αποθηκεύστε το έγγραφο με τις προεπιλεγμένες επιλογές (μετατροπή σελίδων σε εικόνες, αποθήκευση ως PDF)
      var so = new SaveOptions();
      so.Rasterization.Enabled = true;
      so.RedactedFileSuffix = "_scan";
      so.Rasterization.AddAdvancedOption(AdvancedRasterizationOptions.Border);
      so.Rasterization.AddAdvancedOption(AdvancedRasterizationOptions.Noise);
      so.Rasterization.AddAdvancedOption(AdvancedRasterizationOptions.Grayscale);
      so.Rasterization.AddAdvancedOption(AdvancedRasterizationOptions.Tilt);
      redactor.Save(so);
    }
```

Το παρακάτω παράδειγμα δείχνει πώς να εφαρμόσετε την προχωρημένη επιλογή περιγράμματος απόδοσης με προσαρμοσμένες ρυθμίσεις.

```csharp
    using (Redactor redactor = new Redactor(@"C:\sample.docx"))
    {
      // Αποθηκεύστε το έγγραφο με προσαρμοσμένο περίγραμμα
      var so = new SaveOptions();
      so.Rasterization.Enabled = true;
      so.RedactedFileSuffix = "_scan";
      so.Rasterization.AddAdvancedOption(AdvancedRasterizationOptions.Border, new Dictionary<string, string>() { { "border", "10" } });
      redactor.Save(so);
    }
```

Το παρακάτω παράδειγμα δείχνει πώς να εφαρμόσετε την προχωρημένη επιλογή θορύβου απόδοσης με προσαρμοσμένες ρυθμίσεις.

```csharp
    using (Redactor redactor = new Redactor(@"C:\sample.docx"))
    {
      // Αποθηκεύστε το έγγραφο με τον προσαρμοσμένο αριθμό και μέγεθος των εφέ θορύβου
      var so = new SaveOptions();
      so.Rasterization.Enabled = true;
      so.RedactedFileSuffix = "_scan";
      so.Rasterization.AddAdvancedOption(AdvancedRasterizationOptions.Noise, 
          new Dictionary<string, string>() { { "maxSpots", "150" }, { "spotMaxSize", "15" } });
      redactor.Save(so);
    }
```

Το παρακάτω παράδειγμα δείχνει πώς να εφαρμόσετε την προχωρημένη επιλογή rasterization κλίσης με προσαρμοσμένες ρυθμίσεις.

```csharp
    using (Redactor redactor = new Redactor(@"C:\sample.docx"))
    {
      // Αποθηκεύστε το έγγραφο με το προσαρμοσμένο εφέ κλίσης
      var so = new SaveOptions();
      so.Rasterization.Enabled = true;
      so.RedactedFileSuffix = "_scan";
      so.Rasterization.AddAdvancedOption(AdvancedRasterizationOptions.Tilt, 
          new Dictionary<string, string>() { { { "minAngle", "85" }, { "randomAngleMax", "5" } });
      redactor.Save(so);
    }
```

### Δείτε επίσης

* namespace [GroupDocs.Redaction.Options](../../groupdocs.redaction.options)
* assembly [GroupDocs.Redaction](../../)

<!-- ΜΗΝ ΕΠΕΞΕΡΓΑΣΕΤΕ: δημιουργήθηκε από το xmldocmd για το GroupDocs.Redaction.dll -->
