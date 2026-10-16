---
title: "Redactor"
second_title: "GroupDocs.Redaction για .NET API Reference"
description: "Αρχικοποιεί μια νέα παρουσία της κλάσης Redactorgroupdocs.redaction/redactor χρησιμοποιώντας τη διαδρομή του αρχείου."
type: docs
weight: 10
url: /el/net/groupdocs.redaction/redactor/redactor/
---
## Redactor(string) {#constructor_3}

Αρχικοποιεί μια νέα παρουσία της κλάσης [`Redactor`](../../redactor) χρησιμοποιώντας τη διαδρομή του αρχείου.

```csharp
public Redactor(string filePath)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| filePath | String | Διαδρομή προς το αρχείο |

### Παραδείγματα

Το παρακάτω παράδειγμα δείχνει πώς να ανοίξετε ένα έγγραφο για redaction.

```csharp
using (Redactor redactor = new Redactor(@"C:\sample.pdf"))
{
    // Εδώ μπορούμε να χρησιμοποιήσουμε την παρουσία του εγγράφου για να εκτελέσουμε αποκρύψεις
}
```

### Δείτε επίσης

* class [Redactor](../../redactor)
* namespace [GroupDocs.Redaction](../../../groupdocs.redaction)
* assembly [GroupDocs.Redaction](../../../)

---

## Redactor(Stream) {#constructor}

Αρχικοποιεί μια νέα παρουσία της κλάσης [`Redactor`](../../redactor) χρησιμοποιώντας ροή.

```csharp
public Redactor(Stream document)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| έγγραφο | Stream | Ροή προέλευσης του εγγράφου |

### Παραδείγματα

Το παρακάτω παράδειγμα δείχνει πώς να ανοίξετε ένα έγγραφο από ροή.

```csharp
using (Stream stream = File.Open(@"C:\\sample.pdf", FileMode.Open, FileAccess.ReadWrite))
{
    using (Redactor redactor = new Redactor(stream))
    {
        // Εδώ μπορούμε να χρησιμοποιήσουμε την παρουσία του εγγράφου για να εκτελέσουμε αποκρύψεις
    }
}
```

### Δείτε επίσης

* class [Redactor](../../redactor)
* namespace [GroupDocs.Redaction](../../../groupdocs.redaction)
* assembly [GroupDocs.Redaction](../../../)

---

## Redactor(string, LoadOptions) {#constructor_4}

Αρχικοποιεί μια νέα παρουσία της κλάσης [`Redactor`](../../redactor) για ένα έγγραφο προστατευμένο με κωδικό, χρησιμοποιώντας τη διαδρομή του.

```csharp
public Redactor(string filePath, LoadOptions loadOptions)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| filePath | String | Διαδρομή προς αρχείο. |
| loadOptions | LoadOptions | Επιλογές, συμπεριλαμβανομένου κωδικού πρόσβασης. |

### Δείτε επίσης

* class [LoadOptions](../../../groupdocs.redaction.options/loadoptions)
* class [Redactor](../../redactor)
* namespace [GroupDocs.Redaction](../../../groupdocs.redaction)
* assembly [GroupDocs.Redaction](../../../)

---

## Redactor(string, LoadOptions, RedactorSettings) {#constructor_5}

Αρχικοποιεί μια νέα παρουσία της κλάσης [`Redactor`](../../redactor) για ένα έγγραφο προστατευμένο με κωδικό, χρησιμοποιώντας τη διαδρομή του και τις ρυθμίσεις.

```csharp
public Redactor(string filePath, LoadOptions loadOptions, RedactorSettings settings)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| filePath | String | Διαδρομή προς αρχείο. |
| loadOptions | LoadOptions | Επιλογές εξαρτώμενες από το αρχείο, συμπεριλαμβανομένου κωδικού πρόσβασης. |
| ρυθμίσεις | RedactorSettings | Προεπιλεγμένες ρυθμίσεις για τη διαδικασία επεξεργασίας. |

### Δείτε επίσης

* class [LoadOptions](../../../groupdocs.redaction.options/loadoptions)
* class [RedactorSettings](../../../groupdocs.redaction.options/redactorsettings)
* class [Redactor](../../redactor)
* namespace [GroupDocs.Redaction](../../../groupdocs.redaction)
* assembly [GroupDocs.Redaction](../../../)

---

## Redactor(Stream, LoadOptions) {#constructor_1}

Αρχικοποιεί μια νέα παρουσία της κλάσης [`Redactor`](../../redactor) για ένα έγγραφο προστατευμένο με κωδικό, χρησιμοποιώντας ροή.

```csharp
public Redactor(Stream document, LoadOptions loadOptions)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| έγγραφο | Stream | Η ροή εισόδου προέλευσης. |
| loadOptions | LoadOptions | Επιλογές, συμπεριλαμβανομένου κωδικού πρόσβασης. |

### Παραδείγματα

Το παρακάτω παράδειγμα δείχνει πώς να ανοίξετε έγγραφα προστατευμένα με κωδικό χρησιμοποιώντας LoadOptions.

```csharp
LoadOptions loadOptions = new LoadOptions("mypassword");
using (Redactor redactor = new Redactor(@"C:\sample.pdf", loadOptions))
{
    // Εδώ μπορούμε να χρησιμοποιήσουμε την παρουσία του εγγράφου για να εκτελέσουμε αποκρύψεις
}
```

### Δείτε επίσης

* class [LoadOptions](../../../groupdocs.redaction.options/loadoptions)
* class [Redactor](../../redactor)
* namespace [GroupDocs.Redaction](../../../groupdocs.redaction)
* assembly [GroupDocs.Redaction](../../../)

---

## Redactor(Stream, LoadOptions, RedactorSettings) {#constructor_2}

Αρχικοποιεί μια νέα παρουσία της κλάσης [`Redactor`](../../redactor) για ένα έγγραφο προστατευμένο με κωδικό, χρησιμοποιώντας ροή και ρυθμίσεις.

```csharp
public Redactor(Stream document, LoadOptions loadOptions, RedactorSettings settings)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| έγγραφο | Stream | Η ροή εισόδου προέλευσης. |
| loadOptions | LoadOptions | Επιλογές, συμπεριλαμβανομένου κωδικού πρόσβασης. |
| ρυθμίσεις | RedactorSettings | Προεπιλεγμένες ρυθμίσεις για τη διαδικασία επεξεργασίας. |

### Παραδείγματα

Το παρακάτω παράδειγμα δείχνει πώς να ανοίξετε έγγραφα προστατευμένα με κωδικό χρησιμοποιώντας LoadOptions.

```csharp
LoadOptions loadOptions = new LoadOptions("mypassword");
using (Redactor redactor = new Redactor(@"C:\sample.pdf", loadOptions))
{
    // Εδώ μπορούμε να χρησιμοποιήσουμε την παρουσία του εγγράφου για να εκτελέσουμε αποκρύψεις
}
```

### Δείτε επίσης

* class [LoadOptions](../../../groupdocs.redaction.options/loadoptions)
* class [RedactorSettings](../../../groupdocs.redaction.options/redactorsettings)
* class [Redactor](../../redactor)
* namespace [GroupDocs.Redaction](../../../groupdocs.redaction)
* assembly [GroupDocs.Redaction](../../../)

<!-- ΜΗΝ ΕΠΕΞΕΡΓΑΣΕΤΕ: δημιουργήθηκε από το xmldocmd για το GroupDocs.Redaction.dll -->
