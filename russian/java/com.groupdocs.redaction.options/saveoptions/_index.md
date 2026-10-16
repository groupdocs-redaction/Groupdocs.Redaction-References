---
title: "SaveOptions"
second_title: "GroupDocs.Redaction для Java API Reference"
description: "Предоставляет параметры для изменения имени выходного файла и/или преобразования документа в растровый PDF на основе изображений."
type: docs
weight: 14
url: /ru/java/com.groupdocs.redaction.options/saveoptions/
---
**Inheritance:**
java.lang.Object
```
public class SaveOptions
```

Предоставляет параметры для изменения имени выходного файла и/или преобразования документа в PDF на основе изображений (растеризация).

*** ** * ** ***


**Learn more**

* [Save with default options](../https://docs.groupdocs.com/redaction/java/save-with-default-options/)
* [Save in rasterized PDF](../https://docs.groupdocs.com/redaction/java/save-in-rasterized-pdf/)
* [Select specific pages for rasterized PDF](../https://docs.groupdocs.com/redaction/java/select-specific-pages-for-rasterized-pdf/)
* [Save in original format](../https://docs.groupdocs.com/redaction/java/save-in-original-format/)
* [Save overwriting original file](../https://docs.groupdocs.com/redaction/java/save-overwriting-original-file/)
* [Save to stream](../https://docs.groupdocs.com/redaction/java/save-to-stream/)

<br />


## Конструкторы

| Конструктор | Описание |
| --- | --- |
|  | [SaveOptions()](#SaveOptions--) | Инициализирует новый экземпляр со значениями по умолчанию: растеризовать в PDF — false, добавить суффикс — false. |
|
|  | [SaveOptions(boolean rasterizeToPdf, String suffix)](#SaveOptions-boolean-java.lang.String-) | Инициализирует новый экземпляр с заданными параметрами. |
|
## Поля

| Поле | Описание |
| --- | --- |
|  | [SaveSuffix](#SaveSuffix) | Представляет значение суффикса по умолчанию, которое равно "Redacted". |
|
## Методы

| Метод | Описание |
| --- | --- |
|  | [getAddSuffix()](#getAddSuffix--) | Возвращает значение, указывающее, необходимо ли изменить имя файла перед сохранением. |
|
|  | [setAddSuffix(boolean value)](#setAddSuffix-boolean-) | Устанавливает значение, указывающее, необходимо ли изменить имя файла перед сохранением. |
|
|  | [getRedactedFileSuffix()](#getRedactedFileSuffix--) | Возвращает пользовательский суффикс для имени выходного файла. |
|
|  | [setRedactedFileSuffix(String value)](#setRedactedFileSuffix-java.lang.String-) | Устанавливает пользовательский суффикс для имени выходного файла. |
|
|  | [getRasterizeToPDF()](#getRasterizeToPDF--) | Возвращает значение, указывающее, нужно ли конвертировать все страницы документа в изображения и поместить их в один PDF‑файл. |
|
|  | [setRasterizeToPDF(boolean value)](#setRasterizeToPDF-boolean-) | Устанавливает значение, указывающее, нужно ли конвертировать все страницы документа в изображения и поместить их в один PDF‑файл. |
|
|  | [getRasterization()](#getRasterization--) | Возвращает настройки растеризации. |
|
|  | [getWordprocessingSaveOptions()](#getWordprocessingSaveOptions--) | Параметры сохранения обработки текста. |
|
### SaveOptions() {#SaveOptions--}
```
public SaveOptions()
```


Инициализирует новый экземпляр со значениями по умолчанию: растеризовать в PDF — false, добавить суффикс — false.


### SaveOptions(boolean rasterizeToPdf, String suffix) {#SaveOptions-boolean-java.lang.String-}
```
public SaveOptions(boolean rasterizeToPdf, String suffix)
```


Инициализирует новый экземпляр с заданными параметрами.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | rasterizeToPdf | boolean | True, если все страницы документа необходимо конвертировать в изображения и поместить их в один PDF‑файл |
|
|  | suffix | java.lang.String | Этот текст будет добавлен в конец имени файла; если он не пустой, также устанавливает AddSuffix в true |
|

### SaveSuffix {#SaveSuffix}
```
public static final String SaveSuffix
```


Представляет значение суффикса по умолчанию, которое равно "Redacted".


### getAddSuffix() {#getAddSuffix--}
```
public final boolean getAddSuffix()
```


Возвращает значение, указывающее, необходимо ли изменить имя файла перед сохранением. По умолчанию — False.


**Returns:**
boolean — значение, указывающее, необходимо ли изменить имя файла перед сохранением. По умолчанию — False.

### setAddSuffix(boolean value) {#setAddSuffix-boolean-}
```
public final void setAddSuffix(boolean value)
```


Устанавливает значение, указывающее, необходимо ли изменить имя файла перед сохранением. По умолчанию — False.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | значение | boolean | Значение, указывающее, необходимо ли изменить имя файла перед сохранением. По умолчанию — False. |
|

### getRedactedFileSuffix() {#getRedactedFileSuffix--}
```
public final String getRedactedFileSuffix()
```


Возвращает пользовательский суффикс для имени выходного файла. Если он не указан, то
SaveSuffix
константа будет использована.


**Returns:**
java.lang.String — пользовательский суффикс для имени выходного файла. Если он не указан, то константа  SaveSuffix  будет использована.

### setRedactedFileSuffix(String value) {#setRedactedFileSuffix-java.lang.String-}
```
public final void setRedactedFileSuffix(String value)
```


Устанавливает пользовательский суффикс для имени выходного файла. Если он не указан, то
SaveSuffix
константа будет использована.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | значение | java.lang.String | Пользовательский суффикс для имени выходного файла. Если он не указан, будет использована константа  SaveSuffix  . |
|

### getRasterizeToPDF() {#getRasterizeToPDF--}
```
public final boolean getRasterizeToPDF()
```


Возвращает значение, указывающее, нужно ли конвертировать все страницы документа в изображения и поместить их в один PDF‑файл.


**Returns:**
boolean - Значение, указывающее, нужно ли конвертировать все страницы документа в изображения и поместить их в один PDF‑файл.

### setRasterizeToPDF(boolean value) {#setRasterizeToPDF-boolean-}
```
public final void setRasterizeToPDF(boolean value)
```


Устанавливает значение, указывающее, нужно ли конвертировать все страницы документа в изображения и поместить их в один PDF‑файл.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | значение | boolean | Значение, указывающее, нужно ли конвертировать все страницы документа в изображения и поместить их в один PDF‑файл. |
|

### getRasterization() {#getRasterization--}
```
public final RasterizationOptions getRasterization()
```


Возвращает настройки растеризации.


**Returns:**
[RasterizationOptions](../../com.groupdocs.redaction.options/rasterizationoptions) - The rasterization settings.

### getWordprocessingSaveOptions() {#getWordprocessingSaveOptions--}
```
public final WordprocessingSaveOptions getWordprocessingSaveOptions()
```


Параметры сохранения обработки текста.


**Returns:**
[WordprocessingSaveOptions](../../com.groupdocs.redaction.options/wordprocessingsaveoptions)
