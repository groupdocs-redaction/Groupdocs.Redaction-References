---
title: "RedactionDescription"
second_title: "GroupDocs.Redaction for Java API-referentie"
description: "Vertegenwoordigt informatie over een enkele wijzigingsactie die tijdens het redactieproces wordt uitgevoerd."
type: docs
weight: 25
url: /nl/java/com.groupdocs.redaction.redactions/redactiondescription/
---
**Inheritance:**
java.lang.Object
```
public class RedactionDescription
```

Vertegenwoordigt informatie over een enkele wijzigingsactie die tijdens het redactieproces wordt uitgevoerd.

*** ** * ** ***


**Learn more**

* More details about RedactionDescription class and IRedactionCallback interface: [Use redaction callback](../https://docs.groupdocs.com/redaction/java/use-redaction-callback/)

<br />


## Constructors

| Constructor | Beschrijving |
| --- | --- |
|  | [RedactionDescription(int redactionType, RedactionActionType actionType, String originalText)](#RedactionDescription-int-com.groupdocs.redaction.redactions.RedactionActionType-java.lang.String-) | Initialiseert een nieuw exemplaar van de RedactionDescription-klasse zonder vervangingsinformatie. |
|
|  | [RedactionDescription(int redactionType, RedactionActionType actionType, String originalText, TextReplacement replacement)](#RedactionDescription-int-com.groupdocs.redaction.redactions.RedactionActionType-java.lang.String-com.groupdocs.redaction.redactions.TextReplacement-) | Initialiseert een nieuw exemplaar van de RedactionDescription-klasse met vervangingsinformatie. |
|
|  | [RedactionDescription(int redactionType, RedactionActionType actionType, RegionReplacementOptions imageAreaReplacement, String imageDetails)](#RedactionDescription-int-com.groupdocs.redaction.redactions.RedactionActionType-com.groupdocs.redaction.redactions.RegionReplacementOptions-java.lang.String-) | Initialiseert een nieuw exemplaar van de RedactionDescription-klasse met vervangingsinformatie voor een afbeeldingsgebied. |
|
## Methoden

| Methode | Beschrijving |
| --- | --- |
|  | [getRedactionType()](#getRedactionType--) | Haalt het type documentgegevens op - tekst, metadata of annotaties. |
|
|  | [getActionType()](#getActionType--) | Haalt de redactie‑bewerking op: vervanging, opschoning of verwijdering. |
|
|  | [getOriginalText()](#getOriginalText--) | Haalt de overeenkomende tekst op, indien een expressie is opgegeven. |
|
|  | [getReplacement()](#getReplacement--) | Haalt de vervangingsinformatie op, kan null zijn. |
|
|  | [getImageAreaReplacement()](#getImageAreaReplacement--) | Haalt de vervangingsinformatie op voor afbeelding‑gebied redacties, retourneert null voor tekstuele redacties. |
|
|  | [getDetails()](#getDetails--) | Haalt optionele detailinformatie op voor het item dat wordt geredigeerd. |
|
|  | [setDetails(String value)](#setDetails-java.lang.String-) | Stelt optionele detailinformatie in voor het item dat wordt geredigeerd. |
|
### RedactionDescription(int redactionType, RedactionActionType actionType, String originalText) {#RedactionDescription-int-com.groupdocs.redaction.redactions.RedactionActionType-java.lang.String-}
```
public RedactionDescription(int redactionType, RedactionActionType actionType, String originalText)
```


Initialiseert een nieuw exemplaar van de RedactionDescription-klasse zonder vervangingsinformatie.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | redactionType | int | Type van de gegevens die worden geredigeerd |
|
|  | actionType | [RedactionActionType](../../com.groupdocs.redaction.redactions/redactionactiontype) | Actie die op deze gegevens moet worden uitgevoerd |
|
|  | originalText | java.lang.String | Overeenkomende tekst, opmerking of annotatie‑inhoud |
|

### RedactionDescription(int redactionType, RedactionActionType actionType, String originalText, TextReplacement replacement) {#RedactionDescription-int-com.groupdocs.redaction.redactions.RedactionActionType-java.lang.String-com.groupdocs.redaction.redactions.TextReplacement-}
```
public RedactionDescription(int redactionType, RedactionActionType actionType, String originalText, TextReplacement replacement)
```


Initialiseert een nieuw exemplaar van de RedactionDescription-klasse met vervangingsinformatie.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | redactionType | int | Type van de gegevens die worden geredigeerd |
|
|  | actionType | [RedactionActionType](../../com.groupdocs.redaction.redactions/redactionactiontype) | Actie die op deze gegevens moet worden uitgevoerd |
|
|  | originalText | java.lang.String | Overeenkomende tekst, opmerking of annotatie‑inhoud |
|
|  | replacement | [TextReplacement](../../com.groupdocs.redaction.redactions/textreplacement) | Vervangende tekst, overeenkomende tekst en de positie ervan binnen de originele tekenreeks |
|

### RedactionDescription(int redactionType, RedactionActionType actionType, RegionReplacementOptions imageAreaReplacement, String imageDetails) {#RedactionDescription-int-com.groupdocs.redaction.redactions.RedactionActionType-com.groupdocs.redaction.redactions.RegionReplacementOptions-java.lang.String-}
```
public RedactionDescription(int redactionType, RedactionActionType actionType, RegionReplacementOptions imageAreaReplacement, String imageDetails)
```


Initialiseert een nieuw exemplaar van de RedactionDescription-klasse met vervangingsinformatie voor een afbeeldingsgebied.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | redactionType | int | Type van de gegevens die worden geredigeerd |
|
|  | actionType | [RedactionActionType](../../com.groupdocs.redaction.redactions/redactionactiontype) | Actie die op deze gegevens moet worden uitgevoerd |
|
|  | imageAreaReplacement | [RegionReplacementOptions](../../com.groupdocs.redaction.redactions/regionreplacementoptions) | Vervangingsinformatie voor afbeeldingsgebied |
|
|  | imageDetails | java.lang.String | Tekstuele beschrijving van de afbeelding, standaard is String.Empty |
|

### getRedactionType() {#getRedactionType--}
```
public final int getRedactionType()
```


Haalt het type documentgegevens op - tekst, metadata of annotaties.


**Returns:**
int - Het type gegevens van het document - tekst, metadata of annotaties.

### getActionType() {#getActionType--}
```
public final RedactionActionType getActionType()
```


Haalt de redactie‑bewerking op: vervanging, opschoning of verwijdering.


**Returns:**
[RedactionActionType](../../com.groupdocs.redaction.redactions/redactionactiontype) - The redaction operation: replacement, cleanup or deletion.

### getOriginalText() {#getOriginalText--}
```
public final String getOriginalText()
```


Haalt de overeenkomende tekst op, indien een expressie is opgegeven.


**Returns:**
java.lang.String - De overeenkomende tekst, indien een expressie is opgegeven.

### getReplacement() {#getReplacement--}
```
public final TextReplacement getReplacement()
```


Haalt de vervangingsinformatie op, kan null zijn.


**Returns:**
[TextReplacement](../../com.groupdocs.redaction.redactions/textreplacement) - The replacement information, can be null.

### getImageAreaReplacement() {#getImageAreaReplacement--}
```
public final RegionReplacementOptions getImageAreaReplacement()
```


Haalt de vervangingsinformatie op voor afbeelding‑gebied redacties, retourneert null voor tekstuele redacties.


**Returns:**
[RegionReplacementOptions](../../com.groupdocs.redaction.redactions/regionreplacementoptions) - The replacement information for image area redactions, returns null for textual redactions.

### getDetails() {#getDetails--}
```
public final String getDetails()
```


Haalt optionele detailinformatie op voor het item dat wordt geredigeerd.


**Returns:**
java.lang.String - Optionele detailinformatie voor het item dat wordt geredigeerd.

### setDetails(String value) {#setDetails-java.lang.String-}
```
public final void setDetails(String value)
```


Stelt optionele detailinformatie in voor het item dat wordt geredigeerd.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | waarde | java.lang.String | Optionele detailinformatie voor het item dat wordt geredigeerd. |
|

