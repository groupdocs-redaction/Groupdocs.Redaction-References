---
title: "MetadataRedaction"
second_title: "GroupDocs.Redaction för Java API-referens"
description: "Representerar en basabstrakt klass för dokumentmetadata‑redigeringar."
type: docs
weight: 20
url: /sv/java/com.groupdocs.redaction.redactions/metadataredaction/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.redaction.Redaction](../../com.groupdocs.redaction/redaction)
```
public abstract class MetadataRedaction extends Redaction
```

Representerar en basabstrakt klass för dokumentmetadata‑redigeringar.

*** ** * ** ***


**Learn more**

* More details about document metadata redactions: [Metadata redactions](../https://docs.groupdocs.com/redaction/java/metadata-redactions/)

<br />


## Metoder

| Metod | Beskrivning |
| --- | --- |
|  | [getFilter()](#getFilter--) | Hämtar filtret som används för att välja all eller specifik metadata, till exempel Author eller Company. |
|
|  | [setFilter(int value)](#setFilter-int-) | Ställer in filtret som används för att välja all eller specifik metadata, till exempel Author eller Company. |
|
|  | [applyTo(DocumentFormatInstance formatInstance)](#applyTo-com.groupdocs.redaction.integration.DocumentFormatInstance-) | Tillämpar redigeringen på en given formatinstans. |
|
### getFilter() {#getFilter--}
```
public final int getFilter()
```


Hämtar filtret som används för att välja all eller specifik metadata, till exempel Author eller Company.


**Returns:**
int - Filtret som används för att välja all eller specifik metadata, till exempel Author eller Company.

### setFilter(int value) {#setFilter-int-}
```
public final void setFilter(int value)
```


Ställer in filtret som används för att välja all eller specifik metadata, till exempel Author eller Company.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | värde | int | Filtret som används för att välja all eller specifik metadata, till exempel Author eller Company. |
|

### applyTo(DocumentFormatInstance formatInstance) {#applyTo-com.groupdocs.redaction.integration.DocumentFormatInstance-}
```
public RedactorLogEntry applyTo(DocumentFormatInstance formatInstance)
```


Tillämpar redigeringen på en given formatinstans.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | formatInstance | [DocumentFormatInstance](../../com.groupdocs.redaction.integration/documentformatinstance) | En instans av ett dokument för att tillämpa redigering |
|

**Returns:**
[RedactorLogEntry](../../com.groupdocs.redaction/redactorlogentry) - Status of the redaction: success/failure and error message if any

