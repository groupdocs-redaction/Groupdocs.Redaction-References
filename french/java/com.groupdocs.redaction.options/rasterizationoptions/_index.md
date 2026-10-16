---
title: "RasterizationOptions"
second_title: "Référence API de GroupDocs.Redaction pour Java"
description: "Fournit des options pour convertir des fichiers en PDF."
type: docs
weight: 12
url: /fr/java/com.groupdocs.redaction.options/rasterizationoptions/
---
**Inheritance:**
java.lang.Object
```
public class RasterizationOptions
```

Fournit des options pour convertir des fichiers en PDF.

*** ** * ** ***


**Learn more**

* More details about saving document as a rasterized PDF: [Save in rasterized PDF](../https://docs.groupdocs.com/redaction/java/save-in-rasterized-pdf/)
* More details about rasterization options: [Select specific pages for rasterized PDF](../https://docs.groupdocs.com/redaction/java/select-specific-pages-for-rasterized-pdf/)

<br />


## Constructeurs

| Constructeur | Description |
| --- | --- |
|  | [RasterizationOptions()](#RasterizationOptions--) | Initialise une nouvelle instance. |
|
## Méthodes

| Méthode | Description |
| --- | --- |
|  | [getEnabled()](#getEnabled--) | Obtient une valeur indiquant si toutes les pages du document doivent être converties en images et placées dans un seul fichier PDF. |
|
|  | [setEnabled(boolean value)](#setEnabled-boolean-) | Définit une valeur indiquant si toutes les pages du document doivent être converties en images et placées dans un seul fichier PDF. |
|
|  | [getPageIndex()](#getPageIndex--) | Obtient l'index de la première page (à partir de 0) à convertir en PDF. |
|
|  | [setPageIndex(int value)](#setPageIndex-int-) | Définit l'index de la première page (à partir de 0) à convertir en PDF. |
|
|  | [isStartPageIndexSet()](#isStartPageIndexSet--) | Obtient une valeur indiquant si la propriété PageIndex a été modifiée (définie) après son initialisation. |
|
|  | [getPageCount()](#getPageCount--) | Obtient le nombre de pages à convertir en PDF. |
|
|  | [setPageCount(int value)](#setPageCount-int-) | Définit le nombre de pages à convertir en PDF. |
|
|  | [isPageCountSet()](#isPageCountSet--) | Obtient une valeur indiquant si la propriété PageCount a été modifiée (définie) après son initialisation. |
|
|  | [getCompliance()](#getCompliance--) | Obtient le niveau de conformité PDF. |
|
|  | [setCompliance(PdfComplianceLevel value)](#setCompliance-com.groupdocs.redaction.options.PdfComplianceLevel-) | Définit le niveau de conformité PDF. |
|
|  | [hasAdvancedOptions()](#hasAdvancedOptions--) | Obtient un indicateur, qui est vrai si les options de rasterisation avancées sont définies. |
|
|  | [addAdvancedOption(AdvancedRasterizationOptions optionType)](#addAdvancedOption-com.groupdocs.redaction.options.AdvancedRasterizationOptions-) | Vous pouvez utiliser cette méthode pour enregistrer une option de rasterisation avancée à appliquer. |
|
|  | [addAdvancedOption(AdvancedRasterizationOptions optionType, HashMap<String,String> parameters)](#addAdvancedOption-com.groupdocs.redaction.options.AdvancedRasterizationOptions-java.util.HashMap-java.lang.String-java.lang.String--) | Vous pouvez utiliser cette méthode pour enregistrer une option de rasterisation avancée à appliquer. |
|
### RasterizationOptions() {#RasterizationOptions--}
```
public RasterizationOptions()
```


Initialise une nouvelle instance.


### getEnabled() {#getEnabled--}
```
public final boolean getEnabled()
```


Obtient une valeur indiquant si toutes les pages du document doivent être converties en images et placées dans un seul fichier PDF. TRUE par défaut, définissez à FALSE afin d'éviter la rasterisation.


**Returns:**
booléen - Une valeur indiquant si toutes les pages du document doivent être converties en images et placées dans un seul fichier PDF. TRUE par défaut, définissez à FALSE afin d'éviter la rasterisation.

### setEnabled(boolean value) {#setEnabled-boolean-}
```
public final void setEnabled(boolean value)
```


Définit une valeur indiquant si toutes les pages du document doivent être converties en images et placées dans un seul fichier PDF. TRUE par défaut, définissez à FALSE afin d'éviter la rasterisation.


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | valeur | boolean | Une valeur indiquant si toutes les pages du document doivent être converties en images et placées dans un seul fichier PDF. TRUE par défaut, définissez à FALSE afin d'éviter la rasterisation. |
|

### getPageIndex() {#getPageIndex--}
```
public final int getPageIndex()
```


Obtient l'index de la première page (à partir de 0) à convertir en PDF.


**Returns:**
int - L'index de la première page (à partir de 0) à convertir en PDF.

### setPageIndex(int value) {#setPageIndex-int-}
```
public final void setPageIndex(int value)
```


Définit l'index de la première page (à partir de 0) à convertir en PDF.


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | valeur | int | L'index de la première page (à partir de 0) à convertir en PDF. |
|

### isStartPageIndexSet() {#isStartPageIndexSet--}
```
public final boolean isStartPageIndexSet()
```


Obtient une valeur indiquant si la propriété PageIndex a été modifiée (définie) après son initialisation.


**Returns:**
booléen - Une valeur indiquant si la propriété PageIndex a été modifiée (définie) après son initialisation.

### getPageCount() {#getPageCount--}
```
public final int getPageCount()
```


Obtient le nombre de pages à convertir en PDF.


**Returns:**
int - Le nombre de pages à convertir en PDF.

### setPageCount(int value) {#setPageCount-int-}
```
public final void setPageCount(int value)
```


Définit le nombre de pages à convertir en PDF.


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | valeur | int | Le nombre de pages à convertir en PDF. |
|

### isPageCountSet() {#isPageCountSet--}
```
public final boolean isPageCountSet()
```


Obtient une valeur indiquant si la propriété PageCount a été modifiée (définie) après son initialisation.


**Returns:**
booléen - Une valeur indiquant si la propriété PageCount a été modifiée (définie) après son initialisation.

### getCompliance() {#getCompliance--}
```
public final PdfComplianceLevel getCompliance()
```


Obtient le niveau de conformité PDF.


**Returns:**
[PdfComplianceLevel](../../com.groupdocs.redaction.options/pdfcompliancelevel) - The PDF Compliance level.

### setCompliance(PdfComplianceLevel value) {#setCompliance-com.groupdocs.redaction.options.PdfComplianceLevel-}
```
public final void setCompliance(PdfComplianceLevel value)
```


Définit le niveau de conformité PDF.


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | value | [PdfComplianceLevel](../../com.groupdocs.redaction.options/pdfcompliancelevel) | Le niveau de conformité PDF. |
|

### hasAdvancedOptions() {#hasAdvancedOptions--}
```
public final boolean hasAdvancedOptions()
```


Obtient un indicateur, qui est vrai si les options de rasterisation avancées sont définies.


**Returns:**
booléen - Un indicateur, qui est vrai si les options de rasterisation avancées sont définies.

### addAdvancedOption(AdvancedRasterizationOptions optionType) {#addAdvancedOption-com.groupdocs.redaction.options.AdvancedRasterizationOptions-}
```
public final void addAdvancedOption(AdvancedRasterizationOptions optionType)
```


Vous pouvez utiliser cette méthode pour enregistrer une option de rasterisation avancée à appliquer.


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | optionType | [AdvancedRasterizationOptions](../../com.groupdocs.redaction.options/advancedrasterizationoptions) | Fournit des informations sur le type d'effet sélectionné (niveaux de gris, bordure, etc.) |
|

### addAdvancedOption(AdvancedRasterizationOptions optionType, HashMap<String,String> parameters) {#addAdvancedOption-com.groupdocs.redaction.options.AdvancedRasterizationOptions-java.util.HashMap-java.lang.String-java.lang.String--}
```
public final void addAdvancedOption(AdvancedRasterizationOptions optionType, HashMap<String,String> parameters)
```


Vous pouvez utiliser cette méthode pour enregistrer une option de rasterisation avancée à appliquer.


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | optionType | [AdvancedRasterizationOptions](../../com.groupdocs.redaction.options/advancedrasterizationoptions) | Fournit des informations sur le type d'effet sélectionné (niveaux de gris, bordure, etc.) |
|
|  | paramètres | java.util.HashMap<java.lang.String,java.lang.String> | Paramètres pour l'effet donné, tels que l'angle de rotation |
|

