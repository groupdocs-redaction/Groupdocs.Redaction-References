---
title: "RasterizationOptions"
second_title: "GroupDocs.Redaction for Java API-referentie"
description: "Biedt opties voor het converteren van bestanden naar PDF."
type: docs
weight: 12
url: /nl/java/com.groupdocs.redaction.options/rasterizationoptions/
---
**Inheritance:**
java.lang.Object
```
public class RasterizationOptions
```

Biedt opties voor het converteren van bestanden naar PDF.

*** ** * ** ***


**Learn more**

* More details about saving document as a rasterized PDF: [Save in rasterized PDF](../https://docs.groupdocs.com/redaction/java/save-in-rasterized-pdf/)
* More details about rasterization options: [Select specific pages for rasterized PDF](../https://docs.groupdocs.com/redaction/java/select-specific-pages-for-rasterized-pdf/)

<br />


## Constructors

| Constructor | Beschrijving |
| --- | --- |
|  | [RasterizationOptions()](#RasterizationOptions--) | Initialiseert een nieuw exemplaar. |
|
## Methoden

| Methode | Beschrijving |
| --- | --- |
|  | [getEnabled()](#getEnabled--) | Haalt een waarde op die aangeeft of alle pagina's in het document moeten worden geconverteerd naar afbeeldingen en in één PDF-bestand moeten worden geplaatst. |
|
|  | [setEnabled(boolean value)](#setEnabled-boolean-) | Stelt een waarde in die aangeeft of alle pagina's in het document moeten worden geconverteerd naar afbeeldingen en in één PDF-bestand moeten worden geplaatst. |
|
|  | [getPageIndex()](#getPageIndex--) | Haalt de index op van de eerste pagina (0-gebaseerd) om te converteren naar PDF. |
|
|  | [setPageIndex(int value)](#setPageIndex-int-) | Stelt de index in van de eerste pagina (0-gebaseerd) om te converteren naar PDF. |
|
|  | [isStartPageIndexSet()](#isStartPageIndexSet--) | Haalt een waarde op die aangeeft of de PageIndex-eigenschap is gewijzigd (ingesteld) na de initialisatie. |
|
|  | [getPageCount()](#getPageCount--) | Haalt het aantal pagina's op die naar PDF moeten worden geconverteerd. |
|
|  | [setPageCount(int value)](#setPageCount-int-) | Stelt het aantal pagina's in dat moet worden geconverteerd naar PDF. |
|
|  | [isPageCountSet()](#isPageCountSet--) | Haalt een waarde op die aangeeft of de PageCount-eigenschap is gewijzigd (ingesteld) na de initialisatie. |
|
|  | [getCompliance()](#getCompliance--) | Haalt het PDF Compliance-niveau op. |
|
|  | [setCompliance(PdfComplianceLevel value)](#setCompliance-com.groupdocs.redaction.options.PdfComplianceLevel-) | Stelt het PDF Compliance-niveau in. |
|
|  | [hasAdvancedOptions()](#hasAdvancedOptions--) | Haalt een indicator op, die waar is als geavanceerde rasterisatie-opties zijn ingesteld. |
|
|  | [addAdvancedOption(AdvancedRasterizationOptions optionType)](#addAdvancedOption-com.groupdocs.redaction.options.AdvancedRasterizationOptions-) | U kunt deze methode gebruiken om een geavanceerde rasterisatie-optie te registreren die moet worden toegepast. |
|
|  | [addAdvancedOption(AdvancedRasterizationOptions optionType, HashMap<String,String> parameters)](#addAdvancedOption-com.groupdocs.redaction.options.AdvancedRasterizationOptions-java.util.HashMap-java.lang.String-java.lang.String--) | U kunt deze methode gebruiken om een geavanceerde rasterisatie-optie te registreren die moet worden toegepast. |
|
### RasterizationOptions() {#RasterizationOptions--}
```
public RasterizationOptions()
```


Initialiseert een nieuw exemplaar.


### getEnabled() {#getEnabled--}
```
public final boolean getEnabled()
```


Haalt een waarde op die aangeeft of alle pagina's in het document moeten worden geconverteerd naar afbeeldingen en in één PDF-bestand moeten worden geplaatst. Standaard TRUE, stel in op FALSE om rasterisatie te vermijden.


**Returns:**
boolean - Een waarde die aangeeft of alle pagina's in het document moeten worden geconverteerd naar afbeeldingen en in één PDF-bestand moeten worden geplaatst. Standaard TRUE, stel in op FALSE om rasterisatie te vermijden.

### setEnabled(boolean value) {#setEnabled-boolean-}
```
public final void setEnabled(boolean value)
```


Stelt een waarde in die aangeeft of alle pagina's in het document moeten worden geconverteerd naar afbeeldingen en in één PDF-bestand moeten worden geplaatst. Standaard TRUE, stel in op FALSE om rasterisatie te vermijden.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | waarde | boolean | Een waarde die aangeeft of alle pagina's in het document moeten worden geconverteerd naar afbeeldingen en in één PDF-bestand moeten worden geplaatst. Standaard TRUE, stel in op FALSE om rasterisatie te vermijden. |
|

### getPageIndex() {#getPageIndex--}
```
public final int getPageIndex()
```


Haalt de index op van de eerste pagina (0-gebaseerd) om te converteren naar PDF.


**Returns:**
int - De index van de eerste pagina (0-gebaseerd) die moet worden geconverteerd naar PDF.

### setPageIndex(int value) {#setPageIndex-int-}
```
public final void setPageIndex(int value)
```


Stelt de index in van de eerste pagina (0-gebaseerd) om te converteren naar PDF.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | waarde | int | De index van de eerste pagina (0-gebaseerd) die moet worden geconverteerd naar PDF. |
|

### isStartPageIndexSet() {#isStartPageIndexSet--}
```
public final boolean isStartPageIndexSet()
```


Haalt een waarde op die aangeeft of de PageIndex-eigenschap is gewijzigd (ingesteld) na de initialisatie.


**Returns:**
boolean - Een waarde die aangeeft of de PageIndex-eigenschap is gewijzigd (ingesteld) na de initialisatie.

### getPageCount() {#getPageCount--}
```
public final int getPageCount()
```


Haalt het aantal pagina's op die naar PDF moeten worden geconverteerd.


**Returns:**
int - Het aantal pagina's dat moet worden geconverteerd naar PDF.

### setPageCount(int value) {#setPageCount-int-}
```
public final void setPageCount(int value)
```


Stelt het aantal pagina's in dat moet worden geconverteerd naar PDF.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | waarde | int | Het aantal pagina's dat moet worden geconverteerd naar PDF. |
|

### isPageCountSet() {#isPageCountSet--}
```
public final boolean isPageCountSet()
```


Haalt een waarde op die aangeeft of de PageCount-eigenschap is gewijzigd (ingesteld) na de initialisatie.


**Returns:**
boolean - Een waarde die aangeeft of de PageCount-eigenschap is gewijzigd (ingesteld) na de initialisatie.

### getCompliance() {#getCompliance--}
```
public final PdfComplianceLevel getCompliance()
```


Haalt het PDF Compliance-niveau op.


**Returns:**
[PdfComplianceLevel](../../com.groupdocs.redaction.options/pdfcompliancelevel) - The PDF Compliance level.

### setCompliance(PdfComplianceLevel value) {#setCompliance-com.groupdocs.redaction.options.PdfComplianceLevel-}
```
public final void setCompliance(PdfComplianceLevel value)
```


Stelt het PDF Compliance-niveau in.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | value | [PdfComplianceLevel](../../com.groupdocs.redaction.options/pdfcompliancelevel) | Het PDF Compliance-niveau. |
|

### hasAdvancedOptions() {#hasAdvancedOptions--}
```
public final boolean hasAdvancedOptions()
```


Haalt een indicator op, die waar is als geavanceerde rasterisatie-opties zijn ingesteld.


**Returns:**
boolean - Een indicator die waar is als geavanceerde rasterisatie-opties zijn ingesteld.

### addAdvancedOption(AdvancedRasterizationOptions optionType) {#addAdvancedOption-com.groupdocs.redaction.options.AdvancedRasterizationOptions-}
```
public final void addAdvancedOption(AdvancedRasterizationOptions optionType)
```


U kunt deze methode gebruiken om een geavanceerde rasterisatie-optie te registreren die moet worden toegepast.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | optionType | [AdvancedRasterizationOptions](../../com.groupdocs.redaction.options/advancedrasterizationoptions) | Biedt informatie over het geselecteerde effecttype (grijstinten, rand, enz.). |
|

### addAdvancedOption(AdvancedRasterizationOptions optionType, HashMap<String,String> parameters) {#addAdvancedOption-com.groupdocs.redaction.options.AdvancedRasterizationOptions-java.util.HashMap-java.lang.String-java.lang.String--}
```
public final void addAdvancedOption(AdvancedRasterizationOptions optionType, HashMap<String,String> parameters)
```


U kunt deze methode gebruiken om een geavanceerde rasterisatie-optie te registreren die moet worden toegepast.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | optionType | [AdvancedRasterizationOptions](../../com.groupdocs.redaction.options/advancedrasterizationoptions) | Biedt informatie over het geselecteerde effecttype (grijstinten, rand, enz.). |
|
|  | parameters | java.util.HashMap<java.lang.String,java.lang.String> | Parameters voor het gegeven effect, zoals rotatiehoek |
|

