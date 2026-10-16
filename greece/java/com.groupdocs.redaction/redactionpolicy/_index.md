---
title: "RedactionPolicy"
second_title: "GroupDocs.Redaction για Java API Αναφορά"
description: "Αντιπροσωπεύει μια πολιτική εξαγνισμού που περιέχει ένα σύνολο συγκεκριμένων διαγραφών προς εφαρμογή."
type: docs
weight: 14
url: /el/java/com.groupdocs.redaction/redactionpolicy/
---
**Inheritance:**
java.lang.Object
```
public class RedactionPolicy
```

Αντιπροσωπεύει μια πολιτική εξαγνισμού, η οποία περιέχει ένα σύνολο συγκεκριμένων αποκρύψεων προς εφαρμογή.

*** ** * ** ***


**Learn more**

* More details about policies: [Use of redaction policies](../https://docs.groupdocs.com/redaction/java/use-redaction-policies/)
* More details about applying redactions: [Redaction basics](../https://docs.groupdocs.com/redaction/java/redaction-basics/)

<br />


## Κατασκευαστές

| Κατασκευαστής | Περιγραφή |
| --- | --- |
|  | [RedactionPolicy()](#RedactionPolicy--) | Δημιουργεί μια νέα παρουσία της πολιτικής Redaction. |
|
|  | [RedactionPolicy(Redaction[] redactions)](#RedactionPolicy-com.groupdocs.redaction.Redaction---) | Δημιουργεί μια νέα παρουσία της πολιτικής Redaction με έναν συγκεκριμένο κατάλογο διαγραφών. |
|
## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
|  | [getRedactions()](#getRedactions--) | Λαμβάνει έναν πίνακα πλήρως διαμορφωμένων |
Διαγραφή
-derived classes.
|
|  | [load(String filePath)](#load-java.lang.String-) | Φορτώνει μια παρουσία του |
RedactionPolicy
από διαδρομή αρχείου.
|
|  | [load(InputStream input)](#load-java.io.InputStream-) | Φορτώνει μια παρουσία του |
RedactionPolicy
από ροή.
|
|  | [save(String filePath)](#save-java.lang.String-) | Αποθηκεύει την πολιτική redaction σε ένα αρχείο. |
|
|  | [save(OutputStream output)](#save-java.io.OutputStream-) | Αποθηκεύει την πολιτική redaction σε μια ροή. |
|
### RedactionPolicy() {#RedactionPolicy--}
```
public RedactionPolicy()
```


Δημιουργεί μια νέα παρουσία της πολιτικής Redaction.


### RedactionPolicy(Redaction[] redactions) {#RedactionPolicy-com.groupdocs.redaction.Redaction---}
```
public RedactionPolicy(Redaction[] redactions)
```


Δημιουργεί μια νέα παρουσία της πολιτικής Redaction με έναν συγκεκριμένο κατάλογο διαγραφών.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | redactions | [Redaction\[\]](../../com.groupdocs.redaction/redaction) | Ένας πίνακας διαγραφών για την πολιτική |
|

### getRedactions() {#getRedactions--}
```
public final Redaction[] getRedactions()
```


Λαμβάνει έναν πίνακα πλήρως διαμορφωμένων
Διαγραφή
-derived classes.


**Returns:**
com.groupdocs.redaction.Redaction[] - Ένας πίνακας πλήρως διαμορφωμένων κλάσεων που προέρχονται από Redaction.

### load(String filePath) {#load-java.lang.String-}
```
public static RedactionPolicy load(String filePath)
```


Φορτώνει μια παρουσία του
RedactionPolicy
από διαδρομή αρχείου.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | filePath | java.lang.String | Διαδρομή προς το αρχείο XML |
|

**Returns:**
[RedactionPolicy](../../com.groupdocs.redaction/redactionpolicy) - Redaction policy

### load(InputStream input) {#load-java.io.InputStream-}
```
public static RedactionPolicy load(InputStream input)
```


Φορτώνει μια παρουσία του
RedactionPolicy
από ροή.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | είσοδος | java.io.InputStream | Ροή που περιέχει τη διαμόρφωση XML |
|

**Returns:**
[RedactionPolicy](../../com.groupdocs.redaction/redactionpolicy) - Redaction policy

### save(String filePath) {#save-java.lang.String-}
```
public final void save(String filePath)
```


Αποθηκεύει την πολιτική redaction σε ένα αρχείο.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | filePath | java.lang.String | Διαδρομή προς το αρχείο. |
|

### save(OutputStream output) {#save-java.io.OutputStream-}
```
public final void save(OutputStream output)
```


Αποθηκεύει την πολιτική redaction σε μια ροή.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | έξοδος | java.io.OutputStream | Στόχος ροής για αποθήκευση της πολιτικής |
|

