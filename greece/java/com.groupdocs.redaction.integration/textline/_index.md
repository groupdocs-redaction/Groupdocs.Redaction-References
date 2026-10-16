---
title: "TextLine"
second_title: "GroupDocs.Redaction για Java API Αναφορά"
description: "Αναπαριστά μια γραμμή κειμένου που εξάγεται από τη μηχανή OCR από μια εικόνα."
type: docs
weight: 16
url: /el/java/com.groupdocs.redaction.integration/textline/
---
**Inheritance:**
java.lang.Object
```
public class TextLine
```

Αντιπροσωπεύει μια γραμμή κειμένου, εξαγόμενη από τη μηχανή OCR από μια εικόνα.

*** ** * ** ***


**Learn more**

* More details about using OCR in GroupDocs.Redaction: [OCR Usage Basics](../https://docs.groupdocs.com/redaction/java/ocr-usage-basics/)

<br />


## Κατασκευαστές

| Κατασκευαστής | Περιγραφή |
| --- | --- |
|  | [TextLine(TextFragment[] fragments)](#TextLine-com.groupdocs.redaction.integration.TextFragment---) | Αρχικοποιεί μια νέα παρουσία μιας γραμμής κειμένου, εξαγόμενη από τη μηχανή OCR από μια εικόνα. |
|
## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
|  | [getFragments()](#getFragments--) | Λαμβάνει έναν πίνακα τμημάτων κειμένου, όπως σύμβολα και λέξεις, που αναγνωρίζονται στη γραμμή. |
|
|  | [toString()](#toString--) | Επιστρέφει το κειμενικό περιεχόμενο της αναγνωρισμένης γραμμής κειμένου. |
|
### TextLine(TextFragment[] fragments) {#TextLine-com.groupdocs.redaction.integration.TextFragment---}
```
public TextLine(TextFragment[] fragments)
```


Αρχικοποιεί μια νέα παρουσία μιας γραμμής κειμένου, εξαγόμενη από τη μηχανή OCR από μια εικόνα.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | fragments | [TextFragment\[\]](../../com.groupdocs.redaction.integration/textfragment) | αρχικό σύνολο τμημάτων κειμένου |
|

### getFragments() {#getFragments--}
```
public final TextFragment[] getFragments()
```


Λαμβάνει έναν πίνακα τμημάτων κειμένου, όπως σύμβολα και λέξεις, που αναγνωρίζονται στη γραμμή.


**Returns:**
com.groupdocs.redaction.integration.TextFragment[] - Ένας πίνακας τμημάτων κειμένου, όπως σύμβολα και λέξεις, που αναγνωρίζονται στη γραμμή.

### toString() {#toString--}
```
public String toString()
```


Επιστρέφει το κειμενικό περιεχόμενο της αναγνωρισμένης γραμμής κειμένου.


**Returns:**
java.lang.String - κειμενικό περιεχόμενο της αναγνωρισμένης γραμμής κειμένου

