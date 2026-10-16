---
title: "RedactionResult"
second_title: "GroupDocs.Redaction για Java API Αναφορά"
description: "Αντιπροσωπεύει το αποτέλεσμα της λειτουργίας απόκρυψης."
type: docs
weight: 15
url: /el/java/com.groupdocs.redaction/redactionresult/
---
**Inheritance:**
java.lang.Object
```
public class RedactionResult
```

Αντιπροσωπεύει το αποτέλεσμα της λειτουργίας απόκρυψης.

*** ** * ** ***


**Learn more**

* More details about redaction results: [Redaction basics](../https://docs.groupdocs.com/redaction/java/redaction-basics/)

<br />


## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
|  | [getStatus()](#getStatus--) | Λαμβάνει την κατάσταση εκτέλεσης. |
|
|  | [getErrorMessage()](#getErrorMessage--) | Λαμβάνει το μήνυμα σφάλματος για διαγνωστικούς σκοπούς. |
|
|  | [skipped(String description)](#skipped-java.lang.String-) | Αρχικοποιεί ένα νέο αντικείμενο της κλάσης RedactionResult με κατάσταση Skipped. |
|
|  | [partial(String description)](#partial-java.lang.String-) | Αρχικοποιεί ένα νέο αντικείμενο της κλάσης RedactionResult με κατάσταση PartiallyApplied. |
|
|  | [failed(String description)](#failed-java.lang.String-) | Αρχικοποιεί ένα νέο αντικείμενο της κλάσης RedactionResult με κατάσταση Failed. |
|
|  | [successful()](#successful--) | Αρχικοποιεί ένα νέο αντικείμενο της κλάσης RedactionResult με κατάσταση Applied (επιτυχής). |
|
### getStatus() {#getStatus--}
```
public final RedactionStatus getStatus()
```


Λαμβάνει την κατάσταση εκτέλεσης.


**Returns:**
[RedactionStatus](../../com.groupdocs.redaction/redactionstatus) - The execution status.

### getErrorMessage() {#getErrorMessage--}
```
public final String getErrorMessage()
```


Λαμβάνει το μήνυμα σφάλματος για διαγνωστικούς σκοπούς.


**Returns:**
java.lang.String - Το μήνυμα σφάλματος για διαγνωστικούς σκοπούς.

### skipped(String description) {#skipped-java.lang.String-}
```
public static RedactionResult skipped(String description)
```


Αρχικοποιεί ένα νέο αντικείμενο της κλάσης RedactionResult με κατάσταση Skipped.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | περιγραφή | java.lang.String | Αιτία για την παράλειψη της λειτουργίας |
|

**Returns:**
[RedactionResult](../../com.groupdocs.redaction/redactionresult) - Sskipped redaction result

### partial(String description) {#partial-java.lang.String-}
```
public static RedactionResult partial(String description)
```


Αρχικοποιεί ένα νέο αντικείμενο της κλάσης RedactionResult με κατάσταση PartiallyApplied.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | περιγραφή | java.lang.String | Αιτία για το ότι η λειτουργία δεν εφαρμόστηκε πλήρως |
|

**Returns:**
[RedactionResult](../../com.groupdocs.redaction/redactionresult) - Partially applied redaction result

### failed(String description) {#failed-java.lang.String-}
```
public static RedactionResult failed(String description)
```


Αρχικοποιεί ένα νέο αντικείμενο της κλάσης RedactionResult με κατάσταση Failed.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | περιγραφή | java.lang.String | Λεπτομέρειες αποτυχίας ή εξαίρεσης |
|

**Returns:**
[RedactionResult](../../com.groupdocs.redaction/redactionresult) - Failed redaction result

### successful() {#successful--}
```
public static RedactionResult successful()
```


Αρχικοποιεί ένα νέο αντικείμενο της κλάσης RedactionResult με κατάσταση Applied (επιτυχής).


**Returns:**
[RedactionResult](../../com.groupdocs.redaction/redactionresult) - Successful redaction result

