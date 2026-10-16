---
title: "Redactor"
second_title: "GroupDocs.Redaction for Java API-referentie"
description: "Stelt een hoofdklasse voor die het documentredactieproces beheert en het openen, redigeren en opslaan van documenten mogelijk maakt."
type: docs
weight: 16
url: /nl/java/com.groupdocs.redaction/redactor/
---
**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
java.io.Closeable, [com.groupdocs.redaction.integration.IPreviewable](../../com.groupdocs.redaction.integration/ipreviewable)
```
public final class Redactor implements Closeable, IPreviewable
```

Stelt een hoofdklasse voor die het documentredactietraject beheert, waardoor documenten kunnen worden geopend, geredigeerd en opgeslagen.

*** ** * ** ***


**Learn more**

* More details about applying redactions: [Redaction basics](../https://docs.groupdocs.com/redaction/java/redaction-basics/)
* More advanced redaction topics: [Advanced usage](../https://docs.groupdocs.com/redaction/java/advanced-usage/)

<br />


## Constructors

| Constructor | Beschrijving |
| --- | --- |
|  | [Redactor(String filePath)](#Redactor-java.lang.String-) | Initialiseert een nieuw exemplaar van |
Redactor
klasse met bestandspad.
|
|  | [Redactor(InputStream document)](#Redactor-java.io.InputStream-) | Initialiseert een nieuw exemplaar van |
Redactor
klasse met stream.
|
|  | [Redactor(String filePath, LoadOptions loadOptions)](#Redactor-java.lang.String-com.groupdocs.redaction.options.LoadOptions-) | Initialiseert een nieuw exemplaar van |
Redactor
klasse voor een met wachtwoord beveiligd document met zijn pad.
|
|  | [Redactor(String filePath, LoadOptions loadOptions, RedactorSettings settings)](#Redactor-java.lang.String-com.groupdocs.redaction.options.LoadOptions-com.groupdocs.redaction.options.RedactorSettings-) | Initialiseert een nieuw exemplaar van |
Redactor
klasse voor een met wachtwoord beveiligd document met zijn pad en instellingen.
|
|  | [Redactor(InputStream document, LoadOptions loadOptions)](#Redactor-java.io.InputStream-com.groupdocs.redaction.options.LoadOptions-) | Initialiseert een nieuw exemplaar van |
Redactor
klasse voor een met wachtwoord beveiligd document met stream.
|
|  | [Redactor(InputStream document, LoadOptions loadOptions, RedactorSettings settings)](#Redactor-java.io.InputStream-com.groupdocs.redaction.options.LoadOptions-com.groupdocs.redaction.options.RedactorSettings-) | Initialiseert een nieuw exemplaar van |
Redactor
klasse voor een met wachtwoord beveiligd document met stream en instellingen.
|
## Methoden

| Methode | Beschrijving |
| --- | --- |
|  | [close()](#close--) | Vrijgeeft bronnen. |
|
|  | [apply(Redaction redaction)](#apply-com.groupdocs.redaction.Redaction-) | Past een redactie toe op het document. |
|
|  | [apply(Redaction[] redactions)](#apply-com.groupdocs.redaction.Redaction---) | Past een reeks redacties toe op het document. |
|
|  | [apply(RedactionPolicy policy)](#apply-com.groupdocs.redaction.RedactionPolicy-) | Past een redactieregel toe op het document. |
|
|  | [save()](#save--) | Slaat het document op in een bestand met de volgende opties: AddSuffix = true, RasterizeToPDF = true. |
|
|  | [save(SaveOptions saveOptions)](#save-com.groupdocs.redaction.options.SaveOptions-) | Slaat het document op in een bestand. |
|
|  | [save(OutputStream document)](#save-java.io.OutputStream-) | Slaat het document op in een stream. |
|
|  | [save(OutputStream document, SaveOptions saveOptions)](#save-java.io.OutputStream-com.groupdocs.redaction.options.SaveOptions-) | Slaat het document op in een stream. |
|
|  | [save(OutputStream document, RasterizationOptions rasterizationOptions)](#save-java.io.OutputStream-com.groupdocs.redaction.options.RasterizationOptions-) | Slaat het document op in een stream, inclusief aangepaste locatie. |
|
|  | [generatePreview(PreviewOptions previewOptions)](#generatePreview-com.groupdocs.redaction.options.PreviewOptions-) | Genereert voorbeeldafbeeldingen van specifieke pagina's in een gegeven afbeeldingsformaat. |
|
|  | [getDocumentInfo()](#getDocumentInfo--) | Haalt de algemene informatie over het document op - grootte, paginatelling, enz. |
|
### Redactor(String filePath) {#Redactor-java.lang.String-}
```
public Redactor(String filePath)
```


Initialiseert een nieuw exemplaar van
Redactor
klasse met bestandspad.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | filePath | java.lang.String | Pad naar het bestand |


Het volgende voorbeeld toont hoe een document te openen voor redactie.

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
// Hier kunnen we de documentinstantie gebruiken om redactie uit te voeren
}
}
 
``` 
````

|

### Redactor(String filePath, LoadOptions loadOptions) {#Redactor-java.lang.String-com.groupdocs.redaction.options.LoadOptions-}
```
public Redactor(String filePath, LoadOptions loadOptions)
```


Initialiseert een nieuw exemplaar van
Redactor
klasse voor een met wachtwoord beveiligd document met zijn pad.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | filePath | java.lang.String | Pad naar bestand. |
|
|  | loadOptions | [LoadOptions](../../com.groupdocs.redaction.options/loadoptions) | Opties, inclusief wachtwoord. |
|

### Redactor(String filePath, LoadOptions loadOptions, RedactorSettings settings) {#Redactor-java.lang.String-com.groupdocs.redaction.options.LoadOptions-com.groupdocs.redaction.options.RedactorSettings-}
```
public Redactor(String filePath, LoadOptions loadOptions, RedactorSettings settings)
```


Initialiseert een nieuw exemplaar van
Redactor
klasse voor een met wachtwoord beveiligd document met zijn pad en instellingen.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | filePath | java.lang.String | Pad naar bestand. |
|
|  | loadOptions | [LoadOptions](../../com.groupdocs.redaction.options/loadoptions) | Bestandsafhankelijke opties, inclusief wachtwoord. |
|
|  | settings | [RedactorSettings](../../com.groupdocs.redaction.options/redactorsettings) | Standaardinstellingen voor het redactieproces. |
|

### Redactor(InputStream document, LoadOptions loadOptions) {#Redactor-java.io.InputStream-com.groupdocs.redaction.options.LoadOptions-}
```
public Redactor(InputStream document, LoadOptions loadOptions)
```


Initialiseert een nieuw exemplaar van
Redactor
klasse voor een met wachtwoord beveiligd document met stream.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | document | java.io.InputStream | Broninvoerstroom. |
|
|  | loadOptions | [LoadOptions](../../com.groupdocs.redaction.options/loadoptions) | Opties, inclusief wachtwoord. |
|

### Redactor(InputStream document, LoadOptions loadOptions, RedactorSettings settings) {#Redactor-java.io.InputStream-com.groupdocs.redaction.options.LoadOptions-com.groupdocs.redaction.options.RedactorSettings-}
```
public Redactor(InputStream document, LoadOptions loadOptions, RedactorSettings settings)
```


Initialiseert een nieuw exemplaar van
Redactor
klasse voor een met wachtwoord beveiligd document met stream en instellingen.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | document | java.io.InputStream | Broninvoerstroom. |
|
|  | loadOptions | [LoadOptions](../../com.groupdocs.redaction.options/loadoptions) | Opties, inclusief wachtwoord. |
|
|  | settings | [RedactorSettings](../../com.groupdocs.redaction.options/redactorsettings) | Standaardinstellingen voor het redactieproces. |
|

### close() {#close--}
```
public final void close()
```


Vrijgeeft bronnen.


### apply(Redaction redaction) {#apply-com.groupdocs.redaction.Redaction-}
```
public final RedactorChangeLog apply(Redaction redaction)
```


Past een redactie toe op het document.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | redaction | [Redaction](../../com.groupdocs.redaction/redaction) | Een instantie van  Redaction  om toe te passen |
|

**Returns:**
[RedactorChangeLog](../../com.groupdocs.redaction/redactorchangelog) - Success or failure and error message in this case

### apply(Redaction[] redactions) {#apply-com.groupdocs.redaction.Redaction---}
```
public final RedactorChangeLog apply(Redaction[] redactions)
```


Past een reeks redacties toe op het document.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | redactions | [Redaction\[\]](../../com.groupdocs.redaction/redaction) | Een array van redacties om toe te passen |
|

**Returns:**
[RedactorChangeLog](../../com.groupdocs.redaction/redactorchangelog) - Success or failure and error message in this case

### apply(RedactionPolicy policy) {#apply-com.groupdocs.redaction.RedactionPolicy-}
```
public final RedactorChangeLog apply(RedactionPolicy policy)
```


Past een redactieregel toe op het document.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | policy | [RedactionPolicy](../../com.groupdocs.redaction/redactionpolicy) | Redactieregel |
|

**Returns:**
[RedactorChangeLog](../../com.groupdocs.redaction/redactorchangelog) - Success or failure and error message in this case

### save() {#save--}
```
public final String save()
```


Slaat het document op in een bestand met de volgende opties: AddSuffix = true, RasterizeToPDF = true.


**Returns:**
java.lang.String - Pad naar geredigeerd document

### save(SaveOptions saveOptions) {#save-com.groupdocs.redaction.options.SaveOptions-}
```
public final String save(SaveOptions saveOptions)
```


Slaat het document op in een bestand.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | saveOptions | [SaveOptions](../../com.groupdocs.redaction.options/saveoptions) | Opties om een suffix toe te voegen of te rasteren |
|

**Returns:**
java.lang.String - Pad naar geredigeerd document

### save(OutputStream document) {#save-java.io.OutputStream-}
```
public final void save(OutputStream document)
```


Slaat het document op in een stream.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | document | java.io.OutputStream | Doelstream |
|

### save(OutputStream document, SaveOptions saveOptions) {#save-java.io.OutputStream-com.groupdocs.redaction.options.SaveOptions-}
```
public final void save(OutputStream document, SaveOptions saveOptions)
```


Slaat het document op in een stream.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | document | java.io.OutputStream | Doelstream |
|
|  | saveOptions | [SaveOptions](../../com.groupdocs.redaction.options/saveoptions) | Opslaanopties |
|

### save(OutputStream document, RasterizationOptions rasterizationOptions) {#save-java.io.OutputStream-com.groupdocs.redaction.options.RasterizationOptions-}
```
public final void save(OutputStream document, RasterizationOptions rasterizationOptions)
```


Slaat het document op in een stream, inclusief aangepaste locatie.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | document | java.io.OutputStream | Doelstream |
|
|  | rasterizationOptions | [RasterizationOptions](../../com.groupdocs.redaction.options/rasterizationoptions) | Opties om te rasteren of niet en om pagina's voor rasteren op te geven |
|

### generatePreview(PreviewOptions previewOptions) {#generatePreview-com.groupdocs.redaction.options.PreviewOptions-}
```
public final void generatePreview(PreviewOptions previewOptions)
```


Genereert voorbeeldafbeeldingen van specifieke pagina's in een gegeven afbeeldingsformaat.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | previewOptions | [PreviewOptions](../../com.groupdocs.redaction.options/previewoptions) | Afbeeldingseigenschappen en paginabereikinstellingen |
|

### getDocumentInfo() {#getDocumentInfo--}
```
public final IDocumentInfo getDocumentInfo()
```


Haalt de algemene informatie over het document op - grootte, paginatelling, enz.


**Returns:**
[IDocumentInfo](../../com.groupdocs.redaction/idocumentinfo) - An instance of IDocumentInfo

