---
title: "ReplacementOptions"
second_title: "GroupDocs.Redaction for Java API-Referenz"
description: "Stellt Optionen für den Austausch von übereinstimmendem Text dar."
type: docs
weight: 31
url: /de/java/com.groupdocs.redaction.redactions/replacementoptions/
---
**Inheritance:**
java.lang.Object
```
public class ReplacementOptions
```

Stellt Optionen für den Austausch von übereinstimmendem Text dar.

*** ** * ** ***


**Learn more**

* More details about document text redactions: [Text redactions](../https://docs.groupdocs.com/redaction/java/text-redactions/)
* More details about redaction filters: [Use PDF redaction filters](../https://docs.groupdocs.com/redaction/java/use-pdf-redaction-filters/)

<br />


## Konstruktoren

| Konstruktor | Beschreibung |
| --- | --- |
|  | [ReplacementOptions(String replacement)](#ReplacementOptions-java.lang.String-) | Initialisiert eine neue Instanz der Klasse ReplacementOptions mit dem Ersetzungstext als Option. |
|
|  | [ReplacementOptions(Color color)](#ReplacementOptions-java.awt.Color-) | Initialisiert eine neue Instanz der Klasse ReplacementOptions mit einem farbigen Rechteck als Option. |
|
## Methoden

| Methode | Beschreibung |
| --- | --- |
|  | [getActionType()](#getActionType--) | Liefert die Ersetzungsaktion: Box zeichnen oder Text ersetzen. |
|
|  | [getReplacement()](#getReplacement--) | Liefert den textuellen Ersetzungswert. |
|
|  | [setReplacement(String value)](#setReplacement-java.lang.String-) | Setzt den textuellen Ersetzungswert. |
|
|  | [getBoxColor()](#getBoxColor--) | Liefert die Farbe für ein |
ReplacementType.DrawBox
Option (sonst ignoriert).
|
|  | [setBoxColor(Color value)](#setBoxColor-java.awt.Color-) | Setzt die Farbe für ein |
ReplacementType.DrawBox
Option (sonst ignoriert).
|
|  | [getFilters()](#getFilters--) | Liefert ein Array von Filtern, die mit dieser Redaktion angewendet werden. |
|
|  | [setFilters(RedactionFilter[] value)](#setFilters-com.groupdocs.redaction.redactions.RedactionFilter---) | Setzt ein Array von Filtern, die mit dieser Redaktion angewendet werden. |
|
|  | [getCustomRedaction()](#getCustomRedaction--) | Liefert einen benutzerdefinierten Redaktions-Handler. |
|
|  | [setCustomRedaction(ICustomRedactionHandler value)](#setCustomRedaction-com.groupdocs.redaction.redactions.ICustomRedactionHandler-) | Setzt einen benutzerdefinierten Redaktions-Handler. |
|
| [fromFilters(RedactionFilter[] filters)](#fromFilters-com.groupdocs.redaction.redactions.RedactionFilter---) |  |
### ReplacementOptions(String replacement) {#ReplacementOptions-java.lang.String-}
```
public ReplacementOptions(String replacement)
```


Initialisiert eine neue Instanz der Klasse ReplacementOptions mit dem Ersetzungstext als Option.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | Ersetzung | java.lang.String | Textuelle Ersetzung |
|

### ReplacementOptions(Color color) {#ReplacementOptions-java.awt.Color-}
```
public ReplacementOptions(Color color)
```


Initialisiert eine neue Instanz der Klasse ReplacementOptions mit einem farbigen Rechteck als Option.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | Farbe | java.awt.Color | Rechteckfarbe |
|

### getActionType() {#getActionType--}
```
public final ReplacementType getActionType()
```


Liefert die Ersetzungsaktion: Box zeichnen oder Text ersetzen.


**Returns:**
[ReplacementType](../../com.groupdocs.redaction.redactions/replacementtype) - The replacement action: draw box or replace text.

### getReplacement() {#getReplacement--}
```
public final String getReplacement()
```


Liefert den textuellen Ersetzungswert.


**Returns:**
java.lang.String - Der textuelle Ersetzungswert.

### setReplacement(String value) {#setReplacement-java.lang.String-}
```
public final void setReplacement(String value)
```


Setzt den textuellen Ersetzungswert.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | Wert | java.lang.String | Der textuelle Ersetzungswert. |
|

### getBoxColor() {#getBoxColor--}
```
public final Color getBoxColor()
```


Liefert die Farbe für ein
ReplacementType.DrawBox
Option (sonst ignoriert).


**Returns:**
java.awt.Color - Die Farbe für eine  ReplacementType.DrawBox  Option (sonst ignoriert).

### setBoxColor(Color value) {#setBoxColor-java.awt.Color-}
```
public final void setBoxColor(Color value)
```


Setzt die Farbe für ein
ReplacementType.DrawBox
Option (sonst ignoriert).


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | Wert | java.awt.Color | Die Farbe für eine ReplacementType.DrawBox-Option (ansonsten ignoriert). |
|

### getFilters() {#getFilters--}
```
public final RedactionFilter[] getFilters()
```


Liefert ein Array von Filtern, die mit dieser Redaktion angewendet werden.


**Returns:**
com.groupdocs.redaction.redactions.RedactionFilter[] - Ein Array von Filtern, die mit dieser Redaktion angewendet werden sollen.

### setFilters(RedactionFilter[] value) {#setFilters-com.groupdocs.redaction.redactions.RedactionFilter---}
```
public final void setFilters(RedactionFilter[] value)
```


Setzt ein Array von Filtern, die mit dieser Redaktion angewendet werden.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | value | [RedactionFilter\[\]](../../com.groupdocs.redaction.redactions/redactionfilter) | Ein Array von Filtern, die mit dieser Redaktion angewendet werden sollen. |
|

### getCustomRedaction() {#getCustomRedaction--}
```
public final ICustomRedactionHandler getCustomRedaction()
```


Liefert einen benutzerdefinierten Redaktions-Handler. Unterstützt nur für PDF [PageAreaRedaction](../../com.groupdocs.redaction.redactions/pagearearedaction).


**Returns:**
[ICustomRedactionHandler](../../com.groupdocs.redaction.redactions/icustomredactionhandler) - An instance of [ICustomRedactionHandler](../../com.groupdocs.redaction.redactions/icustomredactionhandler), or  null  if not set.

### setCustomRedaction(ICustomRedactionHandler value) {#setCustomRedaction-com.groupdocs.redaction.redactions.ICustomRedactionHandler-}
```
public final void setCustomRedaction(ICustomRedactionHandler value)
```


Setzt einen benutzerdefinierten Redaktions-Handler. Unterstützt nur für PDF [PageAreaRedaction](../../com.groupdocs.redaction.redactions/pagearearedaction).


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | value | [ICustomRedactionHandler](../../com.groupdocs.redaction.redactions/icustomredactionhandler) | Eine Instanz von [ICustomRedactionHandler](../../com.groupdocs.redaction.redactions/icustomredactionhandler). |
|

### fromFilters(RedactionFilter[] filters) {#fromFilters-com.groupdocs.redaction.redactions.RedactionFilter---}
```
public static ReplacementOptions fromFilters(RedactionFilter[] filters)
```




**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| filters | [RedactionFilter\[\]](../../com.groupdocs.redaction.redactions/redactionfilter) |  |

**Returns:**
[ReplacementOptions](../../com.groupdocs.redaction.redactions/replacementoptions)
