---
title: "RasterizationOptions"
second_title: "GroupDocs.Redaction για Java API Αναφορά"
description: "Παρέχει επιλογές για τη μετατροπή αρχείων σε PDF."
type: docs
weight: 12
url: /el/java/com.groupdocs.redaction.options/rasterizationoptions/
---
**Inheritance:**
java.lang.Object
```
public class RasterizationOptions
```

Παρέχει επιλογές για τη μετατροπή αρχείων σε PDF.

*** ** * ** ***


**Learn more**

* More details about saving document as a rasterized PDF: [Save in rasterized PDF](../https://docs.groupdocs.com/redaction/java/save-in-rasterized-pdf/)
* More details about rasterization options: [Select specific pages for rasterized PDF](../https://docs.groupdocs.com/redaction/java/select-specific-pages-for-rasterized-pdf/)

<br />


## Κατασκευαστές

| Κατασκευαστής | Περιγραφή |
| --- | --- |
|  | [RasterizationOptions()](#RasterizationOptions--) | Αρχικοποιεί μια νέα παρουσία. |
|
## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
|  | [getEnabled()](#getEnabled--) | Λαμβάνει μια τιμή που υποδεικνύει εάν όλες οι σελίδες του εγγράφου πρέπει να μετατραπούν σε εικόνες και να τοποθετηθούν σε ένα ενιαίο αρχείο PDF. |
|
|  | [setEnabled(boolean value)](#setEnabled-boolean-) | Ορίζει μια τιμή που υποδεικνύει εάν όλες οι σελίδες του εγγράφου πρέπει να μετατραπούν σε εικόνες και να τοποθετηθούν σε ένα ενιαίο αρχείο PDF. |
|
|  | [getPageIndex()](#getPageIndex--) | Λαμβάνει τον δείκτη της πρώτης σελίδας (από το 0) για μετατροπή σε PDF. |
|
|  | [setPageIndex(int value)](#setPageIndex-int-) | Ορίζει τον δείκτη της πρώτης σελίδας (από το 0) για μετατροπή σε PDF. |
|
|  | [isStartPageIndexSet()](#isStartPageIndexSet--) | Λαμβάνει μια τιμή που υποδεικνύει εάν η ιδιότητα PageIndex άλλαξε (ορίστηκε) μετά την αρχικοποίησή της. |
|
|  | [getPageCount()](#getPageCount--) | Λαμβάνει τον αριθμό των σελίδων που θα μετατραπούν σε PDF. |
|
|  | [setPageCount(int value)](#setPageCount-int-) | Ορίζει τον αριθμό των σελίδων που θα μετατραπούν σε PDF. |
|
|  | [isPageCountSet()](#isPageCountSet--) | Λαμβάνει μια τιμή που υποδεικνύει εάν η ιδιότητα PageCount άλλαξε (ορίστηκε) μετά την αρχικοποίησή της. |
|
|  | [getCompliance()](#getCompliance--) | Λαμβάνει το επίπεδο συμμόρφωσης PDF. |
|
|  | [setCompliance(PdfComplianceLevel value)](#setCompliance-com.groupdocs.redaction.options.PdfComplianceLevel-) | Ορίζει το επίπεδο συμμόρφωσης PDF. |
|
|  | [hasAdvancedOptions()](#hasAdvancedOptions--) | Λαμβάνει έναν δείκτη, ο οποίος είναι αληθής εάν έχουν οριστεί προχωρημένες επιλογές rasterization. |
|
|  | [addAdvancedOption(AdvancedRasterizationOptions optionType)](#addAdvancedOption-com.groupdocs.redaction.options.AdvancedRasterizationOptions-) | Μπορείτε να χρησιμοποιήσετε αυτή τη μέθοδο για να καταχωρήσετε μια προχωρημένη επιλογή rasterization προς εφαρμογή. |
|
|  | [addAdvancedOption(AdvancedRasterizationOptions optionType, HashMap<String,String> parameters)](#addAdvancedOption-com.groupdocs.redaction.options.AdvancedRasterizationOptions-java.util.HashMap-java.lang.String-java.lang.String--) | Μπορείτε να χρησιμοποιήσετε αυτή τη μέθοδο για να καταχωρήσετε μια προχωρημένη επιλογή rasterization προς εφαρμογή. |
|
### RasterizationOptions() {#RasterizationOptions--}
```
public RasterizationOptions()
```


Αρχικοποιεί μια νέα παρουσία.


### getEnabled() {#getEnabled--}
```
public final boolean getEnabled()
```


Λαμβάνει μια τιμή που υποδεικνύει εάν όλες οι σελίδες του εγγράφου πρέπει να μετατραπούν σε εικόνες και να τοποθετηθούν σε ένα ενιαίο αρχείο PDF. Η προεπιλογή είναι TRUE, ορίστε σε FALSE για να αποφύγετε το rasterization.


**Returns:**
boolean - Μια τιμή που υποδεικνύει εάν όλες οι σελίδες του εγγράφου πρέπει να μετατραπούν σε εικόνες και να τοποθετηθούν σε ένα ενιαίο αρχείο PDF. Η προεπιλογή είναι TRUE, ορίστε σε FALSE για να αποφύγετε το rasterization.

### setEnabled(boolean value) {#setEnabled-boolean-}
```
public final void setEnabled(boolean value)
```


Ορίζει μια τιμή που υποδεικνύει εάν όλες οι σελίδες του εγγράφου πρέπει να μετατραπούν σε εικόνες και να τοποθετηθούν σε ένα ενιαίο αρχείο PDF. Η προεπιλογή είναι TRUE, ορίστε σε FALSE για να αποφύγετε το rasterization.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | τιμή | boolean | Μια τιμή που υποδεικνύει εάν όλες οι σελίδες του εγγράφου πρέπει να μετατραπούν σε εικόνες και να τοποθετηθούν σε ένα ενιαίο αρχείο PDF. Η προεπιλογή είναι TRUE, ορίστε σε FALSE για να αποφύγετε το rasterization. |
|

### getPageIndex() {#getPageIndex--}
```
public final int getPageIndex()
```


Λαμβάνει τον δείκτη της πρώτης σελίδας (από το 0) για μετατροπή σε PDF.


**Returns:**
int - Ο δείκτης της πρώτης σελίδας (από το 0) που θα μετατραπεί σε PDF.

### setPageIndex(int value) {#setPageIndex-int-}
```
public final void setPageIndex(int value)
```


Ορίζει τον δείκτη της πρώτης σελίδας (από το 0) για μετατροπή σε PDF.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | τιμή | int | Ο δείκτης της πρώτης σελίδας (από το 0) που θα μετατραπεί σε PDF. |
|

### isStartPageIndexSet() {#isStartPageIndexSet--}
```
public final boolean isStartPageIndexSet()
```


Λαμβάνει μια τιμή που υποδεικνύει εάν η ιδιότητα PageIndex άλλαξε (ορίστηκε) μετά την αρχικοποίησή της.


**Returns:**
boolean - Μια τιμή που υποδεικνύει εάν η ιδιότητα PageIndex άλλαξε (ορίστηκε) μετά την αρχικοποίησή της.

### getPageCount() {#getPageCount--}
```
public final int getPageCount()
```


Λαμβάνει τον αριθμό των σελίδων που θα μετατραπούν σε PDF.


**Returns:**
int - Ο αριθμός των σελίδων που θα μετατραπούν σε PDF.

### setPageCount(int value) {#setPageCount-int-}
```
public final void setPageCount(int value)
```


Ορίζει τον αριθμό των σελίδων που θα μετατραπούν σε PDF.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | τιμή | int | Ο αριθμός των σελίδων που θα μετατραπούν σε PDF. |
|

### isPageCountSet() {#isPageCountSet--}
```
public final boolean isPageCountSet()
```


Λαμβάνει μια τιμή που υποδεικνύει εάν η ιδιότητα PageCount άλλαξε (ορίστηκε) μετά την αρχικοποίησή της.


**Returns:**
boolean - Μια τιμή που υποδεικνύει εάν η ιδιότητα PageCount άλλαξε (ορίστηκε) μετά την αρχικοποίησή της.

### getCompliance() {#getCompliance--}
```
public final PdfComplianceLevel getCompliance()
```


Λαμβάνει το επίπεδο συμμόρφωσης PDF.


**Returns:**
[PdfComplianceLevel](../../com.groupdocs.redaction.options/pdfcompliancelevel) - The PDF Compliance level.

### setCompliance(PdfComplianceLevel value) {#setCompliance-com.groupdocs.redaction.options.PdfComplianceLevel-}
```
public final void setCompliance(PdfComplianceLevel value)
```


Ορίζει το επίπεδο συμμόρφωσης PDF.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | value | [PdfComplianceLevel](../../com.groupdocs.redaction.options/pdfcompliancelevel) | Το επίπεδο συμμόρφωσης PDF. |
|

### hasAdvancedOptions() {#hasAdvancedOptions--}
```
public final boolean hasAdvancedOptions()
```


Λαμβάνει έναν δείκτη, ο οποίος είναι αληθής εάν έχουν οριστεί προχωρημένες επιλογές rasterization.


**Returns:**
boolean - Ένας δείκτης, ο οποίος είναι αληθής εάν έχουν οριστεί προχωρημένες επιλογές rasterization.

### addAdvancedOption(AdvancedRasterizationOptions optionType) {#addAdvancedOption-com.groupdocs.redaction.options.AdvancedRasterizationOptions-}
```
public final void addAdvancedOption(AdvancedRasterizationOptions optionType)
```


Μπορείτε να χρησιμοποιήσετε αυτή τη μέθοδο για να καταχωρήσετε μια προχωρημένη επιλογή rasterization προς εφαρμογή.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | optionType | [AdvancedRasterizationOptions](../../com.groupdocs.redaction.options/advancedrasterizationoptions) | Παρέχει πληροφορίες σχετικά με τον επιλεγμένο τύπο εφέ (γκρίζα κλίμακα, περίγραμμα κ.λπ.). |
|

### addAdvancedOption(AdvancedRasterizationOptions optionType, HashMap<String,String> parameters) {#addAdvancedOption-com.groupdocs.redaction.options.AdvancedRasterizationOptions-java.util.HashMap-java.lang.String-java.lang.String--}
```
public final void addAdvancedOption(AdvancedRasterizationOptions optionType, HashMap<String,String> parameters)
```


Μπορείτε να χρησιμοποιήσετε αυτή τη μέθοδο για να καταχωρήσετε μια προχωρημένη επιλογή rasterization προς εφαρμογή.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | optionType | [AdvancedRasterizationOptions](../../com.groupdocs.redaction.options/advancedrasterizationoptions) | Παρέχει πληροφορίες σχετικά με τον επιλεγμένο τύπο εφέ (γκρίζα κλίμακα, περίγραμμα κ.λπ.). |
|
|  | παράμετροι | java.util.HashMap<java.lang.String,java.lang.String> | Παράμετροι για το συγκεκριμένο εφέ, όπως η γωνία περιστροφής. |
|

