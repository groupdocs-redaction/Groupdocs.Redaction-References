---
title: "MetadataRedaction"
second_title: "Référence API de GroupDocs.Redaction pour Java"
description: "Représente une classe abstraite de base pour les rédactions de métadonnées de document."
type: docs
weight: 20
url: /fr/java/com.groupdocs.redaction.redactions/metadataredaction/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.redaction.Redaction](../../com.groupdocs.redaction/redaction)
```
public abstract class MetadataRedaction extends Redaction
```

Représente une classe abstraite de base pour les rédactions de métadonnées de document.

*** ** * ** ***


**Learn more**

* More details about document metadata redactions: [Metadata redactions](../https://docs.groupdocs.com/redaction/java/metadata-redactions/)

<br />


## Méthodes

| Méthode | Description |
| --- | --- |
|  | [getFilter()](#getFilter--) | Obtient le filtre, qui est utilisé pour sélectionner toutes les métadonnées ou des métadonnées spécifiques, par exemple Auteur ou Société. |
|
|  | [setFilter(int value)](#setFilter-int-) | Définit le filtre, qui est utilisé pour sélectionner toutes les métadonnées ou des métadonnées spécifiques, par exemple Auteur ou Société. |
|
|  | [applyTo(DocumentFormatInstance formatInstance)](#applyTo-com.groupdocs.redaction.integration.DocumentFormatInstance-) | Applique la rédaction à une instance de format donnée. |
|
### getFilter() {#getFilter--}
```
public final int getFilter()
```


Obtient le filtre, qui est utilisé pour sélectionner toutes les métadonnées ou des métadonnées spécifiques, par exemple Auteur ou Société.


**Returns:**
int - Le filtre, qui est utilisé pour sélectionner toutes les métadonnées ou des métadonnées spécifiques, par exemple Auteur ou Société.

### setFilter(int value) {#setFilter-int-}
```
public final void setFilter(int value)
```


Définit le filtre, qui est utilisé pour sélectionner toutes les métadonnées ou des métadonnées spécifiques, par exemple Auteur ou Société.


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | valeur | int | Le filtre, qui est utilisé pour sélectionner toutes les métadonnées ou des métadonnées spécifiques, par exemple Auteur ou Société. |
|

### applyTo(DocumentFormatInstance formatInstance) {#applyTo-com.groupdocs.redaction.integration.DocumentFormatInstance-}
```
public RedactorLogEntry applyTo(DocumentFormatInstance formatInstance)
```


Applique la rédaction à une instance de format donnée.


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | formatInstance | [DocumentFormatInstance](../../com.groupdocs.redaction.integration/documentformatinstance) | Une instance d'un document pour appliquer la rédaction |
|

**Returns:**
[RedactorLogEntry](../../com.groupdocs.redaction/redactorlogentry) - Status of the redaction: success/failure and error message if any

