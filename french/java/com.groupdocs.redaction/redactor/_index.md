---
title: "Redactor"
second_title: "Référence API de GroupDocs.Redaction pour Java"
description: "Représente une classe principale qui contrôle le processus de caviardage de documents, permettant d'ouvrir, de caviarder et d'enregistrer des documents."
type: docs
weight: 16
url: /fr/java/com.groupdocs.redaction/redactor/
---
**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
java.io.Closeable, [com.groupdocs.redaction.integration.IPreviewable](../../com.groupdocs.redaction.integration/ipreviewable)
```
public final class Redactor implements Closeable, IPreviewable
```

Représente la classe principale qui contrôle le processus de rédaction de documents, permettant d'ouvrir, de rédiger et d'enregistrer les documents.

*** ** * ** ***


**Learn more**

* More details about applying redactions: [Redaction basics](../https://docs.groupdocs.com/redaction/java/redaction-basics/)
* More advanced redaction topics: [Advanced usage](../https://docs.groupdocs.com/redaction/java/advanced-usage/)

<br />


## Constructeurs

| Constructeur | Description |
| --- | --- |
|  | [Redactor(String filePath)](#Redactor-java.lang.String-) | Initialise une nouvelle instance de |
Redactor
classe utilisant le chemin du fichier.
|
|  | [Redactor(InputStream document)](#Redactor-java.io.InputStream-) | Initialise une nouvelle instance de |
Redactor
classe utilisant le flux.
|
|  | [Redactor(String filePath, LoadOptions loadOptions)](#Redactor-java.lang.String-com.groupdocs.redaction.options.LoadOptions-) | Initialise une nouvelle instance de |
Redactor
classe pour un document protégé par mot de passe utilisant son chemin.
|
|  | [Redactor(String filePath, LoadOptions loadOptions, RedactorSettings settings)](#Redactor-java.lang.String-com.groupdocs.redaction.options.LoadOptions-com.groupdocs.redaction.options.RedactorSettings-) | Initialise une nouvelle instance de |
Redactor
classe pour un document protégé par mot de passe utilisant son chemin et ses paramètres.
|
|  | [Redactor(InputStream document, LoadOptions loadOptions)](#Redactor-java.io.InputStream-com.groupdocs.redaction.options.LoadOptions-) | Initialise une nouvelle instance de |
Redactor
classe pour un document protégé par mot de passe utilisant le flux.
|
|  | [Redactor(InputStream document, LoadOptions loadOptions, RedactorSettings settings)](#Redactor-java.io.InputStream-com.groupdocs.redaction.options.LoadOptions-com.groupdocs.redaction.options.RedactorSettings-) | Initialise une nouvelle instance de |
Redactor
classe pour un document protégé par mot de passe utilisant le flux et ses paramètres.
|
## Méthodes

| Méthode | Description |
| --- | --- |
|  | [close()](#close--) | Libère les ressources. |
|
|  | [apply(Redaction redaction)](#apply-com.groupdocs.redaction.Redaction-) | Applique un caviardage au document. |
|
|  | [apply(Redaction[] redactions)](#apply-com.groupdocs.redaction.Redaction---) | Applique un ensemble de caviardages au document. |
|
|  | [apply(RedactionPolicy policy)](#apply-com.groupdocs.redaction.RedactionPolicy-) | Applique une politique de caviardage au document. |
|
|  | [save()](#save--) | Enregistre le document dans un fichier avec les options suivantes : AddSuffix = true, RasterizeToPDF = true. |
|
|  | [save(SaveOptions saveOptions)](#save-com.groupdocs.redaction.options.SaveOptions-) | Enregistre le document dans un fichier. |
|
|  | [save(OutputStream document)](#save-java.io.OutputStream-) | Enregistre le document dans un flux. |
|
|  | [save(OutputStream document, SaveOptions saveOptions)](#save-java.io.OutputStream-com.groupdocs.redaction.options.SaveOptions-) | Enregistre le document dans un flux. |
|
|  | [save(OutputStream document, RasterizationOptions rasterizationOptions)](#save-java.io.OutputStream-com.groupdocs.redaction.options.RasterizationOptions-) | Enregistre le document dans un flux, y compris l'emplacement personnalisé. |
|
|  | [generatePreview(PreviewOptions previewOptions)](#generatePreview-com.groupdocs.redaction.options.PreviewOptions-) | Génère des images d'aperçu de pages spécifiques dans un format d'image donné. |
|
|  | [getDocumentInfo()](#getDocumentInfo--) | Obtient les informations générales sur le document - taille, nombre de pages, etc. |
|
### Redactor(String filePath) {#Redactor-java.lang.String-}
```
public Redactor(String filePath)
```


Initialise une nouvelle instance de
Redactor
classe utilisant le chemin du fichier.


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | filePath | java.lang.String | Chemin du fichier |


L'exemple suivant montre comment ouvrir un document pour le caviardage.

````

  try (Redactor redactor = new Redactor("C:\\sample.pdf"))
 {
     // Here we can use document instance to perform redactions
 }
 
``` 
````

 |

### Redactor(InputStream document) {#Redactor-java.io.InputStream-}
```
public Redactor(InputStream document)
```


Initializes a new instance of 
Redactor
 class using stream.


**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| document | java.io.InputStream | Source stream of the document


The following example demonstrates how to open a document from stream.

````

try (InputStream stream = new FileInputStream("C:\\sample.pdf"))
{
try (Redactor redactor = new Redactor(stream))
{
// Ici nous pouvons utiliser l'instance du document pour effectuer des rédactions
}
}
 
``` 
````

|

### Redactor(String filePath, LoadOptions loadOptions) {#Redactor-java.lang.String-com.groupdocs.redaction.options.LoadOptions-}
```
public Redactor(String filePath, LoadOptions loadOptions)
```


Initialise une nouvelle instance de
Redactor
classe pour un document protégé par mot de passe utilisant son chemin.


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | filePath | java.lang.String | Chemin du fichier. |
|
|  | loadOptions | [LoadOptions](../../com.groupdocs.redaction.options/loadoptions) | Options, y compris le mot de passe. |
|

### Redactor(String filePath, LoadOptions loadOptions, RedactorSettings settings) {#Redactor-java.lang.String-com.groupdocs.redaction.options.LoadOptions-com.groupdocs.redaction.options.RedactorSettings-}
```
public Redactor(String filePath, LoadOptions loadOptions, RedactorSettings settings)
```


Initialise une nouvelle instance de
Redactor
classe pour un document protégé par mot de passe utilisant son chemin et ses paramètres.


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | filePath | java.lang.String | Chemin du fichier. |
|
|  | loadOptions | [LoadOptions](../../com.groupdocs.redaction.options/loadoptions) | Options dépendantes du fichier, y compris le mot de passe. |
|
|  | settings | [RedactorSettings](../../com.groupdocs.redaction.options/redactorsettings) | Paramètres par défaut pour le processus de rédaction. |
|

### Redactor(InputStream document, LoadOptions loadOptions) {#Redactor-java.io.InputStream-com.groupdocs.redaction.options.LoadOptions-}
```
public Redactor(InputStream document, LoadOptions loadOptions)
```


Initialise une nouvelle instance de
Redactor
classe pour un document protégé par mot de passe utilisant le flux.


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | document | java.io.InputStream | Flux d'entrée source. |
|
|  | loadOptions | [LoadOptions](../../com.groupdocs.redaction.options/loadoptions) | Options, y compris le mot de passe. |
|

### Redactor(InputStream document, LoadOptions loadOptions, RedactorSettings settings) {#Redactor-java.io.InputStream-com.groupdocs.redaction.options.LoadOptions-com.groupdocs.redaction.options.RedactorSettings-}
```
public Redactor(InputStream document, LoadOptions loadOptions, RedactorSettings settings)
```


Initialise une nouvelle instance de
Redactor
classe pour un document protégé par mot de passe utilisant le flux et ses paramètres.


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | document | java.io.InputStream | Flux d'entrée source. |
|
|  | loadOptions | [LoadOptions](../../com.groupdocs.redaction.options/loadoptions) | Options, y compris le mot de passe. |
|
|  | settings | [RedactorSettings](../../com.groupdocs.redaction.options/redactorsettings) | Paramètres par défaut pour le processus de rédaction. |
|

### close() {#close--}
```
public final void close()
```


Libère les ressources.


### apply(Redaction redaction) {#apply-com.groupdocs.redaction.Redaction-}
```
public final RedactorChangeLog apply(Redaction redaction)
```


Applique un caviardage au document.


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | redaction | [Redaction](../../com.groupdocs.redaction/redaction) | Une instance de  Redaction  à appliquer |
|

**Returns:**
[RedactorChangeLog](../../com.groupdocs.redaction/redactorchangelog) - Success or failure and error message in this case

### apply(Redaction[] redactions) {#apply-com.groupdocs.redaction.Redaction---}
```
public final RedactorChangeLog apply(Redaction[] redactions)
```


Applique un ensemble de caviardages au document.


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | redactions | [Redaction\[\]](../../com.groupdocs.redaction/redaction) | Un tableau de rédactions à appliquer |
|

**Returns:**
[RedactorChangeLog](../../com.groupdocs.redaction/redactorchangelog) - Success or failure and error message in this case

### apply(RedactionPolicy policy) {#apply-com.groupdocs.redaction.RedactionPolicy-}
```
public final RedactorChangeLog apply(RedactionPolicy policy)
```


Applique une politique de caviardage au document.


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | policy | [RedactionPolicy](../../com.groupdocs.redaction/redactionpolicy) | Politique de rédaction |
|

**Returns:**
[RedactorChangeLog](../../com.groupdocs.redaction/redactorchangelog) - Success or failure and error message in this case

### save() {#save--}
```
public final String save()
```


Enregistre le document dans un fichier avec les options suivantes : AddSuffix = true, RasterizeToPDF = true.


**Returns:**
java.lang.String - Chemin vers le document rédigé

### save(SaveOptions saveOptions) {#save-com.groupdocs.redaction.options.SaveOptions-}
```
public final String save(SaveOptions saveOptions)
```


Enregistre le document dans un fichier.


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | saveOptions | [SaveOptions](../../com.groupdocs.redaction.options/saveoptions) | Options pour ajouter un suffixe ou rasteriser |
|

**Returns:**
java.lang.String - Chemin vers le document rédigé

### save(OutputStream document) {#save-java.io.OutputStream-}
```
public final void save(OutputStream document)
```


Enregistre le document dans un flux.


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | document | java.io.OutputStream | Flux cible |
|

### save(OutputStream document, SaveOptions saveOptions) {#save-java.io.OutputStream-com.groupdocs.redaction.options.SaveOptions-}
```
public final void save(OutputStream document, SaveOptions saveOptions)
```


Enregistre le document dans un flux.


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | document | java.io.OutputStream | Flux cible |
|
|  | saveOptions | [SaveOptions](../../com.groupdocs.redaction.options/saveoptions) | Options d'enregistrement |
|

### save(OutputStream document, RasterizationOptions rasterizationOptions) {#save-java.io.OutputStream-com.groupdocs.redaction.options.RasterizationOptions-}
```
public final void save(OutputStream document, RasterizationOptions rasterizationOptions)
```


Enregistre le document dans un flux, y compris l'emplacement personnalisé.


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | document | java.io.OutputStream | Flux cible |
|
|  | rasterizationOptions | [RasterizationOptions](../../com.groupdocs.redaction.options/rasterizationoptions) | Options pour rasteriser ou non et pour spécifier les pages à rasteriser |
|

### generatePreview(PreviewOptions previewOptions) {#generatePreview-com.groupdocs.redaction.options.PreviewOptions-}
```
public final void generatePreview(PreviewOptions previewOptions)
```


Génère des images d'aperçu de pages spécifiques dans un format d'image donné.


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | previewOptions | [PreviewOptions](../../com.groupdocs.redaction.options/previewoptions) | Paramètres des propriétés d'image et de la plage de pages |
|

### getDocumentInfo() {#getDocumentInfo--}
```
public final IDocumentInfo getDocumentInfo()
```


Obtient les informations générales sur le document - taille, nombre de pages, etc.


**Returns:**
[IDocumentInfo](../../com.groupdocs.redaction/idocumentinfo) - An instance of IDocumentInfo

