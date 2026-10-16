---
title: "RedactionActionType"
second_title: "GroupDocs.Redaction για Java API Αναφορά"
description: "Αντιπροσωπεύει ενέργειες που μπορούν να ληφθούν για την εκτέλεση διαγραφής."
type: docs
weight: 37
url: /el/java/com.groupdocs.redaction.redactions/redactionactiontype/
---
**Inheritance:**
java.lang.Object, java.lang.Enum
```
public enum RedactionActionType extends Enum<RedactionActionType>
```

Αντιπροσωπεύει ενέργειες που μπορούν να ληφθούν για την εκτέλεση διαγραφής.

## Πεδία

| Πεδίο | Περιγραφή |
| --- | --- |
|  | [Replacement](#Replacement) | Το κείμενο που έχει επεξεργαστεί αντικαταστάθηκε με άλλο ή καλύφθηκε με ένα μπλοκ. |
|
|  | [Cleanup](#Cleanup) | Τα δεδομένα αφαιρέθηκαν, αλλά ένα κενό αντικείμενο παραμένει στο έγγραφο. |
|
|  | [Deletion](#Deletion) | Τα δεδομένα και οι σχετικές δομές αφαιρέθηκαν από το έγγραφο. |
|
## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
| [values()](#values--) |  |
| [valueOf(String name)](#valueOf-java.lang.String-) |  |
### Replacement {#Replacement}
```
public static final RedactionActionType Replacement
```


Το κείμενο που έχει επεξεργαστεί αντικαταστάθηκε με άλλο ή καλύφθηκε με ένα μπλοκ.


### Cleanup {#Cleanup}
```
public static final RedactionActionType Cleanup
```


Τα δεδομένα αφαιρέθηκαν, αλλά ένα κενό αντικείμενο παραμένει στο έγγραφο.


### Deletion {#Deletion}
```
public static final RedactionActionType Deletion
```


Τα δεδομένα και οι σχετικές δομές αφαιρέθηκαν από το έγγραφο.


### values() {#values--}
```
public static RedactionActionType[] values()
```




**Returns:**
com.groupdocs.redaction.redactions.RedactionActionType[]
### valueOf(String name) {#valueOf-java.lang.String-}
```
public static RedactionActionType valueOf(String name)
```




**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| όνομα | java.lang.String |  |

**Returns:**
[RedactionActionType](../../com.groupdocs.redaction.redactions/redactionactiontype)
