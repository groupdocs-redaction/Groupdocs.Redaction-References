---
title: "RedactorChangeLog"
second_title: "Referensi API GroupDocs.Redaction untuk Java"
description: "Mewakili hasil untuk daftar redaksi yang diteruskan ke metode Apply dari kelas Redactor."
type: docs
weight: 17
url: /id/java/com.groupdocs.redaction/redactorchangelog/
---
**Inheritance:**
java.lang.Object
```
public class RedactorChangeLog
```

Mewakili hasil untuk daftar redaksi, yang diteruskan ke metode Apply() dari
Redactor
kelas.

*** ** * ** ***


**Learn more**

* More details about redaction logs: [Redaction basics](../https://docs.groupdocs.com/redaction/java/redaction-basics/)

<br />


## Konstruktor

| Konstruktor | Deskripsi |
| --- | --- |
|  | [RedactorChangeLog()](#RedactorChangeLog--) | Menginisialisasi instance baru dari kelas RedactorChangeLog. |
|
## Metode

| Metode | Deskripsi |
| --- | --- |
|  | [getStatus()](#getStatus--) | Mendapatkan status akhir dari semua redaksi yang diterapkan. |
|
|  | [getRedactionLog()](#getRedactionLog--) | Mendapatkan daftar |
RedactorLogEntry
instansi.
|
### RedactorChangeLog() {#RedactorChangeLog--}
```
public RedactorChangeLog()
```


Menginisialisasi instance baru dari kelas RedactorChangeLog.


### getStatus() {#getStatus--}
```
public final RedactionStatus getStatus()
```


Mendapatkan status akhir dari semua redaksi yang diterapkan.


**Returns:**
[RedactionStatus](../../com.groupdocs.redaction/redactionstatus) - The final status of all applied redactions.

### getRedactionLog() {#getRedactionLog--}
```
public final List<RedactorLogEntry> getRedactionLog()
```


Mendapatkan daftar
RedactorLogEntry
instansi.


**Returns:**
java.util.List<com.groupdocs.redaction.RedactorLogEntry> - Daftar instansi RedactorLogEntry.

