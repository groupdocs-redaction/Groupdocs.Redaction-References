---
title: "SaveOptions"
second_title: "GroupDocs.Redaction για Java API Αναφορά"
description: "Παρέχει επιλογές για την αλλαγή του ονόματος του αρχείου εξόδου και/ή τη μετατροπή του εγγράφου σε rasterization PDF βασισμένο σε εικόνα."
type: docs
weight: 14
url: /el/java/com.groupdocs.redaction.options/saveoptions/
---
**Inheritance:**
java.lang.Object
```
public class SaveOptions
```

Παρέχει επιλογές για την αλλαγή του ονόματος του αρχείου εξόδου και/ή τη μετατροπή του εγγράφου σε PDF βασισμένο σε εικόνες (rasterization).

*** ** * ** ***


**Learn more**

* [Save with default options](../https://docs.groupdocs.com/redaction/java/save-with-default-options/)
* [Save in rasterized PDF](../https://docs.groupdocs.com/redaction/java/save-in-rasterized-pdf/)
* [Select specific pages for rasterized PDF](../https://docs.groupdocs.com/redaction/java/select-specific-pages-for-rasterized-pdf/)
* [Save in original format](../https://docs.groupdocs.com/redaction/java/save-in-original-format/)
* [Save overwriting original file](../https://docs.groupdocs.com/redaction/java/save-overwriting-original-file/)
* [Save to stream](../https://docs.groupdocs.com/redaction/java/save-to-stream/)

<br />


## Κατασκευαστές

| Κατασκευαστής | Περιγραφή |
| --- | --- |
|  | [SaveOptions()](#SaveOptions--) | Αρχικοποιεί μια νέα παρουσία με προεπιλογές: rasterize σε PDF - false, προσθήκη καταλήξεως - false. |
|
|  | [SaveOptions(boolean rasterizeToPdf, String suffix)](#SaveOptions-boolean-java.lang.String-) | Αρχικοποιεί ένα νέο αντικείμενο με τα δοσμένα παραμέτρους. |
|
## Πεδία

| Πεδίο | Περιγραφή |
| --- | --- |
|  | [SaveSuffix](#SaveSuffix) | Αναπαριστά την προεπιλεγμένη τιμή του επιθήματος, η οποία είναι "Redacted". |
|
## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
|  | [getAddSuffix()](#getAddSuffix--) | Λαμβάνει μια τιμή που υποδεικνύει εάν το όνομα αρχείου πρέπει να αλλάξει πριν από την αποθήκευση. |
|
|  | [setAddSuffix(boolean value)](#setAddSuffix-boolean-) | Ορίζει μια τιμή που υποδεικνύει εάν το όνομα αρχείου πρέπει να αλλάξει πριν από την αποθήκευση. |
|
|  | [getRedactedFileSuffix()](#getRedactedFileSuffix--) | Λαμβάνει ένα προσαρμοσμένο επίθημα για το όνομα αρχείου εξόδου. |
|
|  | [setRedactedFileSuffix(String value)](#setRedactedFileSuffix-java.lang.String-) | Ορίζει ένα προσαρμοσμένο επίθημα για το όνομα αρχείου εξόδου. |
|
|  | [getRasterizeToPDF()](#getRasterizeToPDF--) | Λαμβάνει μια τιμή που υποδεικνύει εάν όλες οι σελίδες του εγγράφου πρέπει να μετατραπούν σε εικόνες και να τοποθετηθούν σε ένα ενιαίο αρχείο PDF. |
|
|  | [setRasterizeToPDF(boolean value)](#setRasterizeToPDF-boolean-) | Ορίζει μια τιμή που υποδεικνύει εάν όλες οι σελίδες του εγγράφου πρέπει να μετατραπούν σε εικόνες και να τοποθετηθούν σε ένα ενιαίο αρχείο PDF. |
|
|  | [getRasterization()](#getRasterization--) | Λαμβάνει τις ρυθμίσεις rasterization. |
|
|  | [getWordprocessingSaveOptions()](#getWordprocessingSaveOptions--) | Επιλογές αποθήκευσης επεξεργασίας κειμένου. |
|
### SaveOptions() {#SaveOptions--}
```
public SaveOptions()
```


Αρχικοποιεί μια νέα παρουσία με προεπιλογές: rasterize σε PDF - false, προσθήκη καταλήξεως - false.


### SaveOptions(boolean rasterizeToPdf, String suffix) {#SaveOptions-boolean-java.lang.String-}
```
public SaveOptions(boolean rasterizeToPdf, String suffix)
```


Αρχικοποιεί ένα νέο αντικείμενο με τα δοσμένα παραμέτρους.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | rasterizeToPdf | boolean | Αληθές, εάν όλες οι σελίδες του εγγράφου πρέπει να μετατραπούν σε εικόνες και να τοποθετηθούν σε ένα ενιαίο αρχείο PDF |
|
|  | suffix | java.lang.String | Αυτό το κείμενο θα προστεθεί στο τέλος του ονόματος αρχείου, εάν δεν είναι κενό επίσης ορίζει το AddSuffix σε αληθές |
|

### SaveSuffix {#SaveSuffix}
```
public static final String SaveSuffix
```


Αναπαριστά την προεπιλεγμένη τιμή του επιθήματος, η οποία είναι "Redacted".


### getAddSuffix() {#getAddSuffix--}
```
public final boolean getAddSuffix()
```


Λαμβάνει μια τιμή που υποδεικνύει εάν το όνομα αρχείου πρέπει να αλλάξει πριν από την αποθήκευση. False εξ ορισμού.


**Returns:**
boolean - Μια τιμή που υποδεικνύει εάν το όνομα αρχείου πρέπει να αλλάξει πριν από την αποθήκευση. False εξ ορισμού.

### setAddSuffix(boolean value) {#setAddSuffix-boolean-}
```
public final void setAddSuffix(boolean value)
```


Ορίζει μια τιμή που υποδεικνύει εάν το όνομα αρχείου πρέπει να αλλάξει πριν από την αποθήκευση. False εξ ορισμού.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | τιμή | boolean | Μια τιμή που υποδεικνύει εάν το όνομα αρχείου πρέπει να αλλάξει πριν από την αποθήκευση. False εξ ορισμού. |
|

### getRedactedFileSuffix() {#getRedactedFileSuffix--}
```
public final String getRedactedFileSuffix()
```


Λαμβάνει ένα προσαρμοσμένο επίθημα για το όνομα αρχείου εξόδου. Εάν δεν καθοριστεί, το
SaveSuffix
σταθερά θα χρησιμοποιηθεί.


**Returns:**
java.lang.String - Ένα προσαρμοσμένο επίθημα για το όνομα αρχείου εξόδου. Εάν δεν καθοριστεί, η σταθερά  SaveSuffix  θα χρησιμοποιηθεί.

### setRedactedFileSuffix(String value) {#setRedactedFileSuffix-java.lang.String-}
```
public final void setRedactedFileSuffix(String value)
```


Ορίζει ένα προσαρμοσμένο επίθημα για το όνομα αρχείου εξόδου. Εάν δεν καθοριστεί, το
SaveSuffix
σταθερά θα χρησιμοποιηθεί.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | τιμή | java.lang.String | Ένα προσαρμοσμένο επίθημα για το όνομα του αρχείου εξόδου. Εάν δεν καθοριστεί, η σταθερά  SaveSuffix  θα χρησιμοποιηθεί. |
|

### getRasterizeToPDF() {#getRasterizeToPDF--}
```
public final boolean getRasterizeToPDF()
```


Λαμβάνει μια τιμή που υποδεικνύει εάν όλες οι σελίδες του εγγράφου πρέπει να μετατραπούν σε εικόνες και να τοποθετηθούν σε ένα ενιαίο αρχείο PDF.


**Returns:**
boolean - Μια τιμή που υποδεικνύει εάν όλες οι σελίδες του εγγράφου πρέπει να μετατραπούν σε εικόνες και να τοποθετηθούν σε ένα ενιαίο αρχείο PDF.

### setRasterizeToPDF(boolean value) {#setRasterizeToPDF-boolean-}
```
public final void setRasterizeToPDF(boolean value)
```


Ορίζει μια τιμή που υποδεικνύει εάν όλες οι σελίδες του εγγράφου πρέπει να μετατραπούν σε εικόνες και να τοποθετηθούν σε ένα ενιαίο αρχείο PDF.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | τιμή | boolean | Μια τιμή που υποδεικνύει εάν όλες οι σελίδες του εγγράφου πρέπει να μετατραπούν σε εικόνες και να τοποθετηθούν σε ένα ενιαίο αρχείο PDF. |
|

### getRasterization() {#getRasterization--}
```
public final RasterizationOptions getRasterization()
```


Λαμβάνει τις ρυθμίσεις rasterization.


**Returns:**
[RasterizationOptions](../../com.groupdocs.redaction.options/rasterizationoptions) - The rasterization settings.

### getWordprocessingSaveOptions() {#getWordprocessingSaveOptions--}
```
public final WordprocessingSaveOptions getWordprocessingSaveOptions()
```


Επιλογές αποθήκευσης επεξεργασίας κειμένου.


**Returns:**
[WordprocessingSaveOptions](../../com.groupdocs.redaction.options/wordprocessingsaveoptions)
