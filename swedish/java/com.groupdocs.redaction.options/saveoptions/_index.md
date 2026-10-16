---
title: "SaveOptions"
second_title: "GroupDocs.Redaction för Java API-referens"
description: "Tillhandahåller alternativ för att ändra ett utdatafilnamn och/eller konvertera dokumentet till bildbaserad PDF‑rasterisering."
type: docs
weight: 14
url: /sv/java/com.groupdocs.redaction.options/saveoptions/
---
**Inheritance:**
java.lang.Object
```
public class SaveOptions
```

Tillhandahåller alternativ för att ändra namn på utdatafilen och/eller konvertera dokumentet till bildbaserad PDF (rasterisering).

*** ** * ** ***


**Learn more**

* [Save with default options](../https://docs.groupdocs.com/redaction/java/save-with-default-options/)
* [Save in rasterized PDF](../https://docs.groupdocs.com/redaction/java/save-in-rasterized-pdf/)
* [Select specific pages for rasterized PDF](../https://docs.groupdocs.com/redaction/java/select-specific-pages-for-rasterized-pdf/)
* [Save in original format](../https://docs.groupdocs.com/redaction/java/save-in-original-format/)
* [Save overwriting original file](../https://docs.groupdocs.com/redaction/java/save-overwriting-original-file/)
* [Save to stream](../https://docs.groupdocs.com/redaction/java/save-to-stream/)

<br />


## Konstruktörer

| Konstruktor | Beskrivning |
| --- | --- |
|  | [SaveOptions()](#SaveOptions--) | Initierar en ny instans med standardvärden: rasterisera till PDF - false, lägg till suffix - false. |
|
|  | [SaveOptions(boolean rasterizeToPdf, String suffix)](#SaveOptions-boolean-java.lang.String-) | Initierar en ny instans med angivna parametrar. |
|
## Fält

| Fält | Beskrivning |
| --- | --- |
|  | [SaveSuffix](#SaveSuffix) | Representerar standardvärdet för suffix, som är "Redacted". |
|
## Metoder

| Metod | Beskrivning |
| --- | --- |
|  | [getAddSuffix()](#getAddSuffix--) | Hämtar ett värde som indikerar om filnamnet måste ändras innan sparning. |
|
|  | [setAddSuffix(boolean value)](#setAddSuffix-boolean-) | Ställer in ett värde som indikerar om filnamnet måste ändras innan sparning. |
|
|  | [getRedactedFileSuffix()](#getRedactedFileSuffix--) | Hämtar ett anpassat suffix för utdatafilens namn. |
|
|  | [setRedactedFileSuffix(String value)](#setRedactedFileSuffix-java.lang.String-) | Ställer in ett anpassat suffix för utdatafilens namn. |
|
|  | [getRasterizeToPDF()](#getRasterizeToPDF--) | Hämtar ett värde som indikerar om alla sidor i dokumentet måste konverteras till bilder och placeras i en enda PDF-fil. |
|
|  | [setRasterizeToPDF(boolean value)](#setRasterizeToPDF-boolean-) | Ställer in ett värde som indikerar om alla sidor i dokumentet måste konverteras till bilder och placeras i en enda PDF-fil. |
|
|  | [getRasterization()](#getRasterization--) | Hämtar rasteriseringsinställningarna. |
|
|  | [getWordprocessingSaveOptions()](#getWordprocessingSaveOptions--) | Sparaalternativ för ordbehandling. |
|
### SaveOptions() {#SaveOptions--}
```
public SaveOptions()
```


Initierar en ny instans med standardvärden: rasterisera till PDF - false, lägg till suffix - false.


### SaveOptions(boolean rasterizeToPdf, String suffix) {#SaveOptions-boolean-java.lang.String-}
```
public SaveOptions(boolean rasterizeToPdf, String suffix)
```


Initierar en ny instans med angivna parametrar.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | rasterizeToPdf | boolean | Sant, om alla sidor i dokumentet måste konverteras till bilder och placeras i en enda PDF-fil |
|
|  | suffix | java.lang.String | Denna text kommer att läggas till i slutet av filnamnet, om den inte är tom sätter den också AddSuffix till true |
|

### SaveSuffix {#SaveSuffix}
```
public static final String SaveSuffix
```


Representerar standardvärdet för suffix, som är "Redacted".


### getAddSuffix() {#getAddSuffix--}
```
public final boolean getAddSuffix()
```


Hämtar ett värde som indikerar om filnamnet måste ändras innan sparning. Falskt som standard.


**Returns:**
boolean - Ett värde som indikerar om filnamnet måste ändras innan sparning. Falskt som standard.

### setAddSuffix(boolean value) {#setAddSuffix-boolean-}
```
public final void setAddSuffix(boolean value)
```


Ställer in ett värde som indikerar om filnamnet måste ändras innan sparning. Falskt som standard.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | värde | boolean | Ett värde som indikerar om filnamnet måste ändras innan sparning. Falskt som standard. |
|

### getRedactedFileSuffix() {#getRedactedFileSuffix--}
```
public final String getRedactedFileSuffix()
```


Hämtar ett anpassat suffix för utdatafilens namn. Om det inte anges, 
SaveSuffix
konstanten kommer att användas.


**Returns:**
java.lang.String - Ett anpassat suffix för utdatafilens namn. Om det inte anges,  SaveSuffix  konstanten kommer att användas.

### setRedactedFileSuffix(String value) {#setRedactedFileSuffix-java.lang.String-}
```
public final void setRedactedFileSuffix(String value)
```


Ställer in ett anpassat suffix för utdatafilens namn. Om det inte anges, 
SaveSuffix
konstanten kommer att användas.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | värde | java.lang.String | Ett anpassat suffix för utdatafilens namn. Om det inte anges, kommer konstanten  SaveSuffix  att användas. |
|

### getRasterizeToPDF() {#getRasterizeToPDF--}
```
public final boolean getRasterizeToPDF()
```


Hämtar ett värde som indikerar om alla sidor i dokumentet måste konverteras till bilder och placeras i en enda PDF-fil.


**Returns:**
boolean - Ett värde som indikerar om alla sidor i dokumentet ska konverteras till bilder och placeras i en enda PDF‑fil.

### setRasterizeToPDF(boolean value) {#setRasterizeToPDF-boolean-}
```
public final void setRasterizeToPDF(boolean value)
```


Ställer in ett värde som indikerar om alla sidor i dokumentet måste konverteras till bilder och placeras i en enda PDF-fil.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | värde | boolean | Ett värde som indikerar om alla sidor i dokumentet ska konverteras till bilder och placeras i en enda PDF‑fil. |
|

### getRasterization() {#getRasterization--}
```
public final RasterizationOptions getRasterization()
```


Hämtar rasteriseringsinställningarna.


**Returns:**
[RasterizationOptions](../../com.groupdocs.redaction.options/rasterizationoptions) - The rasterization settings.

### getWordprocessingSaveOptions() {#getWordprocessingSaveOptions--}
```
public final WordprocessingSaveOptions getWordprocessingSaveOptions()
```


Sparaalternativ för ordbehandling.


**Returns:**
[WordprocessingSaveOptions](../../com.groupdocs.redaction.options/wordprocessingsaveoptions)
