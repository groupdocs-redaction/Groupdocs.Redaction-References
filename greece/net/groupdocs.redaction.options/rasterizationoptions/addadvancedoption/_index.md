---
title: "AddAdvancedOption"
second_title: "GroupDocs.Redaction για .NET API Reference"
description: "Μπορείτε να χρησιμοποιήσετε αυτή τη μέθοδο για να καταχωρήσετε μια προχωρημένη επιλογή αποτύπωσης προς εφαρμογή."
type: docs
weight: 70
url: /el/net/groupdocs.redaction.options/rasterizationoptions/addadvancedoption/
---
## AddAdvancedOption(AdvancedRasterizationOptions) {#addadvancedoption}

Μπορείτε να χρησιμοποιήσετε αυτή τη μέθοδο για να καταχωρήσετε μια προχωρημένη επιλογή αποτύπωσης προς εφαρμογή.

```csharp
public void AddAdvancedOption(AdvancedRasterizationOptions optionType)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| optionType | AdvancedRasterizationOptions | Παρέχει πληροφορίες σχετικά με τον επιλεγμένο τύπο εφέ (γκρι κλίμακα, περίγραμμα κ.λπ.) |

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

### Δείτε επίσης

* enum [AdvancedRasterizationOptions](../../advancedrasterizationoptions)
* class [RasterizationOptions](../../rasterizationoptions)
* namespace [GroupDocs.Redaction.Options](../../../groupdocs.redaction.options)
* assembly [GroupDocs.Redaction](../../../)

---

## AddAdvancedOption(AdvancedRasterizationOptions, Dictionary&lt;string, string&gt;) {#addadvancedoption_1}

Μπορείτε να χρησιμοποιήσετε αυτή τη μέθοδο για να καταχωρήσετε μια προχωρημένη επιλογή αποτύπωσης προς εφαρμογή.

```csharp
public void AddAdvancedOption(AdvancedRasterizationOptions optionType, 
    Dictionary<string, string> parameters)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| optionType | AdvancedRasterizationOptions | Παρέχει πληροφορίες σχετικά με τον επιλεγμένο τύπο εφέ (γκρι κλίμακα, περίγραμμα κ.λπ.) |
| parameters | Dictionary`2 | Παράμετροι για το συγκεκριμένο εφέ, όπως η γωνία περιστροφής |

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

* enum [AdvancedRasterizationOptions](../../advancedrasterizationoptions)
* class [RasterizationOptions](../../rasterizationoptions)
* namespace [GroupDocs.Redaction.Options](../../../groupdocs.redaction.options)
* assembly [GroupDocs.Redaction](../../../)

<!-- ΜΗΝ ΕΠΕΞΕΡΓΑΣΕΤΕ: δημιουργήθηκε από το xmldocmd για το GroupDocs.Redaction.dll -->
