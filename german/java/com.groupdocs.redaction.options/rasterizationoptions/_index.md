---
title: "RasterizationOptions"
second_title: "GroupDocs.Redaction for Java API-Referenz"
description: "Stellt Optionen zum Konvertieren von Dateien in PDF bereit."
type: docs
weight: 12
url: /de/java/com.groupdocs.redaction.options/rasterizationoptions/
---
**Inheritance:**
java.lang.Object
```
public class RasterizationOptions
```

Stellt Optionen zum Konvertieren von Dateien in PDF bereit.

*** ** * ** ***


**Learn more**

* More details about saving document as a rasterized PDF: [Save in rasterized PDF](../https://docs.groupdocs.com/redaction/java/save-in-rasterized-pdf/)
* More details about rasterization options: [Select specific pages for rasterized PDF](../https://docs.groupdocs.com/redaction/java/select-specific-pages-for-rasterized-pdf/)

<br />


## Konstruktoren

| Konstruktor | Beschreibung |
| --- | --- |
|  | [RasterizationOptions()](#RasterizationOptions--) | Initialisiert eine neue Instanz. |
|
## Methoden

| Methode | Beschreibung |
| --- | --- |
|  | [getEnabled()](#getEnabled--) | Gibt einen Wert zurück, der angibt, ob alle Seiten im Dokument in Bilder konvertiert und in einer einzigen PDF-Datei zusammengefasst werden sollen. |
|
|  | [setEnabled(boolean value)](#setEnabled-boolean-) | Setzt einen Wert, der angibt, ob alle Seiten im Dokument in Bilder konvertiert und in einer einzigen PDF-Datei zusammengefasst werden sollen. |
|
|  | [getPageIndex()](#getPageIndex--) | Liefert den Index der ersten Seite (0‑basiert), die in PDF konvertiert werden soll. |
|
|  | [setPageIndex(int value)](#setPageIndex-int-) | Setzt den Index der ersten Seite (0‑basiert), die in PDF konvertiert werden soll. |
|
|  | [isStartPageIndexSet()](#isStartPageIndexSet--) | Liefert einen Wert, der angibt, ob die PageIndex‑Eigenschaft nach ihrer Initialisierung geändert (gesetzt) wurde. |
|
|  | [getPageCount()](#getPageCount--) | Liefert die Anzahl der Seiten, die in PDF konvertiert werden sollen. |
|
|  | [setPageCount(int value)](#setPageCount-int-) | Setzt die Anzahl der Seiten, die in PDF konvertiert werden sollen. |
|
|  | [isPageCountSet()](#isPageCountSet--) | Liefert einen Wert, der angibt, ob die PageCount‑Eigenschaft nach ihrer Initialisierung geändert (gesetzt) wurde. |
|
|  | [getCompliance()](#getCompliance--) | Liefert das PDF‑Compliance‑Level. |
|
|  | [setCompliance(PdfComplianceLevel value)](#setCompliance-com.groupdocs.redaction.options.PdfComplianceLevel-) | Setzt das PDF‑Compliance‑Level. |
|
|  | [hasAdvancedOptions()](#hasAdvancedOptions--) | Liefert einen Indikator, der wahr ist, wenn erweiterte Rasterisierungsoptionen gesetzt sind. |
|
|  | [addAdvancedOption(AdvancedRasterizationOptions optionType)](#addAdvancedOption-com.groupdocs.redaction.options.AdvancedRasterizationOptions-) | Sie können diese Methode verwenden, um eine anzuwendende erweiterte Rasterisierungsoption zu registrieren. |
|
|  | [addAdvancedOption(AdvancedRasterizationOptions optionType, HashMap<String,String> parameters)](#addAdvancedOption-com.groupdocs.redaction.options.AdvancedRasterizationOptions-java.util.HashMap-java.lang.String-java.lang.String--) | Sie können diese Methode verwenden, um eine anzuwendende erweiterte Rasterisierungsoption zu registrieren. |
|
### RasterizationOptions() {#RasterizationOptions--}
```
public RasterizationOptions()
```


Initialisiert eine neue Instanz.


### getEnabled() {#getEnabled--}
```
public final boolean getEnabled()
```


Liefert einen Wert, der angibt, ob alle Seiten im Dokument in Bilder konvertiert und in einer einzigen PDF‑Datei abgelegt werden müssen. Standardmäßig TRUE, auf FALSE setzen, um Rasterisierung zu vermeiden.


**Returns:**
boolean - Ein Wert, der angibt, ob alle Seiten im Dokument in Bilder konvertiert und in einer einzigen PDF‑Datei abgelegt werden müssen. Standardmäßig TRUE, auf FALSE setzen, um Rasterisierung zu vermeiden.

### setEnabled(boolean value) {#setEnabled-boolean-}
```
public final void setEnabled(boolean value)
```


Setzt einen Wert, der angibt, ob alle Seiten im Dokument in Bilder konvertiert und in einer einzigen PDF‑Datei abgelegt werden müssen. Standardmäßig TRUE, auf FALSE setzen, um Rasterisierung zu vermeiden.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | Wert | boolean | Ein Wert, der angibt, ob alle Seiten im Dokument in Bilder konvertiert und in einer einzigen PDF‑Datei abgelegt werden müssen. Standardmäßig TRUE, auf FALSE setzen, um Rasterisierung zu vermeiden. |
|

### getPageIndex() {#getPageIndex--}
```
public final int getPageIndex()
```


Liefert den Index der ersten Seite (0‑basiert), die in PDF konvertiert werden soll.


**Returns:**
int - Der Index der ersten Seite (0‑basiert), die in PDF konvertiert werden soll.

### setPageIndex(int value) {#setPageIndex-int-}
```
public final void setPageIndex(int value)
```


Setzt den Index der ersten Seite (0‑basiert), die in PDF konvertiert werden soll.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | Wert | int | Der Index der ersten Seite (0‑basiert), die in PDF konvertiert werden soll. |
|

### isStartPageIndexSet() {#isStartPageIndexSet--}
```
public final boolean isStartPageIndexSet()
```


Liefert einen Wert, der angibt, ob die PageIndex‑Eigenschaft nach ihrer Initialisierung geändert (gesetzt) wurde.


**Returns:**
boolean - Ein Wert, der angibt, ob die PageIndex‑Eigenschaft nach ihrer Initialisierung geändert (gesetzt) wurde.

### getPageCount() {#getPageCount--}
```
public final int getPageCount()
```


Liefert die Anzahl der Seiten, die in PDF konvertiert werden sollen.


**Returns:**
int - Die Anzahl der Seiten, die in PDF konvertiert werden sollen.

### setPageCount(int value) {#setPageCount-int-}
```
public final void setPageCount(int value)
```


Setzt die Anzahl der Seiten, die in PDF konvertiert werden sollen.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | Wert | int | Die Anzahl der Seiten, die in PDF konvertiert werden sollen. |
|

### isPageCountSet() {#isPageCountSet--}
```
public final boolean isPageCountSet()
```


Liefert einen Wert, der angibt, ob die PageCount‑Eigenschaft nach ihrer Initialisierung geändert (gesetzt) wurde.


**Returns:**
boolean - Ein Wert, der angibt, ob die PageCount-Eigenschaft nach ihrer Initialisierung geändert (gesetzt) wurde.

### getCompliance() {#getCompliance--}
```
public final PdfComplianceLevel getCompliance()
```


Liefert das PDF‑Compliance‑Level.


**Returns:**
[PdfComplianceLevel](../../com.groupdocs.redaction.options/pdfcompliancelevel) - The PDF Compliance level.

### setCompliance(PdfComplianceLevel value) {#setCompliance-com.groupdocs.redaction.options.PdfComplianceLevel-}
```
public final void setCompliance(PdfComplianceLevel value)
```


Setzt das PDF‑Compliance‑Level.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | value | [PdfComplianceLevel](../../com.groupdocs.redaction.options/pdfcompliancelevel) | Das PDF-Compliance-Level. |
|

### hasAdvancedOptions() {#hasAdvancedOptions--}
```
public final boolean hasAdvancedOptions()
```


Liefert einen Indikator, der wahr ist, wenn erweiterte Rasterisierungsoptionen gesetzt sind.


**Returns:**
boolean - Ein Indikator, der wahr ist, wenn erweiterte Rasterisierungsoptionen gesetzt sind.

### addAdvancedOption(AdvancedRasterizationOptions optionType) {#addAdvancedOption-com.groupdocs.redaction.options.AdvancedRasterizationOptions-}
```
public final void addAdvancedOption(AdvancedRasterizationOptions optionType)
```


Sie können diese Methode verwenden, um eine anzuwendende erweiterte Rasterisierungsoption zu registrieren.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | optionType | [AdvancedRasterizationOptions](../../com.groupdocs.redaction.options/advancedrasterizationoptions) | Gibt Informationen über den ausgewählten Effekttyp (Graustufen, Rand usw.). |
|

### addAdvancedOption(AdvancedRasterizationOptions optionType, HashMap<String,String> parameters) {#addAdvancedOption-com.groupdocs.redaction.options.AdvancedRasterizationOptions-java.util.HashMap-java.lang.String-java.lang.String--}
```
public final void addAdvancedOption(AdvancedRasterizationOptions optionType, HashMap<String,String> parameters)
```


Sie können diese Methode verwenden, um eine anzuwendende erweiterte Rasterisierungsoption zu registrieren.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | optionType | [AdvancedRasterizationOptions](../../com.groupdocs.redaction.options/advancedrasterizationoptions) | Gibt Informationen über den ausgewählten Effekttyp (Graustufen, Rand usw.). |
|
|  | Parameter | java.util.HashMap<java.lang.String,java.lang.String> | Parameter für den angegebenen Effekt, wie z. B. den Rotationswinkel |
|

