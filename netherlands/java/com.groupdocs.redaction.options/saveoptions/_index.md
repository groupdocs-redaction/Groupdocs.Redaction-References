---
title: "SaveOptions"
second_title: "GroupDocs.Redaction for Java API-referentie"
description: "Biedt opties om een uitvoerbestandsnaam te wijzigen en/of het document te converteren naar op afbeeldingen gebaseerde PDF-rasterisatie."
type: docs
weight: 14
url: /nl/java/com.groupdocs.redaction.options/saveoptions/
---
**Inheritance:**
java.lang.Object
```
public class SaveOptions
```

Biedt opties om de naam van een uitvoerbestand te wijzigen en/of het document te converteren naar een op afbeeldingen gebaseerde PDF (rasterisatie).

*** ** * ** ***


**Learn more**

* [Save with default options](../https://docs.groupdocs.com/redaction/java/save-with-default-options/)
* [Save in rasterized PDF](../https://docs.groupdocs.com/redaction/java/save-in-rasterized-pdf/)
* [Select specific pages for rasterized PDF](../https://docs.groupdocs.com/redaction/java/select-specific-pages-for-rasterized-pdf/)
* [Save in original format](../https://docs.groupdocs.com/redaction/java/save-in-original-format/)
* [Save overwriting original file](../https://docs.groupdocs.com/redaction/java/save-overwriting-original-file/)
* [Save to stream](../https://docs.groupdocs.com/redaction/java/save-to-stream/)

<br />


## Constructors

| Constructor | Beschrijving |
| --- | --- |
|  | [SaveOptions()](#SaveOptions--) | Initialiseert een nieuwe instantie met standaardwaarden: rasteriseren naar PDF - false, suffix toevoegen - false. |
|
|  | [SaveOptions(boolean rasterizeToPdf, String suffix)](#SaveOptions-boolean-java.lang.String-) | Initialiseert een nieuw exemplaar met de opgegeven parameters. |
|
## Velden

| Veld | Beschrijving |
| --- | --- |
|  | [SaveSuffix](#SaveSuffix) | Stelt de standaard suffixwaarde voor, die "Redacted" is. |
|
## Methoden

| Methode | Beschrijving |
| --- | --- |
|  | [getAddSuffix()](#getAddSuffix--) | Haalt een waarde op die aangeeft of de bestandsnaam moet worden gewijzigd vóór het opslaan. |
|
|  | [setAddSuffix(boolean value)](#setAddSuffix-boolean-) | Stelt een waarde in die aangeeft of de bestandsnaam moet worden gewijzigd vóór het opslaan. |
|
|  | [getRedactedFileSuffix()](#getRedactedFileSuffix--) | Haalt een aangepaste suffix op voor de uitvoerbestandsnaam. |
|
|  | [setRedactedFileSuffix(String value)](#setRedactedFileSuffix-java.lang.String-) | Stelt een aangepaste suffix in voor de uitvoerbestandsnaam. |
|
|  | [getRasterizeToPDF()](#getRasterizeToPDF--) | Haalt een waarde op die aangeeft of alle pagina's in het document moeten worden geconverteerd naar afbeeldingen en in één PDF-bestand moeten worden geplaatst. |
|
|  | [setRasterizeToPDF(boolean value)](#setRasterizeToPDF-boolean-) | Stelt een waarde in die aangeeft of alle pagina's in het document moeten worden geconverteerd naar afbeeldingen en in één PDF-bestand moeten worden geplaatst. |
|
|  | [getRasterization()](#getRasterization--) | Haalt de rasterisatie-instellingen op. |
|
|  | [getWordprocessingSaveOptions()](#getWordprocessingSaveOptions--) | Opslagopties voor tekstverwerking. |
|
### SaveOptions() {#SaveOptions--}
```
public SaveOptions()
```


Initialiseert een nieuwe instantie met standaardwaarden: rasteriseren naar PDF - false, suffix toevoegen - false.


### SaveOptions(boolean rasterizeToPdf, String suffix) {#SaveOptions-boolean-java.lang.String-}
```
public SaveOptions(boolean rasterizeToPdf, String suffix)
```


Initialiseert een nieuw exemplaar met de opgegeven parameters.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | rasterizeToPdf | boolean | True, als alle pagina's in het document moeten worden geconverteerd naar afbeeldingen en in één PDF-bestand moeten worden geplaatst |
|
|  | suffix | java.lang.String | Deze tekst wordt aan het einde van de bestandsnaam toegevoegd; als deze niet leeg is, wordt AddSuffix ook op true gezet. |
|

### SaveSuffix {#SaveSuffix}
```
public static final String SaveSuffix
```


Stelt de standaard suffixwaarde voor, die "Redacted" is.


### getAddSuffix() {#getAddSuffix--}
```
public final boolean getAddSuffix()
```


Haalt een waarde op die aangeeft of de bestandsnaam moet worden gewijzigd vóór het opslaan. Standaard False.


**Returns:**
boolean - Een waarde die aangeeft of de bestandsnaam moet worden gewijzigd vóór het opslaan. Standaard False.

### setAddSuffix(boolean value) {#setAddSuffix-boolean-}
```
public final void setAddSuffix(boolean value)
```


Stelt een waarde in die aangeeft of de bestandsnaam moet worden gewijzigd vóór het opslaan. Standaard False.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | waarde | boolean | Een waarde die aangeeft of de bestandsnaam moet worden gewijzigd vóór het opslaan. Standaard False. |
|

### getRedactedFileSuffix() {#getRedactedFileSuffix--}
```
public final String getRedactedFileSuffix()
```


Haalt een aangepaste suffix op voor de uitvoerbestandsnaam. Als deze niet is gespecificeerd, de
SaveSuffix
constante zal worden gebruikt.


**Returns:**
java.lang.String - Een aangepaste suffix voor de uitvoerbestandsnaam. Als deze niet is gespecificeerd, zal de  SaveSuffix  constante worden gebruikt.

### setRedactedFileSuffix(String value) {#setRedactedFileSuffix-java.lang.String-}
```
public final void setRedactedFileSuffix(String value)
```


Stelt een aangepaste suffix in voor de uitvoerbestandsnaam. Als deze niet is gespecificeerd, de
SaveSuffix
constante zal worden gebruikt.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | waarde | java.lang.String | Een aangepast achtervoegsel voor de uitvoerbestandsnaam. Als het niet is gespecificeerd, wordt de constante  SaveSuffix  gebruikt. |
|

### getRasterizeToPDF() {#getRasterizeToPDF--}
```
public final boolean getRasterizeToPDF()
```


Haalt een waarde op die aangeeft of alle pagina's in het document moeten worden geconverteerd naar afbeeldingen en in één PDF-bestand moeten worden geplaatst.


**Returns:**
boolean - Een waarde die aangeeft of alle pagina's in het document moeten worden geconverteerd naar afbeeldingen en in één PDF-bestand moeten worden geplaatst.

### setRasterizeToPDF(boolean value) {#setRasterizeToPDF-boolean-}
```
public final void setRasterizeToPDF(boolean value)
```


Stelt een waarde in die aangeeft of alle pagina's in het document moeten worden geconverteerd naar afbeeldingen en in één PDF-bestand moeten worden geplaatst.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | waarde | boolean | Een waarde die aangeeft of alle pagina's in het document moeten worden geconverteerd naar afbeeldingen en in één PDF-bestand moeten worden geplaatst. |
|

### getRasterization() {#getRasterization--}
```
public final RasterizationOptions getRasterization()
```


Haalt de rasterisatie-instellingen op.


**Returns:**
[RasterizationOptions](../../com.groupdocs.redaction.options/rasterizationoptions) - The rasterization settings.

### getWordprocessingSaveOptions() {#getWordprocessingSaveOptions--}
```
public final WordprocessingSaveOptions getWordprocessingSaveOptions()
```


Opslagopties voor tekstverwerking.


**Returns:**
[WordprocessingSaveOptions](../../com.groupdocs.redaction.options/wordprocessingsaveoptions)
