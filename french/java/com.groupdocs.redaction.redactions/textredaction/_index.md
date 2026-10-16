---
title: "TextRedaction"
second_title: "Référence API de GroupDocs.Redaction pour Java"
description: "Représente une classe abstraite de base pour les rédactions de texte de document."
type: docs
weight: 32
url: /fr/java/com.groupdocs.redaction.redactions/textredaction/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.redaction.Redaction](../../com.groupdocs.redaction/redaction)
```
public abstract class TextRedaction extends Redaction
```

Représente une classe abstraite de base pour les rédactions de texte de document.

*** ** * ** ***


**Learn more**

* More details about applying redactions: [Redaction basics](../https://docs.groupdocs.com/redaction/java/redaction-basics/)
* More details about document text redactions: [Text redactions](../https://docs.groupdocs.com/redaction/java/text-redactions/)

<br />


## Méthodes

| Méthode | Description |
| --- | --- |
|  | [getActionOptions()](#getActionOptions--) | Obtient le |
ReplacementOptions
instance, spécifiant le type de remplacement de texte.
|
|  | [getOcrConnector()](#getOcrConnector--) | Obtient le |
IOcrConnector
implémentation, requise pour extraire le texte du contenu graphique.
|
|  | [setOcrConnector(IOcrConnector value)](#setOcrConnector-com.groupdocs.redaction.integration.IOcrConnector-) | Définit le |
IOcrConnector
implémentation, requise pour extraire le texte du contenu graphique.
|
### getActionOptions() {#getActionOptions--}
```
public final ReplacementOptions getActionOptions()
```


Obtient le
ReplacementOptions
instance, spécifiant le type de remplacement de texte.


**Returns:**
[ReplacementOptions](../../com.groupdocs.redaction.redactions/replacementoptions) - The  ReplacementOptions  instance, specifying type of text replacement.

### getOcrConnector() {#getOcrConnector--}
```
public final IOcrConnector getOcrConnector()
```


Obtient le
IOcrConnector
implémentation, requise pour extraire le texte du contenu graphique.


**Returns:**
[IOcrConnector](../../com.groupdocs.redaction.integration/iocrconnector) - The  IOcrConnector  implementation, required to extract text from graphic content.

### setOcrConnector(IOcrConnector value) {#setOcrConnector-com.groupdocs.redaction.integration.IOcrConnector-}
```
public final void setOcrConnector(IOcrConnector value)
```


Définit le
IOcrConnector
implémentation, requise pour extraire le texte du contenu graphique.


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | value | [IOcrConnector](../../com.groupdocs.redaction.integration/iocrconnector) | L'implémentation IOcrConnector, requise pour extraire le texte du contenu graphique. |
|

