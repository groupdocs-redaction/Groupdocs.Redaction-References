---
title: "RedactorChangeLog"
second_title: "GroupDocs.Redaction για Java API Αναφορά"
description: "Αναπαριστά τα αποτελέσματα για μια λίστα επεμβάσεων που περάστηκαν στη μέθοδο Apply της κλάσης Redactor."
type: docs
weight: 17
url: /el/java/com.groupdocs.redaction/redactorchangelog/
---
**Inheritance:**
java.lang.Object
```
public class RedactorChangeLog
```

Αναπαριστά τα αποτελέσματα για μια λίστα επεμβάσεων, που περάστηκαν στη μέθοδο Apply() της
Redactor
κλάση.

*** ** * ** ***


**Learn more**

* More details about redaction logs: [Redaction basics](../https://docs.groupdocs.com/redaction/java/redaction-basics/)

<br />


## Κατασκευαστές

| Κατασκευαστής | Περιγραφή |
| --- | --- |
|  | [RedactorChangeLog()](#RedactorChangeLog--) | Αρχικοποιεί ένα νέο στιγμιότυπο της κλάσης RedactorChangeLog. |
|
## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
|  | [getStatus()](#getStatus--) | Αποκτά την τελική κατάσταση όλων των εφαρμοσμένων επεμβάσεων. |
|
|  | [getRedactionLog()](#getRedactionLog--) | Αποκτά τη λίστα των |
RedactorLogEntry
αντιπροσωπείες.
|
### RedactorChangeLog() {#RedactorChangeLog--}
```
public RedactorChangeLog()
```


Αρχικοποιεί ένα νέο στιγμιότυπο της κλάσης RedactorChangeLog.


### getStatus() {#getStatus--}
```
public final RedactionStatus getStatus()
```


Αποκτά την τελική κατάσταση όλων των εφαρμοσμένων επεμβάσεων.


**Returns:**
[RedactionStatus](../../com.groupdocs.redaction/redactionstatus) - The final status of all applied redactions.

### getRedactionLog() {#getRedactionLog--}
```
public final List<RedactorLogEntry> getRedactionLog()
```


Αποκτά τη λίστα των
RedactorLogEntry
αντιπροσωπείες.


**Returns:**
java.util.List<com.groupdocs.redaction.RedactorLogEntry> - Η λίστα των RedactorLogEntry αντιπροσωπειών.

