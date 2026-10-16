---
title: "RedactionDescription"
second_title: "GroupDocs.Redaction for Java API-Referenz"
description: "Stellt eine einzelne Änderungsaktionsinformation dar, die während des Redaktionsprozesses ausgeführt wird."
type: docs
weight: 25
url: /de/java/com.groupdocs.redaction.redactions/redactiondescription/
---
**Inheritance:**
java.lang.Object
```
public class RedactionDescription
```

Stellt eine einzelne Änderungsaktionsinformation dar, die während des Redaktionsprozesses ausgeführt wird.

*** ** * ** ***


**Learn more**

* More details about RedactionDescription class and IRedactionCallback interface: [Use redaction callback](../https://docs.groupdocs.com/redaction/java/use-redaction-callback/)

<br />


## Konstruktoren

| Konstruktor | Beschreibung |
| --- | --- |
|  | [RedactionDescription(int redactionType, RedactionActionType actionType, String originalText)](#RedactionDescription-int-com.groupdocs.redaction.redactions.RedactionActionType-java.lang.String-) | Initialisiert eine neue Instanz der Klasse RedactionDescription ohne Ersetzungsinformationen. |
|
|  | [RedactionDescription(int redactionType, RedactionActionType actionType, String originalText, TextReplacement replacement)](#RedactionDescription-int-com.groupdocs.redaction.redactions.RedactionActionType-java.lang.String-com.groupdocs.redaction.redactions.TextReplacement-) | Initialisiert eine neue Instanz der Klasse RedactionDescription mit Ersetzungsinformationen. |
|
|  | [RedactionDescription(int redactionType, RedactionActionType actionType, RegionReplacementOptions imageAreaReplacement, String imageDetails)](#RedactionDescription-int-com.groupdocs.redaction.redactions.RedactionActionType-com.groupdocs.redaction.redactions.RegionReplacementOptions-java.lang.String-) | Initialisiert eine neue Instanz der Klasse RedactionDescription mit Bildbereich-Ersetzungsinformationen. |
|
## Methoden

| Methode | Beschreibung |
| --- | --- |
|  | [getRedactionType()](#getRedactionType--) | Gibt den Typ der Dokumentdaten zurück – Text, Metadaten oder Anmerkungen. |
|
|  | [getActionType()](#getActionType--) | Gibt die Redaktionsoperation zurück: Ersetzung, Bereinigung oder Löschung. |
|
|  | [getOriginalText()](#getOriginalText--) | Gibt den gefundenen Text zurück, falls ein Ausdruck angegeben ist. |
|
|  | [getReplacement()](#getReplacement--) | Gibt die Ersetzungsinformationen zurück, kann null sein. |
|
|  | [getImageAreaReplacement()](#getImageAreaReplacement--) | Gibt die Ersetzungsinformationen für Bildbereichs-Redaktionen zurück, liefert null für textuelle Redaktionen. |
|
|  | [getDetails()](#getDetails--) | Gibt optionale Detailinformationen für das zu redigierende Element zurück. |
|
|  | [setDetails(String value)](#setDetails-java.lang.String-) | Setzt optionale Detailinformationen für das zu redigierende Element. |
|
### RedactionDescription(int redactionType, RedactionActionType actionType, String originalText) {#RedactionDescription-int-com.groupdocs.redaction.redactions.RedactionActionType-java.lang.String-}
```
public RedactionDescription(int redactionType, RedactionActionType actionType, String originalText)
```


Initialisiert eine neue Instanz der Klasse RedactionDescription ohne Ersetzungsinformationen.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | redactionType | int | Typ der zu redigierenden Daten |
|
|  | actionType | [RedactionActionType](../../com.groupdocs.redaction.redactions/redactionactiontype) | Aktion, die für diese Daten ausgeführt werden soll |
|
|  | originalText | java.lang.String | Gefundener Text, Kommentar oder Anmerkungsinhalt |
|

### RedactionDescription(int redactionType, RedactionActionType actionType, String originalText, TextReplacement replacement) {#RedactionDescription-int-com.groupdocs.redaction.redactions.RedactionActionType-java.lang.String-com.groupdocs.redaction.redactions.TextReplacement-}
```
public RedactionDescription(int redactionType, RedactionActionType actionType, String originalText, TextReplacement replacement)
```


Initialisiert eine neue Instanz der Klasse RedactionDescription mit Ersetzungsinformationen.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | redactionType | int | Typ der zu redigierenden Daten |
|
|  | actionType | [RedactionActionType](../../com.groupdocs.redaction.redactions/redactionactiontype) | Aktion, die für diese Daten ausgeführt werden soll |
|
|  | originalText | java.lang.String | Gefundener Text, Kommentar oder Anmerkungsinhalt |
|
|  | replacement | [TextReplacement](../../com.groupdocs.redaction.redactions/textreplacement) | Ersetzungstext, gefundener Text und dessen Position im Originalstring |
|

### RedactionDescription(int redactionType, RedactionActionType actionType, RegionReplacementOptions imageAreaReplacement, String imageDetails) {#RedactionDescription-int-com.groupdocs.redaction.redactions.RedactionActionType-com.groupdocs.redaction.redactions.RegionReplacementOptions-java.lang.String-}
```
public RedactionDescription(int redactionType, RedactionActionType actionType, RegionReplacementOptions imageAreaReplacement, String imageDetails)
```


Initialisiert eine neue Instanz der Klasse RedactionDescription mit Bildbereich-Ersetzungsinformationen.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | redactionType | int | Typ der zu redigierenden Daten |
|
|  | actionType | [RedactionActionType](../../com.groupdocs.redaction.redactions/redactionactiontype) | Aktion, die für diese Daten ausgeführt werden soll |
|
|  | imageAreaReplacement | [RegionReplacementOptions](../../com.groupdocs.redaction.redactions/regionreplacementoptions) | Informationen zur Ersetzung des Bildbereichs |
|
|  | imageDetails | java.lang.String | Textuelle Bildbeschreibung, standardmäßig ist sie String.Empty |
|

### getRedactionType() {#getRedactionType--}
```
public final int getRedactionType()
```


Gibt den Typ der Dokumentdaten zurück – Text, Metadaten oder Anmerkungen.


**Returns:**
int - Der Typ der Dokumentdaten - Text, Metadaten oder Anmerkungen.

### getActionType() {#getActionType--}
```
public final RedactionActionType getActionType()
```


Gibt die Redaktionsoperation zurück: Ersetzung, Bereinigung oder Löschung.


**Returns:**
[RedactionActionType](../../com.groupdocs.redaction.redactions/redactionactiontype) - The redaction operation: replacement, cleanup or deletion.

### getOriginalText() {#getOriginalText--}
```
public final String getOriginalText()
```


Gibt den gefundenen Text zurück, falls ein Ausdruck angegeben ist.


**Returns:**
java.lang.String - Der gefundene Text, falls ein Ausdruck angegeben ist.

### getReplacement() {#getReplacement--}
```
public final TextReplacement getReplacement()
```


Gibt die Ersetzungsinformationen zurück, kann null sein.


**Returns:**
[TextReplacement](../../com.groupdocs.redaction.redactions/textreplacement) - The replacement information, can be null.

### getImageAreaReplacement() {#getImageAreaReplacement--}
```
public final RegionReplacementOptions getImageAreaReplacement()
```


Gibt die Ersetzungsinformationen für Bildbereichs-Redaktionen zurück, liefert null für textuelle Redaktionen.


**Returns:**
[RegionReplacementOptions](../../com.groupdocs.redaction.redactions/regionreplacementoptions) - The replacement information for image area redactions, returns null for textual redactions.

### getDetails() {#getDetails--}
```
public final String getDetails()
```


Gibt optionale Detailinformationen für das zu redigierende Element zurück.


**Returns:**
java.lang.String - Eine optionale Detailinformation für das zu redigierende Element.

### setDetails(String value) {#setDetails-java.lang.String-}
```
public final void setDetails(String value)
```


Setzt optionale Detailinformationen für das zu redigierende Element.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | Wert | java.lang.String | Eine optionale Detailinformation für das zu redigierende Element. |
|

