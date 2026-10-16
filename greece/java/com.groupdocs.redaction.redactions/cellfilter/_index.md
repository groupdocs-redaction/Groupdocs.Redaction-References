---
title: "CellFilter"
second_title: "GroupDocs.Redaction για Java API Αναφορά"
description: "Παρέχει μια επιλογή για τον περιορισμό του πεδίου μιας CellColumnRedaction σε ένα φύλλο εργασίας και μια στήλη."
type: docs
weight: 12
url: /el/java/com.groupdocs.redaction.redactions/cellfilter/
---
**Inheritance:**
java.lang.Object
```
public class CellFilter
```

Παρέχει μια επιλογή για περιορισμό του πεδίου ενός
CellColumnRedaction
σε ένα φύλλο εργασίας και μια στήλη.

*** ** * ** ***


**Learn more**

* More details about spreadsheet redactions: [Spreadsheet redactions](../https://docs.groupdocs.com/redaction/java/spreadsheet-redactions/)

<br />


## Κατασκευαστές

| Κατασκευαστής | Περιγραφή |
| --- | --- |
|  | [CellFilter()](#CellFilter--) | Αρχικοποιεί μια νέα παρουσία. |
|
## Πεδία

| Πεδίο | Περιγραφή |
| --- | --- |
|  | [NoIndex](#NoIndex) | Αντιπροσωπεύει την προεπιλεγμένη τιμή για το φίλτρο, η οποία είναι -1. |
|
## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
|  | [getWorkSheetName()](#getWorkSheetName--) | Λαμβάνει το όνομα του φύλλου εργασίας (εφόσον υπάρχει). |
|
|  | [setWorkSheetName(String value)](#setWorkSheetName-java.lang.String-) | Ορίζει το όνομα του φύλλου εργασίας (εφόσον υπάρχει). |
|
|  | [getWorkSheetIndex()](#getWorkSheetIndex--) | Λαμβάνει τον δείκτη του φύλλου εργασίας (μηδενική βάση). |
|
|  | [setWorkSheetIndex(int value)](#setWorkSheetIndex-int-) | Ορίζει τον δείκτη του φύλλου εργασίας (μηδενική βάση). |
|
|  | [hasWorkSheetIndex()](#hasWorkSheetIndex--) | Λαμβάνει μια τιμή που υποδεικνύει εάν το |
WorkSheetIndex
είναι ορισμένο ή όχι.
|
|  | [getColumnIndex()](#getColumnIndex--) | Λαμβάνει έναν δείκτη στήλης (μηδενική βάση). |
|
|  | [setColumnIndex(int value)](#setColumnIndex-int-) | Ορίζει έναν δείκτη στήλης (μηδενική βάση). |
|
### CellFilter() {#CellFilter--}
```
public CellFilter()
```


Αρχικοποιεί μια νέα παρουσία.


### NoIndex {#NoIndex}
```
public static final int NoIndex
```


Αντιπροσωπεύει την προεπιλεγμένη τιμή για το φίλτρο, η οποία είναι -1.


### getWorkSheetName() {#getWorkSheetName--}
```
public final String getWorkSheetName()
```


Λαμβάνει το όνομα του φύλλου εργασίας (εφόσον υπάρχει).


**Returns:**
java.lang.String - Ένα όνομα φύλλου εργασίας (εάν ισχύει).

### setWorkSheetName(String value) {#setWorkSheetName-java.lang.String-}
```
public final void setWorkSheetName(String value)
```


Ορίζει το όνομα του φύλλου εργασίας (εφόσον υπάρχει).


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | τιμή | java.lang.String | Ένα όνομα φύλλου εργασίας (εάν ισχύει). |
|

### getWorkSheetIndex() {#getWorkSheetIndex--}
```
public final int getWorkSheetIndex()
```


Λαμβάνει τον δείκτη του φύλλου εργασίας (μηδενική βάση).


**Returns:**
int - Ένας δείκτης φύλλου εργασίας (μηδενική βάση).

### setWorkSheetIndex(int value) {#setWorkSheetIndex-int-}
```
public final void setWorkSheetIndex(int value)
```


Ορίζει τον δείκτη του φύλλου εργασίας (μηδενική βάση).


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | τιμή | int | Ένας δείκτης φύλλου εργασίας (μηδενική βάση). |
|

### hasWorkSheetIndex() {#hasWorkSheetIndex--}
```
public final boolean hasWorkSheetIndex()
```


Λαμβάνει μια τιμή που υποδεικνύει εάν το
WorkSheetIndex
είναι ορισμένο ή όχι.


**Returns:**
boolean - Μια τιμή που υποδεικνύει εάν το  WorkSheetIndex  είναι ορισμένο ή όχι.

### getColumnIndex() {#getColumnIndex--}
```
public final int getColumnIndex()
```


Λαμβάνει έναν δείκτη στήλης (μηδενική βάση).


**Returns:**
int - Ένας δείκτης στήλης (μηδενική βάση).

### setColumnIndex(int value) {#setColumnIndex-int-}
```
public final void setColumnIndex(int value)
```


Ορίζει έναν δείκτη στήλης (μηδενική βάση).


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | τιμή | int | Ένας δείκτης στήλης (μηδενική βάση). |
|

