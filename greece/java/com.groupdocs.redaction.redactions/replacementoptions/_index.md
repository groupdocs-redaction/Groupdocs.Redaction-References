---
title: "ReplacementOptions"
second_title: "GroupDocs.Redaction για Java API Αναφορά"
description: "Αντιπροσωπεύει επιλογές για αντικατάσταση ταιριασμένου κειμένου."
type: docs
weight: 31
url: /el/java/com.groupdocs.redaction.redactions/replacementoptions/
---
**Inheritance:**
java.lang.Object
```
public class ReplacementOptions
```

Αντιπροσωπεύει επιλογές για αντικατάσταση ταιριασμένου κειμένου.

*** ** * ** ***


**Learn more**

* More details about document text redactions: [Text redactions](../https://docs.groupdocs.com/redaction/java/text-redactions/)
* More details about redaction filters: [Use PDF redaction filters](../https://docs.groupdocs.com/redaction/java/use-pdf-redaction-filters/)

<br />


## Κατασκευαστές

| Κατασκευαστής | Περιγραφή |
| --- | --- |
|  | [ReplacementOptions(String replacement)](#ReplacementOptions-java.lang.String-) | Αρχικοποιεί μια νέα παρουσία της κλάσης ReplacementOptions με κείμενο αντικατάστασης ως επιλογή. |
|
|  | [ReplacementOptions(Color color)](#ReplacementOptions-java.awt.Color-) | Αρχικοποιεί μια νέα παρουσία της κλάσης ReplacementOptions με χρωματιστό ορθογώνιο ως επιλογή. |
|
## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
|  | [getActionType()](#getActionType--) | Λαμβάνει τη δράση αντικατάστασης: σχεδίαση πλαισίου ή αντικατάσταση κειμένου. |
|
|  | [getReplacement()](#getReplacement--) | Λαμβάνει την τιμή κειμενικής αντικατάστασης. |
|
|  | [setReplacement(String value)](#setReplacement-java.lang.String-) | Ορίζει την τιμή κειμενικής αντικατάστασης. |
|
|  | [getBoxColor()](#getBoxColor--) | Λαμβάνει το χρώμα για ένα |
ReplacementType.DrawBox
επιλογή (αγνοείται διαφορετικά).
|
|  | [setBoxColor(Color value)](#setBoxColor-java.awt.Color-) | Ορίζει το χρώμα για ένα |
ReplacementType.DrawBox
επιλογή (αγνοείται διαφορετικά).
|
|  | [getFilters()](#getFilters--) | Λαμβάνει έναν πίνακα φίλτρων για εφαρμογή με αυτήν την απόσυρση. |
|
|  | [setFilters(RedactionFilter[] value)](#setFilters-com.groupdocs.redaction.redactions.RedactionFilter---) | Ορίζει έναν πίνακα φίλτρων για εφαρμογή με αυτήν την απόσυρση. |
|
|  | [getCustomRedaction()](#getCustomRedaction--) | Λαμβάνει έναν προσαρμοσμένο χειριστή απόσυρσης. |
|
|  | [setCustomRedaction(ICustomRedactionHandler value)](#setCustomRedaction-com.groupdocs.redaction.redactions.ICustomRedactionHandler-) | Ορίζει έναν προσαρμοσμένο χειριστή απόσυρσης. |
|
| [fromFilters(RedactionFilter[] filters)](#fromFilters-com.groupdocs.redaction.redactions.RedactionFilter---) |  |
### ReplacementOptions(String replacement) {#ReplacementOptions-java.lang.String-}
```
public ReplacementOptions(String replacement)
```


Αρχικοποιεί μια νέα παρουσία της κλάσης ReplacementOptions με κείμενο αντικατάστασης ως επιλογή.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | αντικατάσταση | java.lang.String | Κειμενική αντικατάσταση |
|

### ReplacementOptions(Color color) {#ReplacementOptions-java.awt.Color-}
```
public ReplacementOptions(Color color)
```


Αρχικοποιεί μια νέα παρουσία της κλάσης ReplacementOptions με χρωματιστό ορθογώνιο ως επιλογή.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | χρώμα | java.awt.Color | Χρώμα ορθογωνίου |
|

### getActionType() {#getActionType--}
```
public final ReplacementType getActionType()
```


Λαμβάνει τη δράση αντικατάστασης: σχεδίαση πλαισίου ή αντικατάσταση κειμένου.


**Returns:**
[ReplacementType](../../com.groupdocs.redaction.redactions/replacementtype) - The replacement action: draw box or replace text.

### getReplacement() {#getReplacement--}
```
public final String getReplacement()
```


Λαμβάνει την τιμή κειμενικής αντικατάστασης.


**Returns:**
java.lang.String - Η τιμή κειμενικής αντικατάστασης.

### setReplacement(String value) {#setReplacement-java.lang.String-}
```
public final void setReplacement(String value)
```


Ορίζει την τιμή κειμενικής αντικατάστασης.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | τιμή | java.lang.String | Η τιμή κειμενικής αντικατάστασης. |
|

### getBoxColor() {#getBoxColor--}
```
public final Color getBoxColor()
```


Λαμβάνει το χρώμα για ένα
ReplacementType.DrawBox
επιλογή (αγνοείται διαφορετικά).


**Returns:**
java.awt.Color - Το χρώμα για μια  ReplacementType.DrawBox  επιλογή (αγνοείται διαφορετικά).

### setBoxColor(Color value) {#setBoxColor-java.awt.Color-}
```
public final void setBoxColor(Color value)
```


Ορίζει το χρώμα για ένα
ReplacementType.DrawBox
επιλογή (αγνοείται διαφορετικά).


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | τιμή | java.awt.Color | Το χρώμα για μια  ReplacementType.DrawBox  επιλογή (αγνοείται διαφορετικά). |
|

### getFilters() {#getFilters--}
```
public final RedactionFilter[] getFilters()
```


Λαμβάνει έναν πίνακα φίλτρων για εφαρμογή με αυτήν την απόσυρση.


**Returns:**
com.groupdocs.redaction.redactions.RedactionFilter[] - Ένας πίνακας φίλτρων για εφαρμογή με αυτήν την απόσυρση.

### setFilters(RedactionFilter[] value) {#setFilters-com.groupdocs.redaction.redactions.RedactionFilter---}
```
public final void setFilters(RedactionFilter[] value)
```


Ορίζει έναν πίνακα φίλτρων για εφαρμογή με αυτήν την απόσυρση.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | value | [RedactionFilter\[\]](../../com.groupdocs.redaction.redactions/redactionfilter) | Ένας πίνακας φίλτρων για εφαρμογή με αυτήν την απόσυρση. |
|

### getCustomRedaction() {#getCustomRedaction--}
```
public final ICustomRedactionHandler getCustomRedaction()
```


Λαμβάνει έναν προσαρμοσμένο χειριστή απόσυρσης. Υποστηρίζεται μόνο για PDF [PageAreaRedaction](../../com.groupdocs.redaction.redactions/pagearearedaction).


**Returns:**
[ICustomRedactionHandler](../../com.groupdocs.redaction.redactions/icustomredactionhandler) - An instance of [ICustomRedactionHandler](../../com.groupdocs.redaction.redactions/icustomredactionhandler), or  null  if not set.

### setCustomRedaction(ICustomRedactionHandler value) {#setCustomRedaction-com.groupdocs.redaction.redactions.ICustomRedactionHandler-}
```
public final void setCustomRedaction(ICustomRedactionHandler value)
```


Ορίζει έναν προσαρμοσμένο χειριστή απόσυρσης. Υποστηρίζεται μόνο για PDF [PageAreaRedaction](../../com.groupdocs.redaction.redactions/pagearearedaction).


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | value | [ICustomRedactionHandler](../../com.groupdocs.redaction.redactions/icustomredactionhandler) | Μία παρουσία του [ICustomRedactionHandler](../../com.groupdocs.redaction.redactions/icustomredactionhandler). |
|

### fromFilters(RedactionFilter[] filters) {#fromFilters-com.groupdocs.redaction.redactions.RedactionFilter---}
```
public static ReplacementOptions fromFilters(RedactionFilter[] filters)
```




**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| filters | [RedactionFilter\[\]](../../com.groupdocs.redaction.redactions/redactionfilter) |  |

**Returns:**
[ReplacementOptions](../../com.groupdocs.redaction.redactions/replacementoptions)
