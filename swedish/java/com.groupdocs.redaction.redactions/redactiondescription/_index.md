---
title: "RedactionDescription"
second_title: "GroupDocs.Redaction för Java API-referens"
description: "Representerar information om en enskild förändringsåtgärd som utförs under redigeringsprocessen."
type: docs
weight: 25
url: /sv/java/com.groupdocs.redaction.redactions/redactiondescription/
---
**Inheritance:**
java.lang.Object
```
public class RedactionDescription
```

Representerar information om en enskild förändringsåtgärd som utförs under redigeringsprocessen.

*** ** * ** ***


**Learn more**

* More details about RedactionDescription class and IRedactionCallback interface: [Use redaction callback](../https://docs.groupdocs.com/redaction/java/use-redaction-callback/)

<br />


## Konstruktörer

| Konstruktor | Beskrivning |
| --- | --- |
|  | [RedactionDescription(int redactionType, RedactionActionType actionType, String originalText)](#RedactionDescription-int-com.groupdocs.redaction.redactions.RedactionActionType-java.lang.String-) | Initierar en ny instans av RedactionDescription-klassen utan ersättningsinformation. |
|
|  | [RedactionDescription(int redactionType, RedactionActionType actionType, String originalText, TextReplacement replacement)](#RedactionDescription-int-com.groupdocs.redaction.redactions.RedactionActionType-java.lang.String-com.groupdocs.redaction.redactions.TextReplacement-) | Initierar en ny instans av RedactionDescription-klassen med ersättningsinformation. |
|
|  | [RedactionDescription(int redactionType, RedactionActionType actionType, RegionReplacementOptions imageAreaReplacement, String imageDetails)](#RedactionDescription-int-com.groupdocs.redaction.redactions.RedactionActionType-com.groupdocs.redaction.redactions.RegionReplacementOptions-java.lang.String-) | Initierar en ny instans av RedactionDescription-klassen med ersättningsinformation för bildområde. |
|
## Metoder

| Metod | Beskrivning |
| --- | --- |
|  | [getRedactionType()](#getRedactionType--) | Hämtar typen av dokumentets data - text, metadata eller annotationer. |
|
|  | [getActionType()](#getActionType--) | Hämtar redigeringsoperationen: ersättning, rensning eller borttagning. |
|
|  | [getOriginalText()](#getOriginalText--) | Hämtar den matchade texten, om något uttryck har angetts. |
|
|  | [getReplacement()](#getReplacement--) | Hämtar ersättningsinformationen, kan vara null. |
|
|  | [getImageAreaReplacement()](#getImageAreaReplacement--) | Hämtar ersättningsinformationen för bildområdesredigeringar, returnerar null för textredigeringar. |
|
|  | [getDetails()](#getDetails--) | Hämtar en valfri detaljerad information för objektet som redigeras. |
|
|  | [setDetails(String value)](#setDetails-java.lang.String-) | Ställer in en valfri detaljerad information för objektet som redigeras. |
|
### RedactionDescription(int redactionType, RedactionActionType actionType, String originalText) {#RedactionDescription-int-com.groupdocs.redaction.redactions.RedactionActionType-java.lang.String-}
```
public RedactionDescription(int redactionType, RedactionActionType actionType, String originalText)
```


Initierar en ny instans av RedactionDescription-klassen utan ersättningsinformation.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | redactionType | int | Typ av data som redigeras |
|
|  | actionType | [RedactionActionType](../../com.groupdocs.redaction.redactions/redactionactiontype) | Åtgärd som ska utföras på dessa data |
|
|  | originalText | java.lang.String | Matchad text, kommentar eller annoteringskropp |
|

### RedactionDescription(int redactionType, RedactionActionType actionType, String originalText, TextReplacement replacement) {#RedactionDescription-int-com.groupdocs.redaction.redactions.RedactionActionType-java.lang.String-com.groupdocs.redaction.redactions.TextReplacement-}
```
public RedactionDescription(int redactionType, RedactionActionType actionType, String originalText, TextReplacement replacement)
```


Initierar en ny instans av RedactionDescription-klassen med ersättningsinformation.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | redactionType | int | Typ av data som redigeras |
|
|  | actionType | [RedactionActionType](../../com.groupdocs.redaction.redactions/redactionactiontype) | Åtgärd som ska utföras på dessa data |
|
|  | originalText | java.lang.String | Matchad text, kommentar eller annoteringskropp |
|
|  | replacement | [TextReplacement](../../com.groupdocs.redaction.redactions/textreplacement) | Ersättningstext, matchad text och dess position i den ursprungliga strängen |
|

### RedactionDescription(int redactionType, RedactionActionType actionType, RegionReplacementOptions imageAreaReplacement, String imageDetails) {#RedactionDescription-int-com.groupdocs.redaction.redactions.RedactionActionType-com.groupdocs.redaction.redactions.RegionReplacementOptions-java.lang.String-}
```
public RedactionDescription(int redactionType, RedactionActionType actionType, RegionReplacementOptions imageAreaReplacement, String imageDetails)
```


Initierar en ny instans av RedactionDescription-klassen med ersättningsinformation för bildområde.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | redactionType | int | Typ av data som redigeras |
|
|  | actionType | [RedactionActionType](../../com.groupdocs.redaction.redactions/redactionactiontype) | Åtgärd som ska utföras på dessa data |
|
|  | imageAreaReplacement | [RegionReplacementOptions](../../com.groupdocs.redaction.redactions/regionreplacementoptions) | Ersättningsinformation för bildområde |
|
|  | imageDetails | java.lang.String | Textuell beskrivning av bilden, som standard är den String.Empty |
|

### getRedactionType() {#getRedactionType--}
```
public final int getRedactionType()
```


Hämtar typen av dokumentets data - text, metadata eller annotationer.


**Returns:**
int – Typen av dokumentets data – text, metadata eller annotationer.

### getActionType() {#getActionType--}
```
public final RedactionActionType getActionType()
```


Hämtar redigeringsoperationen: ersättning, rensning eller borttagning.


**Returns:**
[RedactionActionType](../../com.groupdocs.redaction.redactions/redactionactiontype) - The redaction operation: replacement, cleanup or deletion.

### getOriginalText() {#getOriginalText--}
```
public final String getOriginalText()
```


Hämtar den matchade texten, om något uttryck har angetts.


**Returns:**
java.lang.String – Den matchade texten, om något uttryck har angetts.

### getReplacement() {#getReplacement--}
```
public final TextReplacement getReplacement()
```


Hämtar ersättningsinformationen, kan vara null.


**Returns:**
[TextReplacement](../../com.groupdocs.redaction.redactions/textreplacement) - The replacement information, can be null.

### getImageAreaReplacement() {#getImageAreaReplacement--}
```
public final RegionReplacementOptions getImageAreaReplacement()
```


Hämtar ersättningsinformationen för bildområdesredigeringar, returnerar null för textredigeringar.


**Returns:**
[RegionReplacementOptions](../../com.groupdocs.redaction.redactions/regionreplacementoptions) - The replacement information for image area redactions, returns null for textual redactions.

### getDetails() {#getDetails--}
```
public final String getDetails()
```


Hämtar en valfri detaljerad information för objektet som redigeras.


**Returns:**
java.lang.String – En valfri detaljerad information för objektet som redigeras.

### setDetails(String value) {#setDetails-java.lang.String-}
```
public final void setDetails(String value)
```


Ställer in en valfri detaljerad information för objektet som redigeras.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | värde | java.lang.String | En valfri detaljerad information för objektet som redigeras. |
|

