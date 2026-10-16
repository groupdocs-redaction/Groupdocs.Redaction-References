---
title: "RedactionPolicy"
second_title: "GroupDocs.Redaction för Java API-referens"
description: "Representerar en saneringspolicy som innehåller en uppsättning specifika redigeringar att tillämpa."
type: docs
weight: 14
url: /sv/java/com.groupdocs.redaction/redactionpolicy/
---
**Inheritance:**
java.lang.Object
```
public class RedactionPolicy
```

Representerar en saneringspolicy som innehåller en uppsättning specifika raderingar att tillämpa.

*** ** * ** ***


**Learn more**

* More details about policies: [Use of redaction policies](../https://docs.groupdocs.com/redaction/java/use-redaction-policies/)
* More details about applying redactions: [Redaction basics](../https://docs.groupdocs.com/redaction/java/redaction-basics/)

<br />


## Konstruktörer

| Konstruktor | Beskrivning |
| --- | --- |
|  | [RedactionPolicy()](#RedactionPolicy--) | Skapar en ny instans av Redaction policy. |
|
|  | [RedactionPolicy(Redaction[] redactions)](#RedactionPolicy-com.groupdocs.redaction.Redaction---) | Skapar en ny instans av Redaction policy med en specifik lista över redigeringar. |
|
## Metoder

| Metod | Beskrivning |
| --- | --- |
|  | [getRedactions()](#getRedactions--) | Hämtar en array av fullt konfigurerade |
Redigering
-derived classes.
|
|  | [load(String filePath)](#load-java.lang.String-) | Laddar en instans av |
RedactionPolicy
från en filsökväg.
|
|  | [load(InputStream input)](#load-java.io.InputStream-) | Laddar en instans av |
RedactionPolicy
från en ström.
|
|  | [save(String filePath)](#save-java.lang.String-) | Sparar redaction policy till en fil. |
|
|  | [save(OutputStream output)](#save-java.io.OutputStream-) | Sparar redaction policy till en ström. |
|
### RedactionPolicy() {#RedactionPolicy--}
```
public RedactionPolicy()
```


Skapar en ny instans av Redaction policy.


### RedactionPolicy(Redaction[] redactions) {#RedactionPolicy-com.groupdocs.redaction.Redaction---}
```
public RedactionPolicy(Redaction[] redactions)
```


Skapar en ny instans av Redaction policy med en specifik lista över redigeringar.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | redactions | [Redaction\[\]](../../com.groupdocs.redaction/redaction) | En array av redigeringar för policyn |
|

### getRedactions() {#getRedactions--}
```
public final Redaction[] getRedactions()
```


Hämtar en array av fullt konfigurerade
Redigering
-derived classes.


**Returns:**
com.groupdocs.redaction.Redaction[] - En array av fullt konfigurerade Redaction‑avledda klasser.

### load(String filePath) {#load-java.lang.String-}
```
public static RedactionPolicy load(String filePath)
```


Laddar en instans av
RedactionPolicy
från en filsökväg.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | filePath | java.lang.String | Sökväg till XML‑fil |
|

**Returns:**
[RedactionPolicy](../../com.groupdocs.redaction/redactionpolicy) - Redaction policy

### load(InputStream input) {#load-java.io.InputStream-}
```
public static RedactionPolicy load(InputStream input)
```


Laddar en instans av
RedactionPolicy
från en ström.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | input | java.io.InputStream | Ström som innehåller XML‑konfiguration |
|

**Returns:**
[RedactionPolicy](../../com.groupdocs.redaction/redactionpolicy) - Redaction policy

### save(String filePath) {#save-java.lang.String-}
```
public final void save(String filePath)
```


Sparar redaction policy till en fil.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | filePath | java.lang.String | Sökväg till fil. |
|

### save(OutputStream output) {#save-java.io.OutputStream-}
```
public final void save(OutputStream output)
```


Sparar redaction policy till en ström.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | output | java.io.OutputStream | Målsström för att spara policyn |
|

