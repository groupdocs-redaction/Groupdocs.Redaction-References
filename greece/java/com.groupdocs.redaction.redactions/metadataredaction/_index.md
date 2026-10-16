---
title: "MetadataRedaction"
second_title: "GroupDocs.Redaction για Java API Αναφορά"
description: "Αντιπροσωπεύει μια βασική αφηρημένη κλάση για διαγραφές μεταδεδομένων εγγράφου."
type: docs
weight: 20
url: /el/java/com.groupdocs.redaction.redactions/metadataredaction/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.redaction.Redaction](../../com.groupdocs.redaction/redaction)
```
public abstract class MetadataRedaction extends Redaction
```

Αντιπροσωπεύει μια βασική αφηρημένη κλάση για διαγραφές μεταδεδομένων εγγράφου.

*** ** * ** ***


**Learn more**

* More details about document metadata redactions: [Metadata redactions](../https://docs.groupdocs.com/redaction/java/metadata-redactions/)

<br />


## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
|  | [getFilter()](#getFilter--) | Αποκτά το φίλτρο, το οποίο χρησιμοποιείται για την επιλογή όλων ή συγκεκριμένων μεταδεδομένων, για παράδειγμα Author ή Company. |
|
|  | [setFilter(int value)](#setFilter-int-) | Ορίζει το φίλτρο, το οποίο χρησιμοποιείται για την επιλογή όλων ή συγκεκριμένων μεταδεδομένων, για παράδειγμα Author ή Company. |
|
|  | [applyTo(DocumentFormatInstance formatInstance)](#applyTo-com.groupdocs.redaction.integration.DocumentFormatInstance-) | Εφαρμόζει τη διαγραφή σε ένα δεδομένο αντικείμενο μορφής. |
|
### getFilter() {#getFilter--}
```
public final int getFilter()
```


Αποκτά το φίλτρο, το οποίο χρησιμοποιείται για την επιλογή όλων ή συγκεκριμένων μεταδεδομένων, για παράδειγμα Author ή Company.


**Returns:**
int - Το φίλτρο, το οποίο χρησιμοποιείται για την επιλογή όλων ή συγκεκριμένων μεταδεδομένων, για παράδειγμα Author ή Company.

### setFilter(int value) {#setFilter-int-}
```
public final void setFilter(int value)
```


Ορίζει το φίλτρο, το οποίο χρησιμοποιείται για την επιλογή όλων ή συγκεκριμένων μεταδεδομένων, για παράδειγμα Author ή Company.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | τιμή | int | Το φίλτρο, το οποίο χρησιμοποιείται για την επιλογή όλων ή συγκεκριμένων μεταδεδομένων, για παράδειγμα Author ή Company. |
|

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

