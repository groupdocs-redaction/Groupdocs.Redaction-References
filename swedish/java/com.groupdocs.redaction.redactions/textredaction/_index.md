---
title: "TextRedaction"
second_title: "GroupDocs.Redaction för Java API-referens"
description: "Representerar en basabstrakt klass för dokumenttextredigeringar."
type: docs
weight: 32
url: /sv/java/com.groupdocs.redaction.redactions/textredaction/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.redaction.Redaction](../../com.groupdocs.redaction/redaction)
```
public abstract class TextRedaction extends Redaction
```

Representerar en basabstrakt klass för dokumenttextredigeringar.

*** ** * ** ***


**Learn more**

* More details about applying redactions: [Redaction basics](../https://docs.groupdocs.com/redaction/java/redaction-basics/)
* More details about document text redactions: [Text redactions](../https://docs.groupdocs.com/redaction/java/text-redactions/)

<br />


## Metoder

| Metod | Beskrivning |
| --- | --- |
|  | [getActionOptions()](#getActionOptions--) | Hämtar |
ReplacementOptions
instans, som specificerar typ av textersättning.
|
|  | [getOcrConnector()](#getOcrConnector--) | Hämtar |
IOcrConnector
implementation, som krävs för att extrahera text från grafiskt innehåll.
|
|  | [setOcrConnector(IOcrConnector value)](#setOcrConnector-com.groupdocs.redaction.integration.IOcrConnector-) | Ställer in |
IOcrConnector
implementation, som krävs för att extrahera text från grafiskt innehåll.
|
### getActionOptions() {#getActionOptions--}
```
public final ReplacementOptions getActionOptions()
```


Hämtar
ReplacementOptions
instans, som specificerar typ av textersättning.


**Returns:**
[ReplacementOptions](../../com.groupdocs.redaction.redactions/replacementoptions) - The  ReplacementOptions  instance, specifying type of text replacement.

### getOcrConnector() {#getOcrConnector--}
```
public final IOcrConnector getOcrConnector()
```


Hämtar
IOcrConnector
implementation, som krävs för att extrahera text från grafiskt innehåll.


**Returns:**
[IOcrConnector](../../com.groupdocs.redaction.integration/iocrconnector) - The  IOcrConnector  implementation, required to extract text from graphic content.

### setOcrConnector(IOcrConnector value) {#setOcrConnector-com.groupdocs.redaction.integration.IOcrConnector-}
```
public final void setOcrConnector(IOcrConnector value)
```


Ställer in
IOcrConnector
implementation, som krävs för att extrahera text från grafiskt innehåll.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | value | [IOcrConnector](../../com.groupdocs.redaction.integration/iocrconnector) | IOcrConnector-implementationen, som krävs för att extrahera text från grafiskt innehåll. |
|

