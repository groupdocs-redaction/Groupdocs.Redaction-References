---
title: "MetadataRedaction"
second_title: "GroupDocs.Redaction for Java API-referentie"
description: "Vertegenwoordigt een abstracte basisklasse voor documentmetadata-redacties."
type: docs
weight: 20
url: /nl/java/com.groupdocs.redaction.redactions/metadataredaction/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.redaction.Redaction](../../com.groupdocs.redaction/redaction)
```
public abstract class MetadataRedaction extends Redaction
```

Vertegenwoordigt een abstracte basisklasse voor documentmetadata-redacties.

*** ** * ** ***


**Learn more**

* More details about document metadata redactions: [Metadata redactions](../https://docs.groupdocs.com/redaction/java/metadata-redactions/)

<br />


## Methoden

| Methode | Beschrijving |
| --- | --- |
|  | [getFilter()](#getFilter--) | Haalt het filter op, dat wordt gebruikt om alle of specifieke metadata te selecteren, bijvoorbeeld Auteur of Bedrijf. |
|
|  | [setFilter(int value)](#setFilter-int-) | Stelt het filter in, dat wordt gebruikt om alle of specifieke metadata te selecteren, bijvoorbeeld Auteur of Bedrijf. |
|
|  | [applyTo(DocumentFormatInstance formatInstance)](#applyTo-com.groupdocs.redaction.integration.DocumentFormatInstance-) | Past de redactie toe op een gegeven formaatinstantie. |
|
### getFilter() {#getFilter--}
```
public final int getFilter()
```


Haalt het filter op, dat wordt gebruikt om alle of specifieke metadata te selecteren, bijvoorbeeld Auteur of Bedrijf.


**Returns:**
int - Het filter, dat wordt gebruikt om alle of specifieke metadata te selecteren, bijvoorbeeld Auteur of Bedrijf.

### setFilter(int value) {#setFilter-int-}
```
public final void setFilter(int value)
```


Stelt het filter in, dat wordt gebruikt om alle of specifieke metadata te selecteren, bijvoorbeeld Auteur of Bedrijf.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | waarde | int | Het filter, dat wordt gebruikt om alle of specifieke metadata te selecteren, bijvoorbeeld Auteur of Bedrijf. |
|

### applyTo(DocumentFormatInstance formatInstance) {#applyTo-com.groupdocs.redaction.integration.DocumentFormatInstance-}
```
public RedactorLogEntry applyTo(DocumentFormatInstance formatInstance)
```


Past de redactie toe op een gegeven formaatinstantie.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | formatInstance | [DocumentFormatInstance](../../com.groupdocs.redaction.integration/documentformatinstance) | Een instantie van een document om redactie toe te passen |
|

**Returns:**
[RedactorLogEntry](../../com.groupdocs.redaction/redactorlogentry) - Status of the redaction: success/failure and error message if any

