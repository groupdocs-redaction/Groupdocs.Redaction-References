---
title: "RedactorChangeLog"
second_title: "Referencia de la API de GroupDocs.Redaction para Java"
description: "Representa los resultados para una lista de redactados pasados al método Apply de la clase Redactor."
type: docs
weight: 17
url: /es/java/com.groupdocs.redaction/redactorchangelog/
---
**Inheritance:**
java.lang.Object
```
public class RedactorChangeLog
```

Representa los resultados para una lista de redactados, pasados al método Apply() de
Redactor
clase.

*** ** * ** ***


**Learn more**

* More details about redaction logs: [Redaction basics](../https://docs.groupdocs.com/redaction/java/redaction-basics/)

<br />


## Constructores

| Constructor | Descripción |
| --- | --- |
|  | [RedactorChangeLog()](#RedactorChangeLog--) | Inicializa una nueva instancia de la clase RedactorChangeLog. |
|
## Métodos

| Método | Descripción |
| --- | --- |
|  | [getStatus()](#getStatus--) | Obtiene el estado final de todas las redacciones aplicadas. |
|
|  | [getRedactionLog()](#getRedactionLog--) | Obtiene la lista de |
RedactorLogEntry
instancias.
|
### RedactorChangeLog() {#RedactorChangeLog--}
```
public RedactorChangeLog()
```


Inicializa una nueva instancia de la clase RedactorChangeLog.


### getStatus() {#getStatus--}
```
public final RedactionStatus getStatus()
```


Obtiene el estado final de todas las redacciones aplicadas.


**Returns:**
[RedactionStatus](../../com.groupdocs.redaction/redactionstatus) - The final status of all applied redactions.

### getRedactionLog() {#getRedactionLog--}
```
public final List<RedactorLogEntry> getRedactionLog()
```


Obtiene la lista de
RedactorLogEntry
instancias.


**Returns:**
java.util.List<com.groupdocs.redaction.RedactorLogEntry> - La lista de instancias de RedactorLogEntry.

