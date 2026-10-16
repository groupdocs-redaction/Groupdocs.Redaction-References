---
title: "RasterizationOptions"
second_title: "GroupDocs.Redaction για .NET API Reference"
description: "Παρέχει επιλογές για τη μετατροπή αρχείων σε PDF."
type: docs
weight: 420
url: /el/net/groupdocs.redaction.options/rasterizationoptions/
---
## RasterizationOptions class

Παρέχει επιλογές για τη μετατροπή αρχείων σε PDF.

```csharp
public class RasterizationOptions
```

## Κατασκευαστές

| Όνομα | Περιγραφή |
| --- | --- |
| [RasterizationOptions](rasterizationoptions)() | Αρχικοποιεί μια νέα παρουσία. |

## Ιδιότητες

| Όνομα | Περιγραφή |
| --- | --- |
| [Compliance](../../groupdocs.redaction.options/rasterizationoptions/compliance) { get; set; } | Λαμβάνει ή ορίζει το επίπεδο Συμμόρφωσης PDF. |
| [Enabled](../../groupdocs.redaction.options/rasterizationoptions/enabled) { get; set; } | Λαμβάνει ή ορίζει μια τιμή που υποδεικνύει εάν όλες οι σελίδες του εγγράφου πρέπει να μετατραπούν σε εικόνες και να τοποθετηθούν σε ένα ενιαίο αρχείο PDF. TRUE by default, set to FALSE in order to avoid rasterization. |
| [HasAdvancedOptions](../../groupdocs.redaction.options/rasterizationoptions/hasadvancedoptions) { get; } | Λαμβάνει έναν δείκτη, ο οποίος είναι true εάν έχουν οριστεί προχωρημένες επιλογές αποτύπωσης. |
| [PageCount](../../groupdocs.redaction.options/rasterizationoptions/pagecount) { get; set; } | Λαμβάνει ή ορίζει τον αριθμό των σελίδων που θα μετατραπούν σε PDF. |
| [PageIndex](../../groupdocs.redaction.options/rasterizationoptions/pageindex) { get; set; } | Λαμβάνει ή ορίζει το δείκτη της πρώτης σελίδας (0-based) που θα μετατραπεί σε PDF. |

## Μέθοδοι

| Όνομα | Περιγραφή |
| --- | --- |
| [AddAdvancedOption](../../groupdocs.redaction.options/rasterizationoptions/addadvancedoption#addadvancedoption)(AdvancedRasterizationOptions) | Μπορείτε να χρησιμοποιήσετε αυτή τη μέθοδο για να καταχωρήσετε μια προχωρημένη επιλογή αποτύπωσης προς εφαρμογή. |
| [AddAdvancedOption](../../groupdocs.redaction.options/rasterizationoptions/addadvancedoption#addadvancedoption_1)(AdvancedRasterizationOptions, Dictionary&lt;string, string&gt;) | Μπορείτε να χρησιμοποιήσετε αυτή τη μέθοδο για να καταχωρήσετε μια προχωρημένη επιλογή αποτύπωσης προς εφαρμογή. |

### Παρατηρήσεις

**Learn more**

* More details about saving document as a rasterized PDF: [Save in rasterized PDF](https://docs.groupdocs.com/redaction/net/save-in-rasterized-pdf/)
* More details about rasterization options: [Select specific pages for rasterized PDF](https://docs.groupdocs.com/redaction/net/select-specific-pages-for-rasterized-pdf/)

### Παραδείγματα

Το παρακάτω παράδειγμα δείχνει πώς να ορίσετε επιλογές για τη διαδικασία αποτύπωσης.

```csharp
    using (var redactor = new Redactor("SomePresentation.pptx"))
    {
        // αποκρύψτε ευαίσθητα δεδομένα στην πρώτη διαφάνεια 
    
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
