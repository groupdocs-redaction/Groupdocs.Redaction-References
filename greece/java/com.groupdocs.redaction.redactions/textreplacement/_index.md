---
title: "TextReplacement"
second_title: "GroupDocs.Redaction για Java API Αναφορά"
description: "Αντιπροσωπεύει πληροφορίες κειμενικής αντικατάστασης."
type: docs
weight: 33
url: /el/java/com.groupdocs.redaction.redactions/textreplacement/
---
**Inheritance:**
java.lang.Object
```
public class TextReplacement
```

Αντιπροσωπεύει πληροφορίες κειμενικής αντικατάστασης.

*** ** * ** ***


**Learn more**

* More details about RedactionDescription class and IRedactionCallback interface: [Use redaction callback](../https://docs.groupdocs.com/redaction/java/use-redaction-callback/)

<br />


## Κατασκευαστές

| Κατασκευαστής | Περιγραφή |
| --- | --- |
|  | [TextReplacement(int index, String original, String replacement)](#TextReplacement-int-java.lang.String-java.lang.String-) | Αρχικοποιεί ένα νέο αντικείμενο της κλάσης TextReplacement. |
|
## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
|  | [getIndex()](#getIndex--) | Αποκτά έναν δείκτη του ταιριασμένου κειμένου μέσα στη συμβολοσειρά προέλευσης. |
|
|  | [getOriginalText()](#getOriginalText--) | Αποκτά την αρχική ταιριασμένη συμβολοσειρά. |
|
|  | [getReplacement()](#getReplacement--) | Λαμβάνει τη συμβολοσειρά, αντικαθιστώντας OriginalText. |
|
|  | [toString()](#toString--) | Παρέχει περιγραφή αντικατάστασης κειμένου και τη θέση της. |
|
### TextReplacement(int index, String original, String replacement) {#TextReplacement-int-java.lang.String-java.lang.String-}
```
public TextReplacement(int index, String original, String replacement)
```


Αρχικοποιεί ένα νέο αντικείμενο της κλάσης TextReplacement.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | δείκτης | int | Δείκτης του ταιριασμένου κειμένου μέσα στη συμβολοσειρά προέλευσης |
|
|  | αρχικό | java.lang.String | Αρχική ταιριασμένη συμβολοσειρά |
|
|  | αντικατάσταση | java.lang.String | Συμβολοσειρά, αντικαθιστώντας OriginalText στη συμβολοσειρά προέλευσης |
|

### getIndex() {#getIndex--}
```
public final int getIndex()
```


Αποκτά έναν δείκτη του ταιριασμένου κειμένου μέσα στη συμβολοσειρά προέλευσης.


**Returns:**
int - Δείκτης του ταιριασμένου κειμένου μέσα στη συμβολοσειρά προέλευσης.

### getOriginalText() {#getOriginalText--}
```
public final String getOriginalText()
```


Αποκτά την αρχική ταιριασμένη συμβολοσειρά.


**Returns:**
java.lang.String - Η αρχική ταιριασμένη συμβολοσειρά.

### getReplacement() {#getReplacement--}
```
public final String getReplacement()
```


Λαμβάνει τη συμβολοσειρά, αντικαθιστώντας OriginalText.


**Returns:**
java.lang.String - Η συμβολοσειρά, αντικαθιστώντας OriginalText.

### toString() {#toString--}
```
public String toString()
```


Παρέχει περιγραφή αντικατάστασης κειμένου και τη θέση της.


**Returns:**
java.lang.String - Περιγραφή αντικατάστασης

