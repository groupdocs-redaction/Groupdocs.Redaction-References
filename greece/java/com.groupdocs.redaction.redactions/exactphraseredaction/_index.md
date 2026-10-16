---
title: "ExactPhraseRedaction"
second_title: "GroupDocs.Redaction για Java API Αναφορά"
description: "Αναπαριστά μια διαγραφή κειμένου που αντικαθιστά ακριβή φράση στο κείμενο των εγγράφων, χωρίς διάκριση πεζών-κεφαλαίων εξ ορισμού."
type: docs
weight: 17
url: /el/java/com.groupdocs.redaction.redactions/exactphraseredaction/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.redaction.Redaction](../../com.groupdocs.redaction/redaction), [com.groupdocs.redaction.redactions.TextRedaction](../../com.groupdocs.redaction.redactions/textredaction)
```
public class ExactPhraseRedaction extends TextRedaction
```

Αντιπροσωπεύει μια επεξεργασία κειμένου που αντικαθιστά ακριβή φράση στο κείμενο του εγγράφου, χωρίς διάκριση πεζών-κεφαλαίων από προεπιλογή.

*** ** * ** ***


**Learn more**

* More details about applying redactions: [Redaction basics](../https://docs.groupdocs.com/redaction/java/redaction-basics/)
* More details about document text redactions: [Text redactions](../https://docs.groupdocs.com/redaction/java/text-redactions/)

<br />

Το παρακάτω παράδειγμα δείχνει την εκτέλεση αναζήτησης φράσης με διάκριση πεζών-κεφαλαίων και αντικατάστασης.

````

  try (Redactor redactor = new Redactor("C:\\sample.pdf"))
 {
   // By default, the second parameter, isCaseSensitive = false;
   doc.apply(new ExactPhraseRedaction("John Doe", true, new ReplacementOptions("[personal]")));
   doc.save();
 }
 
``` 
````

The following example demonstrates replacing phrase (case insensitive) with solid red rectangle.

````

try (Redactor redactor = new Redactor("C:\\sample.pdf"))
{
// Από προεπιλογή, isCaseSensitive = false;
doc.apply(new ExactPhraseRedaction("John Doe", new ReplacementOptions(System.Drawing.Color.Red)));", "doc.save();
}
Αρχικοποιεί ένα νέο αντικείμενο της κλάσης ExactPhraseRedaction σε λειτουργία χωρίς διάκριση πεζών-κεφαλαίων.
 
``` 
````


## Κατασκευαστές

| Κατασκευαστής | Περιγραφή |
| --- | --- |
|  | [ExactPhraseRedaction(String searchPhrase, ReplacementOptions options)](#ExactPhraseRedaction-java.lang.String-com.groupdocs.redaction.redactions.ReplacementOptions-) | Αρχικοποιεί ένα νέο αντικείμενο της κλάσης ExactPhraseRedaction. |
|
|  | [ExactPhraseRedaction(String searchPhrase, boolean isCaseSensitive, ReplacementOptions options)](#ExactPhraseRedaction-java.lang.String-boolean-com.groupdocs.redaction.redactions.ReplacementOptions-) | Αρχικοποιεί μια νέα παρουσία της κλάσης ExactPhraseRedaction. |
|
## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
|  | [getSearchPhrase()](#getSearchPhrase--) | Λαμβάνει τη συμβολοσειρά για αναζήτηση και αντικατάσταση. |
|
|  | [isCaseSensitive()](#isCaseSensitive--) | Λαμβάνει μια τιμή που υποδεικνύει εάν η αναζήτηση είναι ευαίσθητη σε πεζά-κεφαλαία ή όχι. |
|
|  | [isRightToLeft()](#isRightToLeft--) | Λαμβάνει μια τιμή που υποδεικνύει εάν αυτό το κείμενο είναι από δεξιά προς αριστερά ή όχι, ψευδές εξ ορισμού. |
|
|  | [setRightToLeft(boolean value)](#setRightToLeft-boolean-) | Ορίζει μια τιμή που υποδεικνύει εάν αυτό το κείμενο είναι από δεξιά προς αριστερά ή όχι, ψευδές εξ ορισμού. |
|
|  | [getDescription()](#getDescription--) | Επιστρέφει μια συμβολοσειρά που περιγράφει τη διαγραφή και τις παραμέτρους της. |
|
|  | [applyTo(DocumentFormatInstance formatInstance)](#applyTo-com.groupdocs.redaction.integration.DocumentFormatInstance-) | Εφαρμόζει τη διαγραφή σε ένα δεδομένο αντικείμενο μορφής. |
|
### ExactPhraseRedaction(String searchPhrase, ReplacementOptions options) {#ExactPhraseRedaction-java.lang.String-com.groupdocs.redaction.redactions.ReplacementOptions-}
```
public ExactPhraseRedaction(String searchPhrase, ReplacementOptions options)
```


Αρχικοποιεί ένα νέο αντικείμενο της κλάσης ExactPhraseRedaction.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | searchPhrase | java.lang.String | Συμβολοσειρά για αναζήτηση και αντικατάσταση |
|
|  | options | [ReplacementOptions](../../com.groupdocs.redaction.redactions/replacementoptions) | Επιλογές αντικατάστασης (κειμενικές, χρώματος) |
|

### ExactPhraseRedaction(String searchPhrase, boolean isCaseSensitive, ReplacementOptions options) {#ExactPhraseRedaction-java.lang.String-boolean-com.groupdocs.redaction.redactions.ReplacementOptions-}
```
public ExactPhraseRedaction(String searchPhrase, boolean isCaseSensitive, ReplacementOptions options)
```


Αρχικοποιεί μια νέα παρουσία της κλάσης ExactPhraseRedaction.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | searchPhrase | java.lang.String | Συμβολοσειρά για αναζήτηση και αντικατάσταση |
|
|  | isCaseSensitive | boolean | Αληθές εάν απαιτείται αναζήτηση με διάκριση πεζών-κεφαλαίων |
|
|  | options | [ReplacementOptions](../../com.groupdocs.redaction.redactions/replacementoptions) | Επιλογές αντικατάστασης (κειμενικές, χρώματος) |
|

### getSearchPhrase() {#getSearchPhrase--}
```
public final String getSearchPhrase()
```


Λαμβάνει τη συμβολοσειρά για αναζήτηση και αντικατάσταση.


**Returns:**
java.lang.String - Η συμβολοσειρά για αναζήτηση και αντικατάσταση.

### isCaseSensitive() {#isCaseSensitive--}
```
public final boolean isCaseSensitive()
```


Λαμβάνει μια τιμή που υποδεικνύει εάν η αναζήτηση είναι ευαίσθητη σε πεζά-κεφαλαία ή όχι.


**Returns:**
boolean - Μια τιμή που υποδεικνύει εάν η αναζήτηση είναι ευαίσθητη σε πεζά-κεφαλαία ή όχι.

### isRightToLeft() {#isRightToLeft--}
```
public final boolean isRightToLeft()
```


Λαμβάνει μια τιμή που υποδεικνύει εάν αυτό το κείμενο είναι από δεξιά προς αριστερά ή όχι, ψευδές εξ ορισμού.


**Returns:**
boolean - Μια τιμή που υποδεικνύει εάν αυτό το κείμενο είναι από δεξιά προς αριστερά ή όχι, ψευδές εξ ορισμού.

### setRightToLeft(boolean value) {#setRightToLeft-boolean-}
```
public final void setRightToLeft(boolean value)
```


Ορίζει μια τιμή που υποδεικνύει εάν αυτό το κείμενο είναι από δεξιά προς αριστερά ή όχι, ψευδές εξ ορισμού.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | τιμή | boolean | Μια τιμή που υποδεικνύει εάν αυτό το κείμενο είναι από δεξιά προς αριστερά ή όχι, ψευδές εξ ορισμού. |
|

### getDescription() {#getDescription--}
```
public String getDescription()
```


Επιστρέφει μια συμβολοσειρά που περιγράφει τη διαγραφή και τις παραμέτρους της.


**Returns:**
java.lang.String - Κείμενο, που περιέχει το όνομα και τις παραμέτρους της διαγραφής.

### applyTo(DocumentFormatInstance formatInstance) {#applyTo-com.groupdocs.redaction.integration.DocumentFormatInstance-}
```
public RedactorLogEntry applyTo(DocumentFormatInstance formatInstance)
```


Εφαρμόζει τη διαγραφή σε ένα δεδομένο αντικείμενο μορφής.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | formatInstance | [DocumentFormatInstance](../../com.groupdocs.redaction.integration/documentformatinstance) | Μία παρουσία ενός εγγράφου για εφαρμογή διαγραφής |
|

**Returns:**
[RedactorLogEntry](../../com.groupdocs.redaction/redactorlogentry) - Status of the redaction: success/failure and error message if any

