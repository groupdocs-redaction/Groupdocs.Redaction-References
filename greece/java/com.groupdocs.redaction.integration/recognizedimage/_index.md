---
title: "RecognizedImage"
second_title: "GroupDocs.Redaction για Java API Αναφορά"
description: "Αναπαριστά το κείμενο που εξάγεται από μια εικόνα ως αποτέλεσμα της διαδικασίας αναγνώρισής της."
type: docs
weight: 13
url: /el/java/com.groupdocs.redaction.integration/recognizedimage/
---
**Inheritance:**
java.lang.Object
```
public class RecognizedImage
```

Αντιπροσωπεύει κείμενο, εξαγόμενο από μια εικόνα ως αποτέλεσμα της διαδικασίας αναγνώρισής της.

*** ** * ** ***


**Learn more**

* More details about using OCR in GroupDocs.Redaction: [OCR Usage Basics](../https://docs.groupdocs.com/redaction/java/ocr-usage-basics/)

<br />


## Κατασκευαστές

| Κατασκευαστής | Περιγραφή |
| --- | --- |
|  | [RecognizedImage(TextLine[] lines)](#RecognizedImage-com.groupdocs.redaction.integration.TextLine---) | Αρχικοποιεί μια νέα παρουσία της κλάσης, χρησιμοποιώντας ένα σύνολο αναγνωρισμένων γραμμών. |
|
## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
|  | [getText()](#getText--) | Λαμβάνει την κειμενική ισοδύναμη του δομημένου κειμένου. |
|
|  | [getLines()](#getLines--) | Λαμβάνει τις γραμμές κειμένου, με τα τμήματά τους, που αναγνωρίστηκαν μέσα στο έγγραφο. |
|
|  | [toString()](#toString--) | Λαμβάνει την κειμενική ισοδύναμη του δομημένου κειμένου. |
|
### RecognizedImage(TextLine[] lines) {#RecognizedImage-com.groupdocs.redaction.integration.TextLine---}
```
public RecognizedImage(TextLine[] lines)
```


Αρχικοποιεί μια νέα παρουσία της κλάσης, χρησιμοποιώντας ένα σύνολο αναγνωρισμένων γραμμών.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | lines | [TextLine\[\]](../../com.groupdocs.redaction.integration/textline) | ένα IEnumerable (π.χ. λίστα ή πίνακας) των αναγνωρισμένων γραμμών |
|

### getText() {#getText--}
```
public final String getText()
```


Λαμβάνει την κειμενική ισοδύναμη του δομημένου κειμένου.


**Returns:**
java.lang.String - Κειμενική ισοδύναμη του δομημένου κειμένου.

### getLines() {#getLines--}
```
public final TextLine[] getLines()
```


Λαμβάνει τις γραμμές κειμένου, με τα τμήματά τους, που αναγνωρίστηκαν μέσα στο έγγραφο.


**Returns:**
com.groupdocs.redaction.integration.TextLine[] - Γραμμές κειμένου, με τα τμήματά τους, που αναγνωρίστηκαν μέσα στο έγγραφο.

### toString() {#toString--}
```
public String toString()
```


Λαμβάνει την κειμενική ισοδύναμη του δομημένου κειμένου.


**Returns:**
java.lang.String - Αναγνωρισμένο κείμενο

