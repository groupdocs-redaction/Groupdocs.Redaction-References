---
title: "RedactionPolicy"
second_title: "GroupDocs.Redaction for Java API-referentie"
description: "Stelt een sanitatiebeleid voor dat een reeks specifieke redacties bevat die moeten worden toegepast."
type: docs
weight: 14
url: /nl/java/com.groupdocs.redaction/redactionpolicy/
---
**Inheritance:**
java.lang.Object
```
public class RedactionPolicy
```

Stelt een sanitatiebeleid voor, dat een reeks specifieke redacties bevat die moeten worden toegepast.

*** ** * ** ***


**Learn more**

* More details about policies: [Use of redaction policies](../https://docs.groupdocs.com/redaction/java/use-redaction-policies/)
* More details about applying redactions: [Redaction basics](../https://docs.groupdocs.com/redaction/java/redaction-basics/)

<br />


## Constructors

| Constructor | Beschrijving |
| --- | --- |
|  | [RedactionPolicy()](#RedactionPolicy--) | Maakt een nieuw exemplaar van Redaction policy aan. |
|
|  | [RedactionPolicy(Redaction[] redactions)](#RedactionPolicy-com.groupdocs.redaction.Redaction---) | Maakt een nieuw exemplaar van Redaction policy met een specifieke lijst van redacties aan. |
|
## Methoden

| Methode | Beschrijving |
| --- | --- |
|  | [getRedactions()](#getRedactions--) | Haalt een array op van volledig geconfigureerde |
Redaction
-derived classes.
|
|  | [load(String filePath)](#load-java.lang.String-) | Laadt een exemplaar van |
RedactionPolicy
van een bestandspad.
|
|  | [load(InputStream input)](#load-java.io.InputStream-) | Laadt een exemplaar van |
RedactionPolicy
van een stream.
|
|  | [save(String filePath)](#save-java.lang.String-) | Slaat het redaction policy op naar een bestand. |
|
|  | [save(OutputStream output)](#save-java.io.OutputStream-) | Slaat het redaction policy op naar een stream. |
|
### RedactionPolicy() {#RedactionPolicy--}
```
public RedactionPolicy()
```


Maakt een nieuw exemplaar van Redaction policy aan.


### RedactionPolicy(Redaction[] redactions) {#RedactionPolicy-com.groupdocs.redaction.Redaction---}
```
public RedactionPolicy(Redaction[] redactions)
```


Maakt een nieuw exemplaar van Redaction policy met een specifieke lijst van redacties aan.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | redactions | [Redaction\[\]](../../com.groupdocs.redaction/redaction) | Een array van redacties voor het beleid |
|

### getRedactions() {#getRedactions--}
```
public final Redaction[] getRedactions()
```


Haalt een array op van volledig geconfigureerde
Redaction
-derived classes.


**Returns:**
com.groupdocs.redaction.Redaction[] - Een array van volledig geconfigureerde Redaction-afgeleide klassen.

### load(String filePath) {#load-java.lang.String-}
```
public static RedactionPolicy load(String filePath)
```


Laadt een exemplaar van
RedactionPolicy
van een bestandspad.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | filePath | java.lang.String | Pad naar XML-bestand |
|

**Returns:**
[RedactionPolicy](../../com.groupdocs.redaction/redactionpolicy) - Redaction policy

### load(InputStream input) {#load-java.io.InputStream-}
```
public static RedactionPolicy load(InputStream input)
```


Laadt een exemplaar van
RedactionPolicy
van een stream.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | input | java.io.InputStream | Stream met XML-configuratie |
|

**Returns:**
[RedactionPolicy](../../com.groupdocs.redaction/redactionpolicy) - Redaction policy

### save(String filePath) {#save-java.lang.String-}
```
public final void save(String filePath)
```


Slaat het redaction policy op naar een bestand.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | filePath | java.lang.String | Pad naar bestand. |
|

### save(OutputStream output) {#save-java.io.OutputStream-}
```
public final void save(OutputStream output)
```


Slaat het redaction policy op naar een stream.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | output | java.io.OutputStream | Doelstream om het beleid op te slaan |
|

