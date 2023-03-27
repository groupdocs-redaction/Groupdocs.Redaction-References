---
title: RasterizationOptions
second_title: GroupDocs.Redaction για Αναφορά API .NET
description: Παρέχει επιλογές για τη μετατροπή αρχείων σε PDF.
type: docs
weight: 350
url: /el/net/groupdocs.redaction.options/rasterizationoptions/
---
## RasterizationOptions class

Παρέχει επιλογές για τη μετατροπή αρχείων σε PDF.

```csharp
public class RasterizationOptions
```

## Κατασκευαστές

| Ονομα | Περιγραφή |
| --- | --- |
| [RasterizationOptions](rasterizationoptions)() | Αρχικοποιεί μια νέα παρουσία. |

## Ιδιότητες

| Ονομα | Περιγραφή |
| --- | --- |
| [Compliance](../../groupdocs.redaction.options/rasterizationoptions/compliance) { get; set; } | Λαμβάνει ή ορίζει το επίπεδο συμμόρφωσης PDF. |
| [Enabled](../../groupdocs.redaction.options/rasterizationoptions/enabled) { get; set; } | Λαμβάνει ή ορίζει μια τιμή που υποδεικνύει εάν όλες οι σελίδες του εγγράφου πρέπει να μετατραπούν σε εικόνες και να τοποθετηθούν σε ένα μόνο αρχείο PDF. TRUE από προεπιλογή, ορίστε το FALSE για να αποφευχθεί η ραστεροποίηση. |
| [HasAdvancedOptions](../../groupdocs.redaction.options/rasterizationoptions/hasadvancedoptions) { get; } | Λαμβάνει μια ένδειξη, η οποία ισχύει εάν έχουν οριστεί προηγμένες επιλογές ραστεροποίησης. |
| [PageCount](../../groupdocs.redaction.options/rasterizationoptions/pagecount) { get; set; } | Λαμβάνει ή ορίζει τον αριθμό των σελίδων που θα μετατραπούν σε PDF. |
| [PageIndex](../../groupdocs.redaction.options/rasterizationoptions/pageindex) { get; set; } | Λαμβάνει ή ορίζει το ευρετήριο της πρώτης σελίδας (με βάση το 0) για μετατροπή σε PDF. |

## Μέθοδοι

| Ονομα | Περιγραφή |
| --- | --- |
| [AddAdvancedOption](../../groupdocs.redaction.options/rasterizationoptions/addadvancedoption#addadvancedoption)(AdvancedRasterizationOptions) | Μπορείτε να χρησιμοποιήσετε αυτήν τη μέθοδο για να καταχωρίσετε μια προηγμένη επιλογή ραστεροποίησης για εφαρμογή. |
| [AddAdvancedOption](../../groupdocs.redaction.options/rasterizationoptions/addadvancedoption#addadvancedoption_1)(AdvancedRasterizationOptions, Dictionary&lt;string, string&gt;) | Μπορείτε να χρησιμοποιήσετε αυτήν τη μέθοδο για να καταχωρίσετε μια προηγμένη επιλογή ραστεροποίησης για εφαρμογή. |

### Παρατηρήσεις

**Μάθε περισσότερα**

* Περισσότερες λεπτομέρειες σχετικά με την αποθήκευση εγγράφου ως ραστεροποιημένο PDF: [Αποθήκευση σε ραστεροποιημένο PDF](https://docs.groupdocs.com/redaction/net/save-in-rasterized-pdf/)
* Περισσότερες λεπτομέρειες σχετικά με τις επιλογές ραστεροποίησης: [Επιλέξτε συγκεκριμένες σελίδες για ραστεροποιημένο PDF](https://docs.groupdocs.com/redaction/net/select-specific-pages-for-rasterized-pdf/)

### Παραδείγματα

Το ακόλουθο παράδειγμα δείχνει πώς να ορίσετε επιλογές για τη διαδικασία ραστεροποίησης.

```csharp
    using (var redactor = new Redactor("SomePresentation.pptx"))
    {
        // διόρθωση ευαίσθητων δεδομένων στην πρώτη διαφάνεια 
    
        var rasterizationOptions = new RasterizationOptions();
        rasterizationOptions.PageIndex = 0;
        rasterizationOptions.PageCount = 1;
        rasterizationOptions.Compliance = PdfComplianceLevel.PdfA1a;
        using (var stream = File.Open(Path.Combine(@"C:\Temp", "PresentationFirstSlide.pdf")))
        {
            redactor.Save(stream, rasterizationOptions);
        }
    }      
```

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

* χώρος ονομάτων [GroupDocs.Redaction.Options](../../groupdocs.redaction.options)
* συνέλευση [GroupDocs.Redaction](../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Redaction.dll -->
