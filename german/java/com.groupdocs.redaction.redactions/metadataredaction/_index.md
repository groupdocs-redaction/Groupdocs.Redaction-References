---
title: "MetadataRedaction"
second_title: "GroupDocs.Redaction for Java API-Referenz"
description: "Stellt eine abstrakte Basisklasse für Dokument-Metadaten-Redaktionen dar."
type: docs
weight: 20
url: /de/java/com.groupdocs.redaction.redactions/metadataredaction/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.redaction.Redaction](../../com.groupdocs.redaction/redaction)
```
public abstract class MetadataRedaction extends Redaction
```

Stellt eine abstrakte Basisklasse für Dokument-Metadaten-Redaktionen dar.

*** ** * ** ***


**Learn more**

* More details about document metadata redactions: [Metadata redactions](../https://docs.groupdocs.com/redaction/java/metadata-redactions/)

<br />


## Methoden

| Methode | Beschreibung |
| --- | --- |
|  | [getFilter()](#getFilter--) | Ruft den Filter ab, der verwendet wird, um alle oder bestimmte Metadaten auszuwählen, zum Beispiel Autor oder Unternehmen. |
|
|  | [setFilter(int value)](#setFilter-int-) | Setzt den Filter, der verwendet wird, um alle oder bestimmte Metadaten auszuwählen, zum Beispiel Autor oder Unternehmen. |
|
|  | [applyTo(DocumentFormatInstance formatInstance)](#applyTo-com.groupdocs.redaction.integration.DocumentFormatInstance-) | Wendet die Redaktion auf eine gegebene Formatinstanz an. |
|
### getFilter() {#getFilter--}
```
public final int getFilter()
```


Ruft den Filter ab, der verwendet wird, um alle oder bestimmte Metadaten auszuwählen, zum Beispiel Autor oder Unternehmen.


**Returns:**
int - Der Filter, der verwendet wird, um alle oder bestimmte Metadaten auszuwählen, zum Beispiel Autor oder Unternehmen.

### setFilter(int value) {#setFilter-int-}
```
public final void setFilter(int value)
```


Setzt den Filter, der verwendet wird, um alle oder bestimmte Metadaten auszuwählen, zum Beispiel Autor oder Unternehmen.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | Wert | int | Der Filter, der verwendet wird, um alle oder bestimmte Metadaten auszuwählen, zum Beispiel Autor oder Unternehmen. |
|

### applyTo(DocumentFormatInstance formatInstance) {#applyTo-com.groupdocs.redaction.integration.DocumentFormatInstance-}
```
public RedactorLogEntry applyTo(DocumentFormatInstance formatInstance)
```


Wendet die Redaktion auf eine gegebene Formatinstanz an.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | formatInstance | [DocumentFormatInstance](../../com.groupdocs.redaction.integration/documentformatinstance) | Eine Instanz eines Dokuments, auf das die Redaktion angewendet wird |
|

**Returns:**
[RedactorLogEntry](../../com.groupdocs.redaction/redactorlogentry) - Status of the redaction: success/failure and error message if any

