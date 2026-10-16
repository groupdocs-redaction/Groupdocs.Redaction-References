---
title: "RasterizationOptions"
second_title: "GroupDocs.Redaction для Java API Reference"
description: "Предоставляет параметры для преобразования файлов в PDF."
type: docs
weight: 12
url: /ru/java/com.groupdocs.redaction.options/rasterizationoptions/
---
**Inheritance:**
java.lang.Object
```
public class RasterizationOptions
```

Предоставляет параметры для преобразования файлов в PDF.

*** ** * ** ***


**Learn more**

* More details about saving document as a rasterized PDF: [Save in rasterized PDF](../https://docs.groupdocs.com/redaction/java/save-in-rasterized-pdf/)
* More details about rasterization options: [Select specific pages for rasterized PDF](../https://docs.groupdocs.com/redaction/java/select-specific-pages-for-rasterized-pdf/)

<br />


## Конструкторы

| Конструктор | Описание |
| --- | --- |
|  | [RasterizationOptions()](#RasterizationOptions--) | Инициализирует новый экземпляр. |
|
## Методы

| Метод | Описание |
| --- | --- |
|  | [getEnabled()](#getEnabled--) | Возвращает значение, указывающее, нужно ли конвертировать все страницы документа в изображения и поместить их в один PDF‑файл. |
|
|  | [setEnabled(boolean value)](#setEnabled-boolean-) | Устанавливает значение, указывающее, нужно ли конвертировать все страницы документа в изображения и поместить их в один PDF‑файл. |
|
|  | [getPageIndex()](#getPageIndex--) | Получает индекс первой страницы (нумерация с нуля) для преобразования в PDF. |
|
|  | [setPageIndex(int value)](#setPageIndex-int-) | Устанавливает индекс первой страницы (нумерация с нуля) для преобразования в PDF. |
|
|  | [isStartPageIndexSet()](#isStartPageIndexSet--) | Получает значение, указывающее, был ли изменён (установлен) свойство PageIndex после его инициализации. |
|
|  | [getPageCount()](#getPageCount--) | Получает количество страниц, которые будут преобразованы в PDF. |
|
|  | [setPageCount(int value)](#setPageCount-int-) | Устанавливает количество страниц, которые будут преобразованы в PDF. |
|
|  | [isPageCountSet()](#isPageCountSet--) | Возвращает значение, указывающее, было ли изменено свойство PageCount (установлено) после его инициализации. |
|
|  | [getCompliance()](#getCompliance--) | Возвращает уровень соответствия PDF. |
|
|  | [setCompliance(PdfComplianceLevel value)](#setCompliance-com.groupdocs.redaction.options.PdfComplianceLevel-) | Устанавливает уровень соответствия PDF. |
|
|  | [hasAdvancedOptions()](#hasAdvancedOptions--) | Возвращает индикатор, который истинный, если заданы расширенные параметры растеризации. |
|
|  | [addAdvancedOption(AdvancedRasterizationOptions optionType)](#addAdvancedOption-com.groupdocs.redaction.options.AdvancedRasterizationOptions-) | Вы можете использовать этот метод для регистрации расширенной опции растеризации, которую следует применить. |
|
|  | [addAdvancedOption(AdvancedRasterizationOptions optionType, HashMap<String,String> parameters)](#addAdvancedOption-com.groupdocs.redaction.options.AdvancedRasterizationOptions-java.util.HashMap-java.lang.String-java.lang.String--) | Вы можете использовать этот метод для регистрации расширенной опции растеризации, которую следует применить. |
|
### RasterizationOptions() {#RasterizationOptions--}
```
public RasterizationOptions()
```


Инициализирует новый экземпляр.


### getEnabled() {#getEnabled--}
```
public final boolean getEnabled()
```


Возвращает значение, указывающее, нужно ли преобразовать все страницы документа в изображения и поместить их в один PDF‑файл. По умолчанию TRUE, установите FALSE, чтобы избежать растеризации.


**Returns:**
boolean — Значение, указывающее, нужно ли преобразовать все страницы документа в изображения и поместить их в один PDF‑файл. По умолчанию TRUE, установите FALSE, чтобы избежать растеризации.

### setEnabled(boolean value) {#setEnabled-boolean-}
```
public final void setEnabled(boolean value)
```


Устанавливает значение, указывающее, нужно ли преобразовать все страницы документа в изображения и поместить их в один PDF‑файл. По умолчанию TRUE, установите FALSE, чтобы избежать растеризации.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | значение | boolean | Значение, указывающее, нужно ли преобразовать все страницы документа в изображения и поместить их в один PDF‑файл. По умолчанию TRUE, установите FALSE, чтобы избежать растеризации. |
|

### getPageIndex() {#getPageIndex--}
```
public final int getPageIndex()
```


Получает индекс первой страницы (нумерация с нуля) для преобразования в PDF.


**Returns:**
int — Индекс первой страницы (нумерация с нуля), которую следует преобразовать в PDF.

### setPageIndex(int value) {#setPageIndex-int-}
```
public final void setPageIndex(int value)
```


Устанавливает индекс первой страницы (нумерация с нуля) для преобразования в PDF.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | значение | int | Индекс первой страницы (нумерация с нуля), которую следует преобразовать в PDF. |
|

### isStartPageIndexSet() {#isStartPageIndexSet--}
```
public final boolean isStartPageIndexSet()
```


Получает значение, указывающее, был ли изменён (установлен) свойство PageIndex после его инициализации.


**Returns:**
boolean — Значение, указывающее, было ли изменено свойство PageIndex (установлено) после его инициализации.

### getPageCount() {#getPageCount--}
```
public final int getPageCount()
```


Получает количество страниц, которые будут преобразованы в PDF.


**Returns:**
int — Количество страниц, которые будут преобразованы в PDF.

### setPageCount(int value) {#setPageCount-int-}
```
public final void setPageCount(int value)
```


Устанавливает количество страниц, которые будут преобразованы в PDF.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | значение | int | Количество страниц, которые будут преобразованы в PDF. |
|

### isPageCountSet() {#isPageCountSet--}
```
public final boolean isPageCountSet()
```


Возвращает значение, указывающее, было ли изменено свойство PageCount (установлено) после его инициализации.


**Returns:**
boolean — Значение, указывающее, было ли изменено свойство PageCount (установлено) после его инициализации.

### getCompliance() {#getCompliance--}
```
public final PdfComplianceLevel getCompliance()
```


Возвращает уровень соответствия PDF.


**Returns:**
[PdfComplianceLevel](../../com.groupdocs.redaction.options/pdfcompliancelevel) - The PDF Compliance level.

### setCompliance(PdfComplianceLevel value) {#setCompliance-com.groupdocs.redaction.options.PdfComplianceLevel-}
```
public final void setCompliance(PdfComplianceLevel value)
```


Устанавливает уровень соответствия PDF.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | value | [PdfComplianceLevel](../../com.groupdocs.redaction.options/pdfcompliancelevel) | Уровень соответствия PDF. |
|

### hasAdvancedOptions() {#hasAdvancedOptions--}
```
public final boolean hasAdvancedOptions()
```


Возвращает индикатор, который истинный, если заданы расширенные параметры растеризации.


**Returns:**
boolean — Индикатор, который истинный, если заданы расширенные параметры растеризации.

### addAdvancedOption(AdvancedRasterizationOptions optionType) {#addAdvancedOption-com.groupdocs.redaction.options.AdvancedRasterizationOptions-}
```
public final void addAdvancedOption(AdvancedRasterizationOptions optionType)
```


Вы можете использовать этот метод для регистрации расширенной опции растеризации, которую следует применить.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | optionType | [AdvancedRasterizationOptions](../../com.groupdocs.redaction.options/advancedrasterizationoptions) | Предоставляет информацию о выбранном типе эффекта (оттенки серого, рамка и т.д.). |
|

### addAdvancedOption(AdvancedRasterizationOptions optionType, HashMap<String,String> parameters) {#addAdvancedOption-com.groupdocs.redaction.options.AdvancedRasterizationOptions-java.util.HashMap-java.lang.String-java.lang.String--}
```
public final void addAdvancedOption(AdvancedRasterizationOptions optionType, HashMap<String,String> parameters)
```


Вы можете использовать этот метод для регистрации расширенной опции растеризации, которую следует применить.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | optionType | [AdvancedRasterizationOptions](../../com.groupdocs.redaction.options/advancedrasterizationoptions) | Предоставляет информацию о выбранном типе эффекта (оттенки серого, рамка и т.д.). |
|
|  | параметры | java.util.HashMap<java.lang.String,java.lang.String> | Параметры для заданного эффекта, такие как угол поворота |
|

