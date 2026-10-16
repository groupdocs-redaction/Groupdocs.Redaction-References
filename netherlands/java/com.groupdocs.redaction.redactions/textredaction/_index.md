---
title: "TextRedaction"
second_title: "GroupDocs.Redaction for Java API-referentie"
description: "Vertegenwoordigt een abstracte basisklasse voor documenttekst-redacties."
type: docs
weight: 32
url: /nl/java/com.groupdocs.redaction.redactions/textredaction/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.redaction.Redaction](../../com.groupdocs.redaction/redaction)
```
public abstract class TextRedaction extends Redaction
```

Vertegenwoordigt een abstracte basisklasse voor documenttekst-redacties.

*** ** * ** ***


**Learn more**

* More details about applying redactions: [Redaction basics](../https://docs.groupdocs.com/redaction/java/redaction-basics/)
* More details about document text redactions: [Text redactions](../https://docs.groupdocs.com/redaction/java/text-redactions/)

<br />


## Methoden

| Methode | Beschrijving |
| --- | --- |
|  | [getActionOptions()](#getActionOptions--) | Haalt de |
ReplacementOptions
instantie, die het type tekstvervanging specificeert.
|
|  | [getOcrConnector()](#getOcrConnector--) | Haalt de |
IOcrConnector
implementatie, vereist om tekst uit grafische inhoud te extraheren.
|
|  | [setOcrConnector(IOcrConnector value)](#setOcrConnector-com.groupdocs.redaction.integration.IOcrConnector-) | Stelt de |
IOcrConnector
implementatie, vereist om tekst uit grafische inhoud te extraheren.
|
### getActionOptions() {#getActionOptions--}
```
public final ReplacementOptions getActionOptions()
```


Haalt de
ReplacementOptions
instantie, die het type tekstvervanging specificeert.


**Returns:**
[ReplacementOptions](../../com.groupdocs.redaction.redactions/replacementoptions) - The  ReplacementOptions  instance, specifying type of text replacement.

### getOcrConnector() {#getOcrConnector--}
```
public final IOcrConnector getOcrConnector()
```


Haalt de
IOcrConnector
implementatie, vereist om tekst uit grafische inhoud te extraheren.


**Returns:**
[IOcrConnector](../../com.groupdocs.redaction.integration/iocrconnector) - The  IOcrConnector  implementation, required to extract text from graphic content.

### setOcrConnector(IOcrConnector value) {#setOcrConnector-com.groupdocs.redaction.integration.IOcrConnector-}
```
public final void setOcrConnector(IOcrConnector value)
```


Stelt de
IOcrConnector
implementatie, vereist om tekst uit grafische inhoud te extraheren.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | value | [IOcrConnector](../../com.groupdocs.redaction.integration/iocrconnector) | De  IOcrConnector  implementatie, vereist om tekst uit grafische inhoud te extraheren. |
|

