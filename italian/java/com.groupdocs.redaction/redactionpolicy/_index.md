---
title: "RedactionPolicy"
second_title: "GroupDocs.Redaction per Java Riferimento API"
description: "Rappresenta una politica di sanitizzazione contenente un insieme di redazioni specifiche da applicare."
type: docs
weight: 14
url: /it/java/com.groupdocs.redaction/redactionpolicy/
---
**Inheritance:**
java.lang.Object
```
public class RedactionPolicy
```

Rappresenta una politica di sanificazione, contenente un insieme di redazioni specifiche da applicare.

*** ** * ** ***


**Learn more**

* More details about policies: [Use of redaction policies](../https://docs.groupdocs.com/redaction/java/use-redaction-policies/)
* More details about applying redactions: [Redaction basics](../https://docs.groupdocs.com/redaction/java/redaction-basics/)

<br />


## Costruttori

| Costruttore | Descrizione |
| --- | --- |
|  | [RedactionPolicy()](#RedactionPolicy--) | Crea una nuova istanza di Redaction policy. |
|
|  | [RedactionPolicy(Redaction[] redactions)](#RedactionPolicy-com.groupdocs.redaction.Redaction---) | Crea una nuova istanza di Redaction policy con un elenco specifico di redazioni. |
|
## Metodi

| Metodo | Descrizione |
| --- | --- |
|  | [getRedactions()](#getRedactions--) | Ottiene un array completamente configurato |
Redaction
-derived classes.
|
|  | [load(String filePath)](#load-java.lang.String-) | Carica un'istanza di |
RedactionPolicy
da un percorso file.
|
|  | [load(InputStream input)](#load-java.io.InputStream-) | Carica un'istanza di |
RedactionPolicy
da un flusso.
|
|  | [save(String filePath)](#save-java.lang.String-) | Salva la politica di redaction in un file. |
|
|  | [save(OutputStream output)](#save-java.io.OutputStream-) | Salva la politica di redaction in un flusso. |
|
### RedactionPolicy() {#RedactionPolicy--}
```
public RedactionPolicy()
```


Crea una nuova istanza di Redaction policy.


### RedactionPolicy(Redaction[] redactions) {#RedactionPolicy-com.groupdocs.redaction.Redaction---}
```
public RedactionPolicy(Redaction[] redactions)
```


Crea una nuova istanza di Redaction policy con un elenco specifico di redazioni.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | redactions | [Redaction\[\]](../../com.groupdocs.redaction/redaction) | Un array di redazioni per la politica |
|

### getRedactions() {#getRedactions--}
```
public final Redaction[] getRedactions()
```


Ottiene un array completamente configurato
Redaction
-derived classes.


**Returns:**
com.groupdocs.redaction.Redaction[] - Un array di classi derivate da Redaction completamente configurate.

### load(String filePath) {#load-java.lang.String-}
```
public static RedactionPolicy load(String filePath)
```


Carica un'istanza di
RedactionPolicy
da un percorso file.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | filePath | java.lang.String | Percorso al file XML |
|

**Returns:**
[RedactionPolicy](../../com.groupdocs.redaction/redactionpolicy) - Redaction policy

### load(InputStream input) {#load-java.io.InputStream-}
```
public static RedactionPolicy load(InputStream input)
```


Carica un'istanza di
RedactionPolicy
da un flusso.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | input | java.io.InputStream | Flusso contenente la configurazione XML |
|

**Returns:**
[RedactionPolicy](../../com.groupdocs.redaction/redactionpolicy) - Redaction policy

### save(String filePath) {#save-java.lang.String-}
```
public final void save(String filePath)
```


Salva la politica di redaction in un file.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | filePath | java.lang.String | Percorso al file. |
|

### save(OutputStream output) {#save-java.io.OutputStream-}
```
public final void save(OutputStream output)
```


Salva la politica di redaction in un flusso.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | output | java.io.OutputStream | Flusso di destinazione per salvare la politica |
|

