---
title: "RedactionPolicy"
second_title: "GroupDocs.Redaction for Java API-Referenz"
description: "Stellt eine Bereinigungspolicy dar, die eine Menge spezifischer Redaktionen enthält, die angewendet werden sollen."
type: docs
weight: 14
url: /de/java/com.groupdocs.redaction/redactionpolicy/
---
**Inheritance:**
java.lang.Object
```
public class RedactionPolicy
```

Stellt eine Bereinigungsrichtlinie dar, die einen Satz spezifischer Redaktionen enthält, die angewendet werden sollen.

*** ** * ** ***


**Learn more**

* More details about policies: [Use of redaction policies](../https://docs.groupdocs.com/redaction/java/use-redaction-policies/)
* More details about applying redactions: [Redaction basics](../https://docs.groupdocs.com/redaction/java/redaction-basics/)

<br />


## Konstruktoren

| Konstruktor | Beschreibung |
| --- | --- |
|  | [RedactionPolicy()](#RedactionPolicy--) | Erstellt eine neue Instanz der Redaction policy. |
|
|  | [RedactionPolicy(Redaction[] redactions)](#RedactionPolicy-com.groupdocs.redaction.Redaction---) | Erstellt eine neue Instanz der Redaction policy mit einer spezifischen Liste von Redaktionen. |
|
## Methoden

| Methode | Beschreibung |
| --- | --- |
|  | [getRedactions()](#getRedactions--) | Liefert ein Array vollständig konfigurierter |
Redaction
-derived classes.
|
|  | [load(String filePath)](#load-java.lang.String-) | Lädt eine Instanz von |
RedactionPolicy
aus einem Dateipfad.
|
|  | [load(InputStream input)](#load-java.io.InputStream-) | Lädt eine Instanz von |
RedactionPolicy
aus einem Stream.
|
|  | [save(String filePath)](#save-java.lang.String-) | Speichert die Redaction policy in einer Datei. |
|
|  | [save(OutputStream output)](#save-java.io.OutputStream-) | Speichert die Redaction policy in einem Stream. |
|
### RedactionPolicy() {#RedactionPolicy--}
```
public RedactionPolicy()
```


Erstellt eine neue Instanz der Redaction policy.


### RedactionPolicy(Redaction[] redactions) {#RedactionPolicy-com.groupdocs.redaction.Redaction---}
```
public RedactionPolicy(Redaction[] redactions)
```


Erstellt eine neue Instanz der Redaction policy mit einer spezifischen Liste von Redaktionen.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | redactions | [Redaction\[\]](../../com.groupdocs.redaction/redaction) | Ein Array von Redaktionen für die Policy |
|

### getRedactions() {#getRedactions--}
```
public final Redaction[] getRedactions()
```


Liefert ein Array vollständig konfigurierter
Redaction
-derived classes.


**Returns:**
com.groupdocs.redaction.Redaction[] - Ein Array vollständig konfigurierter, von Redaction abgeleiteter Klassen.

### load(String filePath) {#load-java.lang.String-}
```
public static RedactionPolicy load(String filePath)
```


Lädt eine Instanz von
RedactionPolicy
aus einem Dateipfad.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | filePath | java.lang.String | Pfad zur XML-Datei |
|

**Returns:**
[RedactionPolicy](../../com.groupdocs.redaction/redactionpolicy) - Redaction policy

### load(InputStream input) {#load-java.io.InputStream-}
```
public static RedactionPolicy load(InputStream input)
```


Lädt eine Instanz von
RedactionPolicy
aus einem Stream.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | input | java.io.InputStream | Stream, der die XML-Konfiguration enthält |
|

**Returns:**
[RedactionPolicy](../../com.groupdocs.redaction/redactionpolicy) - Redaction policy

### save(String filePath) {#save-java.lang.String-}
```
public final void save(String filePath)
```


Speichert die Redaction policy in einer Datei.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | filePath | java.lang.String | Pfad zur Datei. |
|

### save(OutputStream output) {#save-java.io.OutputStream-}
```
public final void save(OutputStream output)
```


Speichert die Redaction policy in einem Stream.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | Ausgabe | java.io.OutputStream | Ziel-Stream zum Speichern der Richtlinie |
|

