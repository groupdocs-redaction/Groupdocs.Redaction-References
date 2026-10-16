---
title: "TextFragment"
second_title: "GroupDocs.Redaction για Java API Αναφορά"
description: "Αντιπροσωπεύει ένα μέρος του αναγνωρισμένου κειμένου, λέξης, συμβόλου κ.λπ. που εξάγεται από τη μηχανή OCR."
type: docs
weight: 15
url: /el/java/com.groupdocs.redaction.integration/textfragment/
---
**Inheritance:**
java.lang.Object
```
public class TextFragment
```

Αντιπροσωπεύει ένα μέρος του αναγνωρισμένου κειμένου (λέξη, σύμβολο κ.λπ.), εξαγόμενο από τη μηχανή OCR.

*** ** * ** ***


**Learn more**

* More details about using OCR in GroupDocs.Redaction: [OCR Usage Basics](../https://docs.groupdocs.com/redaction/java/ocr-usage-basics/)

<br />


## Κατασκευαστές

| Κατασκευαστής | Περιγραφή |
| --- | --- |
|  | [TextFragment(String text, Rectangle rectangle)](#TextFragment-java.lang.String-java.awt.Rectangle-) | Αρχικοποιεί μια νέα παρουσία του αναγνωρισμένου τμήματος κειμένου. |
|
## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
|  | [getText()](#getText--) | Αποκτά το κειμενικό περιεχόμενο του αναγνωρισμένου τμήματος κειμένου. |
|
|  | [getRectangle()](#getRectangle--) | Αποκτά το περιβάλλον ορθογώνιο του αναγνωρισμένου τμήματος κειμένου. |
|
|  | [toString()](#toString--) | Επιστρέφει το κειμενικό περιεχόμενο του αναγνωρισμένου τμήματος κειμένου. |
|
### TextFragment(String text, Rectangle rectangle) {#TextFragment-java.lang.String-java.awt.Rectangle-}
```
public TextFragment(String text, Rectangle rectangle)
```


Αρχικοποιεί μια νέα παρουσία του αναγνωρισμένου τμήματος κειμένου.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | κείμενο | java.lang.String | κειμενικό περιεχόμενο του αναγνωρισμένου τμήματος κειμένου |
|
|  | ορθογώνιο | java.awt.Rectangle | περιβάλλον ορθογώνιο του αναγνωρισμένου τμήματος κειμένου |
|

### getText() {#getText--}
```
public final String getText()
```


Αποκτά το κειμενικό περιεχόμενο του αναγνωρισμένου τμήματος κειμένου.


**Returns:**
java.lang.String - Το κειμενικό περιεχόμενο του αναγνωρισμένου τμήματος κειμένου.

### getRectangle() {#getRectangle--}
```
public final Rectangle getRectangle()
```


Αποκτά το περιβάλλον ορθογώνιο του αναγνωρισμένου τμήματος κειμένου.


**Returns:**
java.awt.Rectangle - Ένα περιβάλλον ορθογώνιο του αναγνωρισμένου τμήματος κειμένου.

### toString() {#toString--}
```
public String toString()
```


Επιστρέφει το κειμενικό περιεχόμενο του αναγνωρισμένου τμήματος κειμένου.


**Returns:**
java.lang.String - κειμενικό περιεχόμενο του αναγνωρισμένου τμήματος κειμένου

