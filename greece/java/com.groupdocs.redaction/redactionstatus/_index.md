---
title: "RedactionStatus"
second_title: "GroupDocs.Redaction για Java API Αναφορά"
description: "Αντιπροσωπεύει μια κατάσταση ολοκλήρωσης απόκρυψης."
type: docs
weight: 20
url: /el/java/com.groupdocs.redaction/redactionstatus/
---
**Inheritance:**
java.lang.Object, java.lang.Enum
```
public enum RedactionStatus extends Enum<RedactionStatus>
```

Αντιπροσωπεύει μια κατάσταση ολοκλήρωσης απόκρυψης.

## Πεδία

| Πεδίο | Περιγραφή |
| --- | --- |
|  | [Applied](#Applied) | Η διαγραφή εφαρμόστηκε πλήρως και επιτυχώς. |
|
|  | [PartiallyApplied](#PartiallyApplied) | Η διαγραφή εφαρμόστηκε μόνο σε μέρος των αντιστοιχίσεων της. |
|
|  | [Skipped](#Skipped) | Η διαγραφή παραλήφθηκε (δεν εφαρμόστηκε). |
|
|  | [Failed](#Failed) | Η διαγραφή απέτυχε με εξαίρεση. |
|
## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
| [values()](#values--) |  |
| [valueOf(String name)](#valueOf-java.lang.String-) |  |
### Applied {#Applied}
```
public static final RedactionStatus Applied
```


Η διαγραφή εφαρμόστηκε πλήρως και επιτυχώς.


### PartiallyApplied {#PartiallyApplied}
```
public static final RedactionStatus PartiallyApplied
```


Η διαγραφή εφαρμόστηκε μόνο σε μέρος των αντιστοιχίσεων της.


### Skipped {#Skipped}
```
public static final RedactionStatus Skipped
```


Η διαγραφή παραλήφθηκε (δεν εφαρμόστηκε).


### Failed {#Failed}
```
public static final RedactionStatus Failed
```


Η διαγραφή απέτυχε με εξαίρεση.


### values() {#values--}
```
public static RedactionStatus[] values()
```




**Returns:**
com.groupdocs.redaction.RedactionStatus[]
### valueOf(String name) {#valueOf-java.lang.String-}
```
public static RedactionStatus valueOf(String name)
```




**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| όνομα | java.lang.String |  |

**Returns:**
[RedactionStatus](../../com.groupdocs.redaction/redactionstatus)
