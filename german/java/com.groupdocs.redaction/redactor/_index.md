---
title: "Redactor"
second_title: "GroupDocs.Redaction for Java API-Referenz"
description: "Stellt eine Hauptklasse dar, die den Dokumenten-Redaktionsprozess steuert und das Öffnen, Redigieren und Speichern von Dokumenten ermöglicht."
type: docs
weight: 16
url: /de/java/com.groupdocs.redaction/redactor/
---
**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
java.io.Closeable, [com.groupdocs.redaction.integration.IPreviewable](../../com.groupdocs.redaction.integration/ipreviewable)
```
public final class Redactor implements Closeable, IPreviewable
```

Stellt die Hauptklasse dar, die den Dokumenten-Redaktionsprozess steuert und das Öffnen, Redigieren und Speichern von Dokumenten ermöglicht.

*** ** * ** ***


**Learn more**

* More details about applying redactions: [Redaction basics](../https://docs.groupdocs.com/redaction/java/redaction-basics/)
* More advanced redaction topics: [Advanced usage](../https://docs.groupdocs.com/redaction/java/advanced-usage/)

<br />


## Konstruktoren

| Konstruktor | Beschreibung |
| --- | --- |
|  | [Redactor(String filePath)](#Redactor-java.lang.String-) | Initialisiert eine neue Instanz von |
Redactor
Klasse, die einen Dateipfad verwendet.
|
|  | [Redactor(InputStream document)](#Redactor-java.io.InputStream-) | Initialisiert eine neue Instanz von |
Redactor
Klasse, die einen Stream verwendet.
|
|  | [Redactor(String filePath, LoadOptions loadOptions)](#Redactor-java.lang.String-com.groupdocs.redaction.options.LoadOptions-) | Initialisiert eine neue Instanz von |
Redactor
Klasse für ein passwortgeschütztes Dokument, das seinen Pfad verwendet.
|
|  | [Redactor(String filePath, LoadOptions loadOptions, RedactorSettings settings)](#Redactor-java.lang.String-com.groupdocs.redaction.options.LoadOptions-com.groupdocs.redaction.options.RedactorSettings-) | Initialisiert eine neue Instanz von |
Redactor
Klasse für ein passwortgeschütztes Dokument, das seinen Pfad und Einstellungen verwendet.
|
|  | [Redactor(InputStream document, LoadOptions loadOptions)](#Redactor-java.io.InputStream-com.groupdocs.redaction.options.LoadOptions-) | Initialisiert eine neue Instanz von |
Redactor
Klasse für ein passwortgeschütztes Dokument, das einen Stream verwendet.
|
|  | [Redactor(InputStream document, LoadOptions loadOptions, RedactorSettings settings)](#Redactor-java.io.InputStream-com.groupdocs.redaction.options.LoadOptions-com.groupdocs.redaction.options.RedactorSettings-) | Initialisiert eine neue Instanz von |
Redactor
Klasse für ein passwortgeschütztes Dokument, das einen Stream und Einstellungen verwendet.
|
## Methoden

| Methode | Beschreibung |
| --- | --- |
|  | [close()](#close--) | Gibt Ressourcen frei. |
|
|  | [apply(Redaction redaction)](#apply-com.groupdocs.redaction.Redaction-) | Wendet eine Redaktion auf das Dokument an. |
|
|  | [apply(Redaction[] redactions)](#apply-com.groupdocs.redaction.Redaction---) | Wendet eine Menge von Redaktionen auf das Dokument an. |
|
|  | [apply(RedactionPolicy policy)](#apply-com.groupdocs.redaction.RedactionPolicy-) | Wendet eine Redaktionsrichtlinie auf das Dokument an. |
|
|  | [save()](#save--) | Speichert das Dokument in einer Datei mit den folgenden Optionen: AddSuffix = true, RasterizeToPDF = true. |
|
|  | [save(SaveOptions saveOptions)](#save-com.groupdocs.redaction.options.SaveOptions-) | Speichert das Dokument in einer Datei. |
|
|  | [save(OutputStream document)](#save-java.io.OutputStream-) | Speichert das Dokument in einen Stream. |
|
|  | [save(OutputStream document, SaveOptions saveOptions)](#save-java.io.OutputStream-com.groupdocs.redaction.options.SaveOptions-) | Speichert das Dokument in einen Stream. |
|
|  | [save(OutputStream document, RasterizationOptions rasterizationOptions)](#save-java.io.OutputStream-com.groupdocs.redaction.options.RasterizationOptions-) | Speichert das Dokument in einen Stream, einschließlich benutzerdefiniertem Speicherort. |
|
|  | [generatePreview(PreviewOptions previewOptions)](#generatePreview-com.groupdocs.redaction.options.PreviewOptions-) | Erstellt Vorschaubilder bestimmter Seiten in einem angegebenen Bildformat. |
|
|  | [getDocumentInfo()](#getDocumentInfo--) | Ermittelt die allgemeinen Informationen über das Dokument – Größe, Seitenzahl usw. |
|
### Redactor(String filePath) {#Redactor-java.lang.String-}
```
public Redactor(String filePath)
```


Initialisiert eine neue Instanz von
Redactor
Klasse, die einen Dateipfad verwendet.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | filePath | java.lang.String | Pfad zur Datei |


Das folgende Beispiel zeigt, wie ein Dokument zur Redaktion geöffnet wird.

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
// Hier können wir die Dokumentinstanz verwenden, um Redaktionen durchzuführen
}
}
 
``` 
````

|

### Redactor(String filePath, LoadOptions loadOptions) {#Redactor-java.lang.String-com.groupdocs.redaction.options.LoadOptions-}
```
public Redactor(String filePath, LoadOptions loadOptions)
```


Initialisiert eine neue Instanz von
Redactor
Klasse für ein passwortgeschütztes Dokument, das seinen Pfad verwendet.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | filePath | java.lang.String | Pfad zur Datei. |
|
|  | loadOptions | [LoadOptions](../../com.groupdocs.redaction.options/loadoptions) | Optionen, einschließlich Passwort. |
|

### Redactor(String filePath, LoadOptions loadOptions, RedactorSettings settings) {#Redactor-java.lang.String-com.groupdocs.redaction.options.LoadOptions-com.groupdocs.redaction.options.RedactorSettings-}
```
public Redactor(String filePath, LoadOptions loadOptions, RedactorSettings settings)
```


Initialisiert eine neue Instanz von
Redactor
Klasse für ein passwortgeschütztes Dokument, das seinen Pfad und Einstellungen verwendet.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | filePath | java.lang.String | Pfad zur Datei. |
|
|  | loadOptions | [LoadOptions](../../com.groupdocs.redaction.options/loadoptions) | Dateiabhängige Optionen, einschließlich Passwort. |
|
|  | settings | [RedactorSettings](../../com.groupdocs.redaction.options/redactorsettings) | Standardeinstellungen für den Redaktionsprozess. |
|

### Redactor(InputStream document, LoadOptions loadOptions) {#Redactor-java.io.InputStream-com.groupdocs.redaction.options.LoadOptions-}
```
public Redactor(InputStream document, LoadOptions loadOptions)
```


Initialisiert eine neue Instanz von
Redactor
Klasse für ein passwortgeschütztes Dokument, das einen Stream verwendet.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | Dokument | java.io.InputStream | Quell-Eingabestream. |
|
|  | loadOptions | [LoadOptions](../../com.groupdocs.redaction.options/loadoptions) | Optionen, einschließlich Passwort. |
|

### Redactor(InputStream document, LoadOptions loadOptions, RedactorSettings settings) {#Redactor-java.io.InputStream-com.groupdocs.redaction.options.LoadOptions-com.groupdocs.redaction.options.RedactorSettings-}
```
public Redactor(InputStream document, LoadOptions loadOptions, RedactorSettings settings)
```


Initialisiert eine neue Instanz von
Redactor
Klasse für ein passwortgeschütztes Dokument, das einen Stream und Einstellungen verwendet.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | Dokument | java.io.InputStream | Quell-Eingabestream. |
|
|  | loadOptions | [LoadOptions](../../com.groupdocs.redaction.options/loadoptions) | Optionen, einschließlich Passwort. |
|
|  | settings | [RedactorSettings](../../com.groupdocs.redaction.options/redactorsettings) | Standardeinstellungen für den Redaktionsprozess. |
|

### close() {#close--}
```
public final void close()
```


Gibt Ressourcen frei.


### apply(Redaction redaction) {#apply-com.groupdocs.redaction.Redaction-}
```
public final RedactorChangeLog apply(Redaction redaction)
```


Wendet eine Redaktion auf das Dokument an.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | redaction | [Redaction](../../com.groupdocs.redaction/redaction) | Eine Instanz von  Redaction  zum Anwenden |
|

**Returns:**
[RedactorChangeLog](../../com.groupdocs.redaction/redactorchangelog) - Success or failure and error message in this case

### apply(Redaction[] redactions) {#apply-com.groupdocs.redaction.Redaction---}
```
public final RedactorChangeLog apply(Redaction[] redactions)
```


Wendet eine Menge von Redaktionen auf das Dokument an.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | redactions | [Redaction\[\]](../../com.groupdocs.redaction/redaction) | Ein Array von Redaktionen zum Anwenden |
|

**Returns:**
[RedactorChangeLog](../../com.groupdocs.redaction/redactorchangelog) - Success or failure and error message in this case

### apply(RedactionPolicy policy) {#apply-com.groupdocs.redaction.RedactionPolicy-}
```
public final RedactorChangeLog apply(RedactionPolicy policy)
```


Wendet eine Redaktionsrichtlinie auf das Dokument an.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | policy | [RedactionPolicy](../../com.groupdocs.redaction/redactionpolicy) | Redaktionsrichtlinie |
|

**Returns:**
[RedactorChangeLog](../../com.groupdocs.redaction/redactorchangelog) - Success or failure and error message in this case

### save() {#save--}
```
public final String save()
```


Speichert das Dokument in einer Datei mit den folgenden Optionen: AddSuffix = true, RasterizeToPDF = true.


**Returns:**
java.lang.String - Pfad zum redigierten Dokument

### save(SaveOptions saveOptions) {#save-com.groupdocs.redaction.options.SaveOptions-}
```
public final String save(SaveOptions saveOptions)
```


Speichert das Dokument in einer Datei.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | saveOptions | [SaveOptions](../../com.groupdocs.redaction.options/saveoptions) | Optionen zum Hinzufügen eines Suffixes oder zum Rastern |
|

**Returns:**
java.lang.String - Pfad zum redigierten Dokument

### save(OutputStream document) {#save-java.io.OutputStream-}
```
public final void save(OutputStream document)
```


Speichert das Dokument in einen Stream.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | Dokument | java.io.OutputStream | Ziel-Stream |
|

### save(OutputStream document, SaveOptions saveOptions) {#save-java.io.OutputStream-com.groupdocs.redaction.options.SaveOptions-}
```
public final void save(OutputStream document, SaveOptions saveOptions)
```


Speichert das Dokument in einen Stream.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | Dokument | java.io.OutputStream | Ziel-Stream |
|
|  | saveOptions | [SaveOptions](../../com.groupdocs.redaction.options/saveoptions) | Speicheroptionen |
|

### save(OutputStream document, RasterizationOptions rasterizationOptions) {#save-java.io.OutputStream-com.groupdocs.redaction.options.RasterizationOptions-}
```
public final void save(OutputStream document, RasterizationOptions rasterizationOptions)
```


Speichert das Dokument in einen Stream, einschließlich benutzerdefiniertem Speicherort.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | Dokument | java.io.OutputStream | Ziel-Stream |
|
|  | rasterizationOptions | [RasterizationOptions](../../com.groupdocs.redaction.options/rasterizationoptions) | Optionen zum Rastern oder Nicht-Rastern und zum Festlegen von Seiten für das Rastern |
|

### generatePreview(PreviewOptions previewOptions) {#generatePreview-com.groupdocs.redaction.options.PreviewOptions-}
```
public final void generatePreview(PreviewOptions previewOptions)
```


Erstellt Vorschaubilder bestimmter Seiten in einem angegebenen Bildformat.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | previewOptions | [PreviewOptions](../../com.groupdocs.redaction.options/previewoptions) | Bildeigenschaften und Einstellungen für den Seitenbereich |
|

### getDocumentInfo() {#getDocumentInfo--}
```
public final IDocumentInfo getDocumentInfo()
```


Ermittelt die allgemeinen Informationen über das Dokument – Größe, Seitenzahl usw.


**Returns:**
[IDocumentInfo](../../com.groupdocs.redaction/idocumentinfo) - An instance of IDocumentInfo

