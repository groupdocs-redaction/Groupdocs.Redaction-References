---
title: "MetadataItem"
second_title: "GroupDocs.Redaction για Java API Αναφορά"
description: "Αναπαριστά ένα στοιχείο μεταδεδομένων κοινό για όλες τις υποστηριζόμενες μορφές και χρησιμοποιείται σε επεμβάσεις μεταδεδομένων."
type: docs
weight: 12
url: /el/java/com.groupdocs.redaction.integration/metadataitem/
---
**Inheritance:**
java.lang.Object
```
public class MetadataItem
```

Αντιπροσωπεύει ένα στοιχείο μεταδεδομένων, κοινό για όλες τις υποστηριζόμενες μορφές και χρησιμοποιείται σε διαγραφές μεταδεδομένων.

## Κατασκευαστές

| Κατασκευαστής | Περιγραφή |
| --- | --- |
|  | [MetadataItem()](#MetadataItem--) | Αρχικοποιεί μια νέα παρουσία. |
|
## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
|  | [getOriginalName()](#getOriginalName--) | Λαμβάνει το αρχικό όνομα του στοιχείου μεταδεδομένων, όπως εμφανίζεται στο έγγραφο. |
|
|  | [setOriginalName(String value)](#setOriginalName-java.lang.String-) | Ορίζει το αρχικό όνομα του στοιχείου μεταδεδομένων, όπως εμφανίζεται στο έγγραφο. |
|
|  | [getCategory()](#getCategory--) | Λαμβάνει μια κατηγορία του στοιχείου μεταδεδομένων, για παράδειγμα το αναγνωριστικό πόρου για ένα ενσωματωμένο στοιχείο μεταδεδομένων πόρου. |
|
|  | [setCategory(String value)](#setCategory-java.lang.String-) | Ορίζει μια κατηγορία του στοιχείου μεταδεδομένων, για παράδειγμα το αναγνωριστικό πόρου για ένα ενσωματωμένο στοιχείο μεταδεδομένων. |
|
|  | [getFilter()](#getFilter--) | Λαμβάνει μια τιμή του |
MetadataFilters
, που ανατίθεται σε αυτό το στοιχείο μεταδεδομένων και χρησιμοποιείται στο φιλτράρισμα των στοιχείων.
|
|  | [setFilter(int value)](#setFilter-int-) | Ορίζει μια τιμή του |
MetadataFilters
, που ανατίθεται σε αυτό το στοιχείο μεταδεδομένων και χρησιμοποιείται στο φιλτράρισμα των στοιχείων.
|
|  | [getValues()](#getValues--) | Λαμβάνει την τιμή του στοιχείου μεταδεδομένων. |
|
|  | [setValues(List<String> value)](#setValues-java.util.List-java.lang.String--) | Ορίζει την τιμή του στοιχείου μεταδεδομένων. |
|
|  | [isCustom()](#isCustom--) | Λαμβάνει μια τιμή που υποδεικνύει αν αυτό το στοιχείο είναι προσαρμοσμένο (προστεθειμένο από τους συγγραφείς του εγγράφου). |
|
|  | [setCustom(boolean value)](#setCustom-boolean-) | Ορίζει μια τιμή που υποδεικνύει αν αυτό το στοιχείο είναι προσαρμοσμένο (προστεθειμένο από τους συγγραφείς του εγγράφου). |
|
|  | [getDictionaryKey()](#getDictionaryKey--) | Λαμβάνει ένα κλειδί λεξικού για , χρησιμοποιώντας το OriginalName του και άλλα δεδομένα. |
|
|  | [createClone()](#createClone--) | Δημιουργεί ένα βαθύ αντίγραφο της τρέχουσας παρουσίας. |
|
|  | [getActualValue()](#getActualValue--) | Λαμβάνει την αναπαράσταση συμβολοσειράς της τιμής του στοιχείου μεταδεδομένων. |
|
### MetadataItem() {#MetadataItem--}
```
public MetadataItem()
```


Αρχικοποιεί μια νέα παρουσία.


### getOriginalName() {#getOriginalName--}
```
public final String getOriginalName()
```


Λαμβάνει το αρχικό όνομα του στοιχείου μεταδεδομένων, όπως εμφανίζεται στο έγγραφο.


**Returns:**
java.lang.String - Ένα αρχικό όνομα του στοιχείου μεταδεδομένων, όπως εμφανίζεται στο έγγραφο.

### setOriginalName(String value) {#setOriginalName-java.lang.String-}
```
public final void setOriginalName(String value)
```


Ορίζει το αρχικό όνομα του στοιχείου μεταδεδομένων, όπως εμφανίζεται στο έγγραφο.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | τιμή | java.lang.String | Ένα αρχικό όνομα του στοιχείου μεταδεδομένων, όπως εμφανίζεται στο έγγραφο. |
|

### getCategory() {#getCategory--}
```
public final String getCategory()
```


Λαμβάνει μια κατηγορία του στοιχείου μεταδεδομένων, για παράδειγμα το αναγνωριστικό πόρου για ένα ενσωματωμένο στοιχείο μεταδεδομένων πόρου.


**Returns:**
java.lang.String - Μια κατηγορία του στοιχείου μεταδεδομένων, για παράδειγμα το αναγνωριστικό πόρου για ένα ενσωματωμένο στοιχείο μεταδεδομένων.

### setCategory(String value) {#setCategory-java.lang.String-}
```
public final void setCategory(String value)
```


Ορίζει μια κατηγορία του στοιχείου μεταδεδομένων, για παράδειγμα το αναγνωριστικό πόρου για ένα ενσωματωμένο στοιχείο μεταδεδομένων.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | τιμή | java.lang.String | Μια κατηγορία του στοιχείου μεταδεδομένων, για παράδειγμα το αναγνωριστικό πόρου για ένα ενσωματωμένο στοιχείο μεταδεδομένων. |
|

### getFilter() {#getFilter--}
```
public final int getFilter()
```


Λαμβάνει μια τιμή του
MetadataFilters
, που ανατίθεται σε αυτό το στοιχείο μεταδεδομένων και χρησιμοποιείται στο φιλτράρισμα των στοιχείων.


**Returns:**
int - Μια τιμή του  MetadataFilters , που ανατίθεται σε αυτό το στοιχείο μεταδεδομένων και χρησιμοποιείται στο φιλτράρισμα των στοιχείων.

### setFilter(int value) {#setFilter-int-}
```
public final void setFilter(int value)
```


Ορίζει μια τιμή του
MetadataFilters
, που ανατίθεται σε αυτό το στοιχείο μεταδεδομένων και χρησιμοποιείται στο φιλτράρισμα των στοιχείων.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | τιμή | int | Μια τιμή του  MetadataFilters , που ανατίθεται σε αυτό το στοιχείο μεταδεδομένων και χρησιμοποιείται στο φιλτράρισμα των στοιχείων. |
|

### getValues() {#getValues--}
```
public final List<String> getValues()
```


Λαμβάνει την τιμή του στοιχείου μεταδεδομένων.


**Returns:**
java.util.List<java.lang.String> - Η τιμή του στοιχείου μεταδεδομένων.

### setValues(List<String> value) {#setValues-java.util.List-java.lang.String--}
```
public final void setValues(List<String> value)
```


Ορίζει την τιμή του στοιχείου μεταδεδομένων.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | τιμή | java.util.List<java.lang.String> | Η τιμή του στοιχείου μεταδεδομένων. |
|

### isCustom() {#isCustom--}
```
public final boolean isCustom()
```


Λαμβάνει μια τιμή που υποδεικνύει αν αυτό το στοιχείο είναι προσαρμοσμένο (προστεθειμένο από τους συγγραφείς του εγγράφου).


**Returns:**
boolean - Μια τιμή που υποδεικνύει αν αυτό το στοιχείο είναι προσαρμοσμένο (προστεθειμένο από τους συγγραφείς του εγγράφου).

### setCustom(boolean value) {#setCustom-boolean-}
```
public final void setCustom(boolean value)
```


Ορίζει μια τιμή που υποδεικνύει αν αυτό το στοιχείο είναι προσαρμοσμένο (προστεθειμένο από τους συγγραφείς του εγγράφου).


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | τιμή | boolean | Μια τιμή που υποδεικνύει αν αυτό το στοιχείο είναι προσαρμοσμένο (προστεθειμένο από τους συγγραφείς του εγγράφου). |
|

### getDictionaryKey() {#getDictionaryKey--}
```
public String getDictionaryKey()
```


Λαμβάνει ένα κλειδί λεξικού για , χρησιμοποιώντας το OriginalName του και άλλα δεδομένα.


**Returns:**
java.lang.String - Ένα κλειδί λεξικού για , χρησιμοποιώντας το OriginalName του και άλλα δεδομένα.

### createClone() {#createClone--}
```
public MetadataItem createClone()
```


Δημιουργεί ένα βαθύ αντίγραφο της τρέχουσας παρουσίας.


**Returns:**
[MetadataItem](../../com.groupdocs.redaction.integration/metadataitem) - Object clone

### getActualValue() {#getActualValue--}
```
public final String getActualValue()
```


Λαμβάνει την αναπαράσταση συμβολοσειράς της τιμής του στοιχείου μεταδεδομένων.


**Returns:**
java.lang.String - Η αναπαράσταση συμβολοσειράς της τιμής του στοιχείου μεταδεδομένων.

