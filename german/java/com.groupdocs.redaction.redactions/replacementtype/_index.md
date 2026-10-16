---
title: "ReplacementType"
second_title: "GroupDocs.Redaction for Java API-Referenz"
description: "Stellt einen Typ des Austauschs für den übereinstimmenden Text dar."
type: docs
weight: 38
url: /de/java/com.groupdocs.redaction.redactions/replacementtype/
---
**Inheritance:**
java.lang.Object, java.lang.Enum
```
public enum ReplacementType extends Enum<ReplacementType>
```

Stellt einen Typ des Austauschs für den übereinstimmenden Text dar.

## Felder

| Feld | Beschreibung |
| --- | --- |
|  | [ReplaceString](#ReplaceString) | Ersetzt den gefundenen Text durch einen anderen String, z. B. |
|
|  | [DrawBox](#DrawBox) | Zeichnet ein Rechteck mit einer bestimmten Farbe (Standard ist Schwarz) anstelle des geschwärzten Textes. |
|
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [values()](#values--) |  |
| [valueOf(String name)](#valueOf-java.lang.String-) |  |
### ReplaceString {#ReplaceString}
```
public static final ReplacementType ReplaceString
```


Ersetzt den gefundenen Text durch einen anderen String, z. B. den Befreiungscode.


### DrawBox {#DrawBox}
```
public static final ReplacementType DrawBox
```


Zeichnet ein Rechteck mit einer bestimmten Farbe (Standard ist Schwarz) anstelle des geschwärzten Textes.


### values() {#values--}
```
public static ReplacementType[] values()
```




**Returns:**
com.groupdocs.redaction.redactions.ReplacementType[]
### valueOf(String name) {#valueOf-java.lang.String-}
```
public static ReplacementType valueOf(String name)
```




**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Name | java.lang.String |  |

**Returns:**
[ReplacementType](../../com.groupdocs.redaction.redactions/replacementtype)
