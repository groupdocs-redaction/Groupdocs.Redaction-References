---
title: "MetadataFilters"
second_title: "GroupDocs.Redaction για Java API Αναφορά"
description: "Αντιπροσωπεύει μια λίστα με τους πιο συνηθισμένους τύπους μεταδεδομένων εγγράφου."
type: docs
weight: 19
url: /el/java/com.groupdocs.redaction.redactions/metadatafilters/
---
**Inheritance:**
java.lang.Object
```
public final class MetadataFilters
```

Αντιπροσωπεύει μια λίστα με τους πιο συνηθισμένους τύπους μεταδεδομένων εγγράφου.

## Κατασκευαστές

| Κατασκευαστής | Περιγραφή |
| --- | --- |
| [MetadataFilters()](#MetadataFilters--) |  |
## Πεδία

| Πεδίο | Περιγραφή |
| --- | --- |
|  | [None](#None) | Κενή ρύθμιση φίλτρου, δεν ταιριάζει με κανένα στοιχείο μεταδεδομένων. |
|
|  | [Author](#Author) | Συγγραφέας του εγγράφου. |
|
|  | [Category](#Category) | Κατηγορία του εγγράφου. |
|
|  | [Comments](#Comments) | Σχόλιο για το έγγραφο. |
|
|  | [Company](#Company) | Εταιρεία του Συγγραφέα. |
|
|  | [ContentStatus](#ContentStatus) | Κατάσταση περιεχομένου. |
|
|  | [CreatedTime](#CreatedTime) | Ώρα δημιουργίας. |
|
|  | [HyperlinkBase](#HyperlinkBase) | Βάση υπερσυνδέσμου. |
|
|  | [LastPrinted](#LastPrinted) | Τελευταία ημερομηνία και ώρα εκτύπωσης. |
|
|  | [LastSavedBy](#LastSavedBy) | Τελευταία αποθήκευση από χρήστη. |
|
|  | [LastSavedTime](#LastSavedTime) | Τελευταία ημερομηνία και ώρα αποθήκευσης. |
|
|  | [NameOfApplication](#NameOfApplication) | Όνομα εφαρμογής όπου δημιουργήθηκε το έγγραφο. |
|
|  | [Manager](#Manager) | Όνομα διευθυντή του Συγγραφέα. |
|
|  | [RevisionNumber](#RevisionNumber) | Αριθμός αναθεώρησης. |
|
|  | [Subject](#Subject) | Θέμα του εγγράφου. |
|
|  | [Template](#Template) | Όνομα προτύπου εγγράφου. |
|
|  | [Title](#Title) | Τίτλος εγγράφου. |
|
|  | [TotalEditingTime](#TotalEditingTime) | Συνολικός χρόνος επεξεργασίας. |
|
|  | [Version](#Version) | Έκδοση εγγράφου. |
|
|  | [Description](#Description) | Περιγραφή εγγράφου. |
|
|  | [Keywords](#Keywords) | Λέξεις-κλειδιά εγγράφου. |
|
|  | [ContentType](#ContentType) | Τύπος περιεχομένου. |
|
|  | [All](#All) | Όλοι οι τύποι των στοιχείων μεταδεδομένων. |
|
## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
|  | [getNames()](#getNames--) | Λαμβάνει ένα σύνολο με όλους τους δηλωμένους τύπους φίλτρων. |
|
|  | [getValueByName(String valueName)](#getValueByName-java.lang.String-) | Λαμβάνει την τιμή του MetadataFiler με το όνομά του. |
|
|  | [parse(String values)](#parse-java.lang.String-) | Αναλύει μια συμβολοσειρά τιμών MetadataFilers διαχωρισμένων με κόμμα σε ακέραιο. |
|
|  | [toString(int value)](#toString-int-) | Αποθηκεύει έναν ακέραιο ως συμβολοσειρά τιμών MetadataFilers χωρισμένων με κόμμα. |
|
### MetadataFilters() {#MetadataFilters--}
```
public MetadataFilters()
```


### None {#None}
```
public static final int None
```


Κενή ρύθμιση φίλτρου, δεν ταιριάζει με κανένα στοιχείο μεταδεδομένων.


### Author {#Author}
```
public static final int Author
```


Συγγραφέας του εγγράφου.


### Category {#Category}
```
public static final int Category
```


Κατηγορία του εγγράφου.


### Comments {#Comments}
```
public static final int Comments
```


Σχόλιο για το έγγραφο.


### Company {#Company}
```
public static final int Company
```


Εταιρεία του Συγγραφέα.


### ContentStatus {#ContentStatus}
```
public static final int ContentStatus
```


Κατάσταση περιεχομένου.


### CreatedTime {#CreatedTime}
```
public static final int CreatedTime
```


Ώρα δημιουργίας.


### HyperlinkBase {#HyperlinkBase}
```
public static final int HyperlinkBase
```


Βάση υπερσυνδέσμου.


### LastPrinted {#LastPrinted}
```
public static final int LastPrinted
```


Τελευταία ημερομηνία και ώρα εκτύπωσης.


### LastSavedBy {#LastSavedBy}
```
public static final int LastSavedBy
```


Τελευταία αποθήκευση από χρήστη.


### LastSavedTime {#LastSavedTime}
```
public static final int LastSavedTime
```


Τελευταία ημερομηνία και ώρα αποθήκευσης.


### NameOfApplication {#NameOfApplication}
```
public static final int NameOfApplication
```


Όνομα εφαρμογής όπου δημιουργήθηκε το έγγραφο.


### Manager {#Manager}
```
public static final int Manager
```


Όνομα διευθυντή του Συγγραφέα.


### RevisionNumber {#RevisionNumber}
```
public static final int RevisionNumber
```


Αριθμός αναθεώρησης.


### Subject {#Subject}
```
public static final int Subject
```


Θέμα του εγγράφου.


### Template {#Template}
```
public static final int Template
```


Όνομα προτύπου εγγράφου.


### Title {#Title}
```
public static final int Title
```


Τίτλος εγγράφου.


### TotalEditingTime {#TotalEditingTime}
```
public static final int TotalEditingTime
```


Συνολικός χρόνος επεξεργασίας.


### Version {#Version}
```
public static final int Version
```


Έκδοση εγγράφου.


### Description {#Description}
```
public static final int Description
```


Περιγραφή εγγράφου.


### Keywords {#Keywords}
```
public static final int Keywords
```


Λέξεις-κλειδιά εγγράφου.


### ContentType {#ContentType}
```
public static final int ContentType
```


Τύπος περιεχομένου.


### All {#All}
```
public static final int All
```


Όλοι οι τύποι των στοιχείων μεταδεδομένων.


### getNames() {#getNames--}
```
public static Set<String> getNames()
```


Λαμβάνει ένα σύνολο με όλους τους δηλωμένους τύπους φίλτρων.


**Returns:**
java.util.Set<java.lang.String> - Ένα σύνολο με όλους τους δηλωμένους τύπους φίλτρων.

### getValueByName(String valueName) {#getValueByName-java.lang.String-}
```
public static int getValueByName(String valueName)
```


Λαμβάνει την τιμή του MetadataFiler με το όνομά του.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | valueName | java.lang.String | Όνομα του MetadataFilter. |
|

**Returns:**
int - Τιμή του MetadataFiler.

### parse(String values) {#parse-java.lang.String-}
```
public static int parse(String values)
```


Αναλύει μια συμβολοσειρά τιμών MetadataFilers διαχωρισμένων με κόμμα σε ακέραιο.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | values | java.lang.String | Μια συμβολοσειρά τιμών MetadataFilers χωρισμένων με κόμμα. |
|

**Returns:**
int - Τιμή των MetadataFilers.

### toString(int value) {#toString-int-}
```
public static String toString(int value)
```


Αποθηκεύει έναν ακέραιο ως συμβολοσειρά τιμών MetadataFilers χωρισμένων με κόμμα.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | τιμή | int | Τιμή του MetadataFiler. |
|

**Returns:**
java.lang.String - Μια συμβολοσειρά τιμών MetadataFiler χωρισμένων με κόμμα.

