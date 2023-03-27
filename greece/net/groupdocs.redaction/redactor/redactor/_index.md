---
title: Redactor
second_title: GroupDocs.Redaction για Αναφορά API .NET
description: Αρχικοποιεί μια νέα παρουσία τουRedactorgroupdocs.redaction/redactor κλάση χρησιμοποιώντας διαδρομή αρχείου.
type: docs
weight: 10
url: /el/net/groupdocs.redaction/redactor/redactor/
---
## Redactor(string) {#constructor_3}

Αρχικοποιεί μια νέα παρουσία του[`Redactor`](../../redactor) κλάση χρησιμοποιώντας διαδρομή αρχείου.

```csharp
public Redactor(string filePath)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| filePath | String | Διαδρομή προς το αρχείο |

### Παραδείγματα

Το ακόλουθο παράδειγμα δείχνει πώς να ανοίξετε ένα έγγραφο για επεξεργασία.

```csharp
using (Redactor redactor = new Redactor(@"C:\sample.pdf"))
{
    // Εδώ μπορούμε να χρησιμοποιήσουμε το παράδειγμα εγγράφου για να εκτελέσουμε διορθώσεις
}
```

### Δείτε επίσης

* class [Redactor](../../redactor)
* χώρος ονομάτων [GroupDocs.Redaction](../../redactor)
* συνέλευση [GroupDocs.Redaction](../../../)

---

## Redactor(Stream) {#constructor}

Αρχικοποιεί μια νέα παρουσία του[`Redactor`](../../redactor) τάξη με χρήση ροής.

```csharp
public Redactor(Stream document)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| document | Stream | Ροή πηγής του εγγράφου |

### Παραδείγματα

Το ακόλουθο παράδειγμα δείχνει πώς να ανοίξετε ένα έγγραφο από ροή.

```csharp
using (Stream stream = File.Open(@"C:\\sample.pdf", FileMode.Open, FileAccess.ReadWrite))
{
    using (Redactor redactor = new Redactor(stream))
    {
        // Εδώ μπορούμε να χρησιμοποιήσουμε το παράδειγμα εγγράφου για να εκτελέσουμε διορθώσεις
    }
}
```

### Δείτε επίσης

* class [Redactor](../../redactor)
* χώρος ονομάτων [GroupDocs.Redaction](../../redactor)
* συνέλευση [GroupDocs.Redaction](../../../)

---

## Redactor(string, LoadOptions) {#constructor_4}

Αρχικοποιεί μια νέα παρουσία του[`Redactor`](../../redactor) κλάση για ένα έγγραφο που προστατεύεται με κωδικό πρόσβασης χρησιμοποιώντας τη διαδρομή του.

```csharp
public Redactor(string filePath, LoadOptions loadOptions)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| filePath | String | Διαδρομή προς το αρχείο. |
| loadOptions | LoadOptions | Επιλογές, συμπεριλαμβανομένου του κωδικού πρόσβασης. |

### Δείτε επίσης

* class [LoadOptions](../../../groupdocs.redaction.options/loadoptions)
* class [Redactor](../../redactor)
* χώρος ονομάτων [GroupDocs.Redaction](../../redactor)
* συνέλευση [GroupDocs.Redaction](../../../)

---

## Redactor(string, LoadOptions, RedactorSettings) {#constructor_5}

Αρχικοποιεί μια νέα παρουσία του[`Redactor`](../../redactor) τάξη για ένα έγγραφο που προστατεύεται με κωδικό πρόσβασης χρησιμοποιώντας τη διαδρομή και τις ρυθμίσεις του.

```csharp
public Redactor(string filePath, LoadOptions loadOptions, RedactorSettings settings)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| filePath | String | Διαδρομή προς το αρχείο. |
| loadOptions | LoadOptions | Επιλογές που εξαρτώνται από το αρχείο, συμπεριλαμβανομένου του κωδικού πρόσβασης. |
| settings | RedactorSettings | Προεπιλεγμένες ρυθμίσεις για τη διαδικασία σύνταξης. |

### Δείτε επίσης

* class [LoadOptions](../../../groupdocs.redaction.options/loadoptions)
* class [RedactorSettings](../../../groupdocs.redaction.options/redactorsettings)
* class [Redactor](../../redactor)
* χώρος ονομάτων [GroupDocs.Redaction](../../redactor)
* συνέλευση [GroupDocs.Redaction](../../../)

---

## Redactor(Stream, LoadOptions) {#constructor_1}

Αρχικοποιεί μια νέα παρουσία του[`Redactor`](../../redactor) τάξη για ένα έγγραφο που προστατεύεται με κωδικό πρόσβασης με χρήση ροής.

```csharp
public Redactor(Stream document, LoadOptions loadOptions)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| document | Stream | Ροή εισόδου πηγής. |
| loadOptions | LoadOptions | Επιλογές, συμπεριλαμβανομένου του κωδικού πρόσβασης. |

### Παραδείγματα

Το ακόλουθο παράδειγμα δείχνει πώς να ανοίξετε έγγραφα που προστατεύονται με κωδικό πρόσβασης χρησιμοποιώντας το LoadOptions.

```csharp
LoadOptions loadOptions = new LoadOptions("mypassword");
using (Redactor redactor = new Redactor(@"C:\sample.pdf", loadOptions))
{
    // Εδώ μπορούμε να χρησιμοποιήσουμε το παράδειγμα εγγράφου για να εκτελέσουμε διορθώσεις
}
```

### Δείτε επίσης

* class [LoadOptions](../../../groupdocs.redaction.options/loadoptions)
* class [Redactor](../../redactor)
* χώρος ονομάτων [GroupDocs.Redaction](../../redactor)
* συνέλευση [GroupDocs.Redaction](../../../)

---

## Redactor(Stream, LoadOptions, RedactorSettings) {#constructor_2}

Αρχικοποιεί μια νέα παρουσία του[`Redactor`](../../redactor)τάξη για ένα έγγραφο που προστατεύεται με κωδικό πρόσβασης χρησιμοποιώντας ροή και ρυθμίσεις.

```csharp
public Redactor(Stream document, LoadOptions loadOptions, RedactorSettings settings)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| document | Stream | Ροή εισόδου πηγής. |
| loadOptions | LoadOptions | Επιλογές, συμπεριλαμβανομένου του κωδικού πρόσβασης. |
| settings | RedactorSettings | Προεπιλεγμένες ρυθμίσεις για τη διαδικασία σύνταξης. |

### Παραδείγματα

Το ακόλουθο παράδειγμα δείχνει πώς να ανοίξετε έγγραφα που προστατεύονται με κωδικό πρόσβασης χρησιμοποιώντας το LoadOptions.

```csharp
LoadOptions loadOptions = new LoadOptions("mypassword");
using (Redactor redactor = new Redactor(@"C:\sample.pdf", loadOptions))
{
    // Εδώ μπορούμε να χρησιμοποιήσουμε το παράδειγμα εγγράφου για να εκτελέσουμε διορθώσεις
}
```

### Δείτε επίσης

* class [LoadOptions](../../../groupdocs.redaction.options/loadoptions)
* class [RedactorSettings](../../../groupdocs.redaction.options/redactorsettings)
* class [Redactor](../../redactor)
* χώρος ονομάτων [GroupDocs.Redaction](../../redactor)
* συνέλευση [GroupDocs.Redaction](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Redaction.dll -->
