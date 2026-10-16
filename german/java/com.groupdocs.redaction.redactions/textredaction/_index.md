---
title: "TextRedaction"
second_title: "GroupDocs.Redaction for Java API-Referenz"
description: "Stellt eine abstrakte Basisklasse für Dokument-Text-Redaktionen dar."
type: docs
weight: 32
url: /de/java/com.groupdocs.redaction.redactions/textredaction/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.redaction.Redaction](../../com.groupdocs.redaction/redaction)
```
public abstract class TextRedaction extends Redaction
```

Stellt eine abstrakte Basisklasse für Dokument-Text-Redaktionen dar.

*** ** * ** ***


**Learn more**

* More details about applying redactions: [Redaction basics](../https://docs.groupdocs.com/redaction/java/redaction-basics/)
* More details about document text redactions: [Text redactions](../https://docs.groupdocs.com/redaction/java/text-redactions/)

<br />


## Methoden

| Methode | Beschreibung |
| --- | --- |
|  | [getActionOptions()](#getActionOptions--) | Liest das |
ReplacementOptions
Instanz, die den Typ des Textaustauschs angibt.
|
|  | [getOcrConnector()](#getOcrConnector--) | Liest das |
IOcrConnector
Implementierung, die zum Extrahieren von Text aus grafischen Inhalten erforderlich ist.
|
|  | [setOcrConnector(IOcrConnector value)](#setOcrConnector-com.groupdocs.redaction.integration.IOcrConnector-) | Setzt das |
IOcrConnector
Implementierung, die zum Extrahieren von Text aus grafischen Inhalten erforderlich ist.
|
### getActionOptions() {#getActionOptions--}
```
public final ReplacementOptions getActionOptions()
```


Liest das
ReplacementOptions
Instanz, die den Typ des Textaustauschs angibt.


**Returns:**
[ReplacementOptions](../../com.groupdocs.redaction.redactions/replacementoptions) - The  ReplacementOptions  instance, specifying type of text replacement.

### getOcrConnector() {#getOcrConnector--}
```
public final IOcrConnector getOcrConnector()
```


Liest das
IOcrConnector
Implementierung, die zum Extrahieren von Text aus grafischen Inhalten erforderlich ist.


**Returns:**
[IOcrConnector](../../com.groupdocs.redaction.integration/iocrconnector) - The  IOcrConnector  implementation, required to extract text from graphic content.

### setOcrConnector(IOcrConnector value) {#setOcrConnector-com.groupdocs.redaction.integration.IOcrConnector-}
```
public final void setOcrConnector(IOcrConnector value)
```


Setzt das
IOcrConnector
Implementierung, die zum Extrahieren von Text aus grafischen Inhalten erforderlich ist.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | value | [IOcrConnector](../../com.groupdocs.redaction.integration/iocrconnector) | Die IOcrConnector-Implementierung, die zum Extrahieren von Text aus grafischen Inhalten erforderlich ist. |
|

