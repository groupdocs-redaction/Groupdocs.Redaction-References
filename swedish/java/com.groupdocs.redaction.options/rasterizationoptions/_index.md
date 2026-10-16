---
title: "RasterizationOptions"
second_title: "GroupDocs.Redaction för Java API-referens"
description: "Tillhandahåller alternativ för att konvertera filer till PDF."
type: docs
weight: 12
url: /sv/java/com.groupdocs.redaction.options/rasterizationoptions/
---
**Inheritance:**
java.lang.Object
```
public class RasterizationOptions
```

Tillhandahåller alternativ för att konvertera filer till PDF.

*** ** * ** ***


**Learn more**

* More details about saving document as a rasterized PDF: [Save in rasterized PDF](../https://docs.groupdocs.com/redaction/java/save-in-rasterized-pdf/)
* More details about rasterization options: [Select specific pages for rasterized PDF](../https://docs.groupdocs.com/redaction/java/select-specific-pages-for-rasterized-pdf/)

<br />


## Konstruktörer

| Konstruktor | Beskrivning |
| --- | --- |
|  | [RasterizationOptions()](#RasterizationOptions--) | Initierar en ny instans. |
|
## Metoder

| Metod | Beskrivning |
| --- | --- |
|  | [getEnabled()](#getEnabled--) | Hämtar ett värde som indikerar om alla sidor i dokumentet måste konverteras till bilder och placeras i en enda PDF-fil. |
|
|  | [setEnabled(boolean value)](#setEnabled-boolean-) | Ställer in ett värde som indikerar om alla sidor i dokumentet måste konverteras till bilder och placeras i en enda PDF-fil. |
|
|  | [getPageIndex()](#getPageIndex--) | Hämtar indexet för den första sidan (0-baserad) som ska konverteras till PDF. |
|
|  | [setPageIndex(int value)](#setPageIndex-int-) | Ställer in indexet för den första sidan (0-baserad) som ska konverteras till PDF. |
|
|  | [isStartPageIndexSet()](#isStartPageIndexSet--) | Hämtar ett värde som indikerar om PageIndex-egenskapen ändrades (sattes) efter dess initiering. |
|
|  | [getPageCount()](#getPageCount--) | Hämtar antalet sidor som ska konverteras till PDF. |
|
|  | [setPageCount(int value)](#setPageCount-int-) | Ställer in antalet sidor som ska konverteras till PDF. |
|
|  | [isPageCountSet()](#isPageCountSet--) | Hämtar ett värde som indikerar om egenskapen PageCount ändrades (sattes) efter dess initiering. |
|
|  | [getCompliance()](#getCompliance--) | Hämtar PDF‑efterlevnadsnivån. |
|
|  | [setCompliance(PdfComplianceLevel value)](#setCompliance-com.groupdocs.redaction.options.PdfComplianceLevel-) | Ställer in PDF‑efterlevnadsnivån. |
|
|  | [hasAdvancedOptions()](#hasAdvancedOptions--) | Hämtar en indikator som är sann om avancerade rasteriseringsalternativ är inställda. |
|
|  | [addAdvancedOption(AdvancedRasterizationOptions optionType)](#addAdvancedOption-com.groupdocs.redaction.options.AdvancedRasterizationOptions-) | Du kan använda den här metoden för att registrera ett avancerat rasteriseringsalternativ att tillämpa. |
|
|  | [addAdvancedOption(AdvancedRasterizationOptions optionType, HashMap<String,String> parameters)](#addAdvancedOption-com.groupdocs.redaction.options.AdvancedRasterizationOptions-java.util.HashMap-java.lang.String-java.lang.String--) | Du kan använda den här metoden för att registrera ett avancerat rasteriseringsalternativ att tillämpa. |
|
### RasterizationOptions() {#RasterizationOptions--}
```
public RasterizationOptions()
```


Initierar en ny instans.


### getEnabled() {#getEnabled--}
```
public final boolean getEnabled()
```


Hämtar ett värde som indikerar om alla sidor i dokumentet måste konverteras till bilder och placeras i en enda PDF‑fil. TRUE som standard, sätt till FALSE för att undvika rasterisering.


**Returns:**
boolean – Ett värde som indikerar om alla sidor i dokumentet måste konverteras till bilder och placeras i en enda PDF‑fil. TRUE som standard, sätt till FALSE för att undvika rasterisering.

### setEnabled(boolean value) {#setEnabled-boolean-}
```
public final void setEnabled(boolean value)
```


Ställer in ett värde som indikerar om alla sidor i dokumentet måste konverteras till bilder och placeras i en enda PDF‑fil. TRUE som standard, sätt till FALSE för att undvika rasterisering.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | värde | boolean | Ett värde som indikerar om alla sidor i dokumentet måste konverteras till bilder och placeras i en enda PDF‑fil. TRUE som standard, sätt till FALSE för att undvika rasterisering. |
|

### getPageIndex() {#getPageIndex--}
```
public final int getPageIndex()
```


Hämtar indexet för den första sidan (0-baserad) som ska konverteras till PDF.


**Returns:**
int – Indexet för den första sidan (0‑baserat) som ska konverteras till PDF.

### setPageIndex(int value) {#setPageIndex-int-}
```
public final void setPageIndex(int value)
```


Ställer in indexet för den första sidan (0-baserad) som ska konverteras till PDF.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | värde | int | Indexet för den första sidan (0‑baserat) som ska konverteras till PDF. |
|

### isStartPageIndexSet() {#isStartPageIndexSet--}
```
public final boolean isStartPageIndexSet()
```


Hämtar ett värde som indikerar om PageIndex-egenskapen ändrades (sattes) efter dess initiering.


**Returns:**
boolean – Ett värde som indikerar om egenskapen PageIndex ändrades (sattes) efter dess initiering.

### getPageCount() {#getPageCount--}
```
public final int getPageCount()
```


Hämtar antalet sidor som ska konverteras till PDF.


**Returns:**
int – Antalet sidor som ska konverteras till PDF.

### setPageCount(int value) {#setPageCount-int-}
```
public final void setPageCount(int value)
```


Ställer in antalet sidor som ska konverteras till PDF.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | värde | int | Antalet sidor som ska konverteras till PDF. |
|

### isPageCountSet() {#isPageCountSet--}
```
public final boolean isPageCountSet()
```


Hämtar ett värde som indikerar om egenskapen PageCount ändrades (sattes) efter dess initiering.


**Returns:**
boolean – Ett värde som indikerar om egenskapen PageCount ändrades (sattes) efter dess initiering.

### getCompliance() {#getCompliance--}
```
public final PdfComplianceLevel getCompliance()
```


Hämtar PDF‑efterlevnadsnivån.


**Returns:**
[PdfComplianceLevel](../../com.groupdocs.redaction.options/pdfcompliancelevel) - The PDF Compliance level.

### setCompliance(PdfComplianceLevel value) {#setCompliance-com.groupdocs.redaction.options.PdfComplianceLevel-}
```
public final void setCompliance(PdfComplianceLevel value)
```


Ställer in PDF‑efterlevnadsnivån.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | value | [PdfComplianceLevel](../../com.groupdocs.redaction.options/pdfcompliancelevel) | PDF‑efterlevnadsnivån. |
|

### hasAdvancedOptions() {#hasAdvancedOptions--}
```
public final boolean hasAdvancedOptions()
```


Hämtar en indikator som är sann om avancerade rasteriseringsalternativ är inställda.


**Returns:**
boolean – En indikator som är sann om avancerade rasteriseringsalternativ är inställda.

### addAdvancedOption(AdvancedRasterizationOptions optionType) {#addAdvancedOption-com.groupdocs.redaction.options.AdvancedRasterizationOptions-}
```
public final void addAdvancedOption(AdvancedRasterizationOptions optionType)
```


Du kan använda den här metoden för att registrera ett avancerat rasteriseringsalternativ att tillämpa.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | optionType | [AdvancedRasterizationOptions](../../com.groupdocs.redaction.options/advancedrasterizationoptions) | Tillhandahåller information om den valda effekttypen (gråskala, ram osv.) |
|

### addAdvancedOption(AdvancedRasterizationOptions optionType, HashMap<String,String> parameters) {#addAdvancedOption-com.groupdocs.redaction.options.AdvancedRasterizationOptions-java.util.HashMap-java.lang.String-java.lang.String--}
```
public final void addAdvancedOption(AdvancedRasterizationOptions optionType, HashMap<String,String> parameters)
```


Du kan använda den här metoden för att registrera ett avancerat rasteriseringsalternativ att tillämpa.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | optionType | [AdvancedRasterizationOptions](../../com.groupdocs.redaction.options/advancedrasterizationoptions) | Tillhandahåller information om den valda effekttypen (gråskala, ram osv.) |
|
|  | parametrar | java.util.HashMap<java.lang.String,java.lang.String> | Parametrar för den givna effekten, såsom rotationsvinkel |
|

