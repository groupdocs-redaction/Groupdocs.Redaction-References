---
title: "Save"
second_title: "GroupDocs.Redaction για .NET API Reference"
description: "Αποθηκεύει το έγγραφο σε αρχείο με τις ακόλουθες επιλογές AddSuffix  true RasterizeToPDF  true."
type: docs
weight: 60
url: /el/net/groupdocs.redaction/redactor/save/
---
## Save() {#save}

Αποθηκεύει το έγγραφο σε αρχείο με τις ακόλουθες επιλογές: AddSuffix = true, RasterizeToPDF = true.

```csharp
public string Save()
```

### Τιμή Επιστροφής

Διαδρομή προς το επεξεργασμένο έγγραφο

### Δείτε επίσης

* class [Redactor](../../redactor)
* namespace [GroupDocs.Redaction](../../../groupdocs.redaction)
* assembly [GroupDocs.Redaction](../../../)

---

## Save(SaveOptions) {#save_1}

Αποθηκεύει το έγγραφο σε αρχείο.

```csharp
public string Save(SaveOptions saveOptions)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| saveOptions | SaveOptions | Επιλογές για προσθήκη καταλήξεως ή απόδοση σε raster |

### Τιμή Επιστροφής

Διαδρομή προς το επεξεργασμένο έγγραφο

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

* class [SaveOptions](../../../groupdocs.redaction.options/saveoptions)
* class [Redactor](../../redactor)
* namespace [GroupDocs.Redaction](../../../groupdocs.redaction)
* assembly [GroupDocs.Redaction](../../../)

---

## Save(Stream, SaveOptions) {#save_3}

Αποθηκεύει το έγγραφο στην καθορισμένη ροή.

```csharp
public void Save(Stream document, SaveOptions saveOptions)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| έγγραφο | Stream | Η ροή προορισμού. |
| saveOptions | SaveOptions | Οι επιλογές αποθήκευσης που ελέγχουν τη rasterization, την κατάληξη του ονόματος του αρχείου εξόδου και τις ρυθμίσεις αποθήκευσης ειδικές για το έγγραφο. |

### Δείτε επίσης

* class [SaveOptions](../../../groupdocs.redaction.options/saveoptions)
* class [Redactor](../../redactor)
* namespace [GroupDocs.Redaction](../../../groupdocs.redaction)
* assembly [GroupDocs.Redaction](../../../)

<!-- ΜΗΝ ΕΠΕΞΕΡΓΑΣΕΤΕ: δημιουργήθηκε από το xmldocmd για το GroupDocs.Redaction.dll -->
