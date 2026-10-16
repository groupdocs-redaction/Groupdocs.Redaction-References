---
title: "RedactorLogEntry"
second_title: "GroupDocs.Redaction για Java API Αναφορά"
description: "Αντιπροσωπεύει τα αποτελέσματα της εφαρμογής της απόκρυψης."
type: docs
weight: 18
url: /el/java/com.groupdocs.redaction/redactorlogentry/
---
**Inheritance:**
java.lang.Object
```
public class RedactorLogEntry
```

Αντιπροσωπεύει τα αποτελέσματα της εφαρμογής της απόκρυψης.

*** ** * ** ***


**Learn more**

* More details about redaction log entries: [Redaction basics](../https://docs.groupdocs.com/redaction/java/redaction-basics/)

<br />


## Κατασκευαστές

| Κατασκευαστής | Περιγραφή |
| --- | --- |
|  | [RedactorLogEntry(Redaction redaction, RedactionResult result)](#RedactorLogEntry-com.groupdocs.redaction.Redaction-com.groupdocs.redaction.RedactionResult-) | Αρχικοποιεί μια νέα παρουσία της κλάσης RedactorLogEntry για διαγραφή. |
|
## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
|  | [getResult()](#getResult--) | Λαμβάνει το αποτέλεσμα, που επιστρέφεται από |
GroupDocs.Redaction.Integration.DocumentFormatInstance
.
|
|  | [getRedaction()](#getRedaction--) | Λαμβάνει την αναφορά στην επεξεργασία και τις επιλογές της. |
|
### RedactorLogEntry(Redaction redaction, RedactionResult result) {#RedactorLogEntry-com.groupdocs.redaction.Redaction-com.groupdocs.redaction.RedactionResult-}
```
public RedactorLogEntry(Redaction redaction, RedactionResult result)
```


Αρχικοποιεί μια νέα παρουσία της κλάσης RedactorLogEntry για διαγραφή.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | redaction | [Redaction](../../com.groupdocs.redaction/redaction) | Αναφορά στην επεξεργασία |
|
|  | result | [RedactionResult](../../com.groupdocs.redaction/redactionresult) | Αποτέλεσμα επεξεργασίας, αναφέρεται από τον διαχειριστή μορφής |
|

### getResult() {#getResult--}
```
public final RedactionResult getResult()
```


Λαμβάνει το αποτέλεσμα, που επιστρέφεται από
GroupDocs.Redaction.Integration.DocumentFormatInstance
.


**Returns:**
[RedactionResult](../../com.groupdocs.redaction/redactionresult) - The result, returned by  GroupDocs.Redaction.Integration.DocumentFormatInstance .

### getRedaction() {#getRedaction--}
```
public final Redaction getRedaction()
```


Λαμβάνει την αναφορά στην επεξεργασία και τις επιλογές της.


**Returns:**
[Redaction](../../com.groupdocs.redaction/redaction) - The reference to redaction and its options.

