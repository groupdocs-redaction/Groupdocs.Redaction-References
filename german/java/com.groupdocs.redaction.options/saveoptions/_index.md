---
title: "SaveOptions"
second_title: "GroupDocs.Redaction for Java API-Referenz"
description: "Bietet Optionen zum Ändern eines Ausgabedateinamens und/oder zum Konvertieren des Dokuments in bildbasierte PDF-Rasterung."
type: docs
weight: 14
url: /de/java/com.groupdocs.redaction.options/saveoptions/
---
**Inheritance:**
java.lang.Object
```
public class SaveOptions
```

Bietet Optionen zum Ändern eines Ausgabedateinamens und/oder zur Konvertierung des Dokuments in ein bildbasiertes PDF (Rasterisierung).

*** ** * ** ***


**Learn more**

* [Save with default options](../https://docs.groupdocs.com/redaction/java/save-with-default-options/)
* [Save in rasterized PDF](../https://docs.groupdocs.com/redaction/java/save-in-rasterized-pdf/)
* [Select specific pages for rasterized PDF](../https://docs.groupdocs.com/redaction/java/select-specific-pages-for-rasterized-pdf/)
* [Save in original format](../https://docs.groupdocs.com/redaction/java/save-in-original-format/)
* [Save overwriting original file](../https://docs.groupdocs.com/redaction/java/save-overwriting-original-file/)
* [Save to stream](../https://docs.groupdocs.com/redaction/java/save-to-stream/)

<br />


## Konstruktoren

| Konstruktor | Beschreibung |
| --- | --- |
|  | [SaveOptions()](#SaveOptions--) | Initialisiert eine neue Instanz mit Standardwerten: Rasterisierung zu PDF - false, Suffix hinzufügen - false. |
|
|  | [SaveOptions(boolean rasterizeToPdf, String suffix)](#SaveOptions-boolean-java.lang.String-) | Initialisiert eine neue Instanz mit angegebenen Parametern. |
|
## Felder

| Feld | Beschreibung |
| --- | --- |
|  | [SaveSuffix](#SaveSuffix) | Stellt den Standardwert für das Suffix dar, welcher "Redacted" ist. |
|
## Methoden

| Methode | Beschreibung |
| --- | --- |
|  | [getAddSuffix()](#getAddSuffix--) | Gibt einen Wert zurück, der angibt, ob der Dateiname vor dem Speichern geändert werden muss. |
|
|  | [setAddSuffix(boolean value)](#setAddSuffix-boolean-) | Setzt einen Wert, der angibt, ob der Dateiname vor dem Speichern geändert werden muss. |
|
|  | [getRedactedFileSuffix()](#getRedactedFileSuffix--) | Gibt ein benutzerdefiniertes Suffix für den Ausgabedateinamen zurück. |
|
|  | [setRedactedFileSuffix(String value)](#setRedactedFileSuffix-java.lang.String-) | Setzt ein benutzerdefiniertes Suffix für den Ausgabedateinamen. |
|
|  | [getRasterizeToPDF()](#getRasterizeToPDF--) | Gibt einen Wert zurück, der angibt, ob alle Seiten im Dokument in Bilder konvertiert und in einer einzigen PDF-Datei zusammengefasst werden sollen. |
|
|  | [setRasterizeToPDF(boolean value)](#setRasterizeToPDF-boolean-) | Setzt einen Wert, der angibt, ob alle Seiten im Dokument in Bilder konvertiert und in einer einzigen PDF-Datei zusammengefasst werden sollen. |
|
|  | [getRasterization()](#getRasterization--) | Gibt die Rasterisierungseinstellungen zurück. |
|
|  | [getWordprocessingSaveOptions()](#getWordprocessingSaveOptions--) | Speicheroptionen für die Textverarbeitung. |
|
### SaveOptions() {#SaveOptions--}
```
public SaveOptions()
```


Initialisiert eine neue Instanz mit Standardwerten: Rasterisierung zu PDF - false, Suffix hinzufügen - false.


### SaveOptions(boolean rasterizeToPdf, String suffix) {#SaveOptions-boolean-java.lang.String-}
```
public SaveOptions(boolean rasterizeToPdf, String suffix)
```


Initialisiert eine neue Instanz mit angegebenen Parametern.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | rasterizeToPdf | boolean | True, wenn alle Seiten im Dokument in Bilder konvertiert und in einer einzigen PDF-Datei zusammengefasst werden sollen |
|
|  | suffix | java.lang.String | Dieser Text wird an das Ende des Dateinamens angehängt, wenn er nicht leer ist, setzt außerdem AddSuffix auf true. |
|

### SaveSuffix {#SaveSuffix}
```
public static final String SaveSuffix
```


Stellt den Standardwert für das Suffix dar, welcher "Redacted" ist.


### getAddSuffix() {#getAddSuffix--}
```
public final boolean getAddSuffix()
```


Liefert einen Wert, der angibt, ob der Dateiname vor dem Speichern geändert werden muss. Standardmäßig false.


**Returns:**
boolean - Ein Wert, der angibt, ob der Dateiname vor dem Speichern geändert werden muss. Standardmäßig false.

### setAddSuffix(boolean value) {#setAddSuffix-boolean-}
```
public final void setAddSuffix(boolean value)
```


Setzt einen Wert, der angibt, ob der Dateiname vor dem Speichern geändert werden muss. Standardmäßig false.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | Wert | boolean | Ein Wert, der angibt, ob der Dateiname vor dem Speichern geändert werden muss. Standardmäßig false. |
|

### getRedactedFileSuffix() {#getRedactedFileSuffix--}
```
public final String getRedactedFileSuffix()
```


Liefert einen benutzerdefinierten Suffix für den Ausgabedateinamen. Wenn er nicht angegeben ist, wird
SaveSuffix
Konstante wird verwendet.


**Returns:**
java.lang.String - Ein benutzerdefinierter Suffix für den Ausgabedateinamen. Wenn er nicht angegeben ist, wird die  SaveSuffix  Konstante verwendet.

### setRedactedFileSuffix(String value) {#setRedactedFileSuffix-java.lang.String-}
```
public final void setRedactedFileSuffix(String value)
```


Setzt einen benutzerdefinierten Suffix für den Ausgabedateinamen. Wenn er nicht angegeben ist, wird
SaveSuffix
Konstante wird verwendet.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | Wert | java.lang.String | Ein benutzerdefinierter Suffix für den Ausgabedateinamen. Wenn er nicht angegeben ist, wird die  SaveSuffix  Konstante verwendet. |
|

### getRasterizeToPDF() {#getRasterizeToPDF--}
```
public final boolean getRasterizeToPDF()
```


Gibt einen Wert zurück, der angibt, ob alle Seiten im Dokument in Bilder konvertiert und in einer einzigen PDF-Datei zusammengefasst werden sollen.


**Returns:**
boolean - Ein Wert, der angibt, ob alle Seiten im Dokument in Bilder konvertiert und in einer einzigen PDF-Datei zusammengefasst werden müssen.

### setRasterizeToPDF(boolean value) {#setRasterizeToPDF-boolean-}
```
public final void setRasterizeToPDF(boolean value)
```


Setzt einen Wert, der angibt, ob alle Seiten im Dokument in Bilder konvertiert und in einer einzigen PDF-Datei zusammengefasst werden sollen.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | Wert | boolean | Ein Wert, der angibt, ob alle Seiten im Dokument in Bilder konvertiert und in einer einzigen PDF-Datei zusammengefasst werden müssen. |
|

### getRasterization() {#getRasterization--}
```
public final RasterizationOptions getRasterization()
```


Gibt die Rasterisierungseinstellungen zurück.


**Returns:**
[RasterizationOptions](../../com.groupdocs.redaction.options/rasterizationoptions) - The rasterization settings.

### getWordprocessingSaveOptions() {#getWordprocessingSaveOptions--}
```
public final WordprocessingSaveOptions getWordprocessingSaveOptions()
```


Speicheroptionen für die Textverarbeitung.


**Returns:**
[WordprocessingSaveOptions](../../com.groupdocs.redaction.options/wordprocessingsaveoptions)
