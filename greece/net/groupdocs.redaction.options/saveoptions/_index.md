---
title: "SaveOptions"
second_title: "GroupDocs.Redaction για .NET API Reference"
description: "Παρέχει επιλογές για την αλλαγή του ονόματος του αρχείου εξόδου και/ή τη μετατροπή του εγγράφου σε rasterization PDF βασισμένο σε εικόνα."
type: docs
weight: 450
url: /el/net/groupdocs.redaction.options/saveoptions/
---
## SaveOptions class

Παρέχει επιλογές για την αλλαγή του ονόματος του αρχείου εξόδου και/ή τη μετατροπή του εγγράφου σε PDF βασισμένο σε εικόνα (rasterization).

```csharp
public class SaveOptions
```

## Κατασκευαστές

| Όνομα | Περιγραφή |
| --- | --- |
| [SaveOptions](saveoptions#constructor)() | Αρχικοποιεί μια νέα παρουσία με προεπιλογές: rasterize to PDF - false, add suffix - false. |
| [SaveOptions](saveoptions#constructor_1)(bool, string) | Αρχικοποιεί μια νέα παρουσία με δοσμένες παραμέτρους. |

## Ιδιότητες

| Όνομα | Περιγραφή |
| --- | --- |
| [AddSuffix](../../groupdocs.redaction.options/saveoptions/addsuffix) { get; set; } | Λαμβάνει ή ορίζει μια τιμή που υποδεικνύει εάν το όνομα αρχείου πρέπει να αλλάξει πριν από την αποθήκευση. False από προεπιλογή. |
| [Rasterization](../../groupdocs.redaction.options/saveoptions/rasterization) { get; } | Λαμβάνει τις ρυθμίσεις rasterization. |
| [RasterizeToPDF](../../groupdocs.redaction.options/saveoptions/rasterizetopdf) { get; set; } | Λαμβάνει ή ορίζει μια τιμή που υποδεικνύει εάν όλες οι σελίδες του εγγράφου πρέπει να μετατραπούν σε εικόνες και να τοποθετηθούν σε ένα ενιαίο αρχείο PDF. |
| [RedactedFileSuffix](../../groupdocs.redaction.options/saveoptions/redactedfilesuffix) { get; set; } | Λαμβάνει ή ορίζει μια προσαρμοσμένη κατάληξη για το όνομα αρχείου εξόδου. Εάν δεν καθοριστεί, η [`SaveSuffix`](./savesuffix) σταθερά θα χρησιμοποιηθεί. |
| [WordprocessingSaveOptions](../../groupdocs.redaction.options/saveoptions/wordprocessingsaveoptions) { get; } | Λαμβάνει τις επιλογές αποθήκευσης ειδικές για έγγραφα επεξεργασίας κειμένου. |

## Πεδία

| Όνομα | Περιγραφή |
| --- | --- |
| const [SaveSuffix](../../groupdocs.redaction.options/saveoptions/savesuffix) | Αντιπροσωπεύει την προεπιλεγμένη τιμή κατάληξης, η οποία είναι "Redacted". |

### Παρατηρήσεις

**Learn more**

* [Save with default options](https://docs.groupdocs.com/redaction/net/save-with-default-options/)
* [Save in rasterized PDF](https://docs.groupdocs.com/redaction/net/save-in-rasterized-pdf/)
* [Select specific pages for rasterized PDF](https://docs.groupdocs.com/redaction/net/select-specific-pages-for-rasterized-pdf/)
* [Save in original format](https://docs.groupdocs.com/redaction/net/save-in-original-format/)
* [Save overwriting original file](https://docs.groupdocs.com/redaction/net/save-overwriting-original-file/)
* [Save to stream](https://docs.groupdocs.com/redaction/net/save-to-stream/)

### Παραδείγματα

Το παρακάτω παράδειγμα δείχνει πώς να αποθηκεύσετε ένα έγγραφο χρησιμοποιώντας το SaveOptions.

```csharp
    using (Redactor redactor = new Redactor(@"C:\sample.pdf"))
    {
       // Η διαγραφή εγγράφου πηγαίνει εδώ
       // ...
    
       // Αποθηκεύστε το έγγραφο με τις προεπιλεγμένες επιλογές (μετατροπή σελίδων σε εικόνες, αποθήκευση ως PDF)
       redactor.Save();
    
       // Αποθηκεύστε το έγγραφο στην αρχική μορφή αντικαθιστώντας το αρχικό αρχείο
       redactor.Save(new SaveOptions() { AddSuffix = false, RasterizeToPDF = false });
    
       // Αποθηκεύστε το έγγραφο σε αρχείο "*_Redacted.*" στην αρχική μορφή
       redactor.Save(new SaveOptions() { AddSuffix = true, RasterizeToPDF = false });
    
       // Αποθηκεύστε το έγγραφο σε "*_AnyText.*" (π.χ. χρονική σήμανση αντί για "AnyText") στο όνομα αρχείου του χωρίς rasterization
       redactor.Save(new SaveOptions(false, "AnyText"));
    }    
```

### Δείτε επίσης

* namespace [GroupDocs.Redaction.Options](../../groupdocs.redaction.options)
* assembly [GroupDocs.Redaction](../../)

<!-- ΜΗΝ ΕΠΕΞΕΡΓΑΣΕΤΕ: δημιουργήθηκε από το xmldocmd για το GroupDocs.Redaction.dll -->
