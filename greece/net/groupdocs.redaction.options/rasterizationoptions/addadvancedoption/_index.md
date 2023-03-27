---
title: AddAdvancedOption
second_title: GroupDocs.Redaction για Αναφορά API .NET
description: Μπορείτε να χρησιμοποιήσετε αυτήν τη μέθοδο για να καταχωρίσετε μια προηγμένη επιλογή ραστεροποίησης για εφαρμογή.
type: docs
weight: 70
url: /el/net/groupdocs.redaction.options/rasterizationoptions/addadvancedoption/
---
## AddAdvancedOption(AdvancedRasterizationOptions) {#addadvancedoption}

Μπορείτε να χρησιμοποιήσετε αυτήν τη μέθοδο για να καταχωρίσετε μια προηγμένη επιλογή ραστεροποίησης για εφαρμογή.

```csharp
public void AddAdvancedOption(AdvancedRasterizationOptions optionType)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| optionType | AdvancedRasterizationOptions | Παρέχει πληροφορίες σχετικά με τον επιλεγμένο τύπο εφέ (κλίμακα του γκρι, περίγραμμα κ.λπ.) |

### Παραδείγματα

Το ακόλουθο παράδειγμα δείχνει πώς να εφαρμόσετε τις προηγμένες επιλογές ραστεροποίησης με προεπιλεγμένες ρυθμίσεις.

```csharp
    using (Redactor redactor = new Redactor(@"C:\sample.docx"))
    {
      // Αποθήκευση του εγγράφου με προεπιλεγμένες επιλογές (μετατροπή σελίδων σε εικόνες, αποθήκευση ως PDF)
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
* χώρος ονομάτων [GroupDocs.Redaction.Options](../../rasterizationoptions)
* συνέλευση [GroupDocs.Redaction](../../../)

---

## AddAdvancedOption(AdvancedRasterizationOptions, Dictionary&lt;string, string&gt;) {#addadvancedoption_1}

Μπορείτε να χρησιμοποιήσετε αυτήν τη μέθοδο για να καταχωρίσετε μια προηγμένη επιλογή ραστεροποίησης για εφαρμογή.

```csharp
public void AddAdvancedOption(AdvancedRasterizationOptions optionType, 
    Dictionary<string, string> parameters)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| optionType | AdvancedRasterizationOptions | Παρέχει πληροφορίες σχετικά με τον επιλεγμένο τύπο εφέ (κλίμακα του γκρι, περίγραμμα κ.λπ.) |
| parameters | Dictionary`2 | Παράμετροι για το δεδομένο εφέ, όπως η γωνία περιστροφής |

### Παραδείγματα

Το ακόλουθο παράδειγμα δείχνει πώς να εφαρμόσετε τις προηγμένες επιλογές ραστεροποίησης με προεπιλεγμένες ρυθμίσεις.

```csharp
    using (Redactor redactor = new Redactor(@"C:\sample.docx"))
    {
      // Αποθήκευση του εγγράφου με προεπιλεγμένες επιλογές (μετατροπή σελίδων σε εικόνες, αποθήκευση ως PDF)
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

Το ακόλουθο παράδειγμα δείχνει πώς να εφαρμόσετε την επιλογή προηγμένης ραστεροποίησης περιγράμματος με προσαρμοσμένες ρυθμίσεις.

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

Το ακόλουθο παράδειγμα δείχνει πώς να εφαρμόσετε την επιλογή ραστεροποίησης για προχωρημένους θορύβου με προσαρμοσμένες ρυθμίσεις.

```csharp
    using (Redactor redactor = new Redactor(@"C:\sample.docx"))
    {
      // Αποθηκεύστε το έγγραφο με τον προσαρμοσμένο αριθμό και το μέγεθος των εφέ θορύβου
      var so = new SaveOptions();
      so.Rasterization.Enabled = true;
      so.RedactedFileSuffix = "_scan";
      so.Rasterization.AddAdvancedOption(AdvancedRasterizationOptions.Noise, 
          new Dictionary<string, string>() { { "maxSpots", "150" }, { "spotMaxSize", "15" } });
      redactor.Save(so);
    }
```

Το ακόλουθο παράδειγμα δείχνει πώς να εφαρμόσετε την επιλογή σύνθετης ραστεροποίησης κλίσης με προσαρμοσμένες ρυθμίσεις.

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
* χώρος ονομάτων [GroupDocs.Redaction.Options](../../rasterizationoptions)
* συνέλευση [GroupDocs.Redaction](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Redaction.dll -->
