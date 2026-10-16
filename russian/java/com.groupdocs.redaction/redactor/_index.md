---
title: "Redactor"
second_title: "GroupDocs.Redaction для Java API Reference"
description: "Представляет основной класс, который управляет процессом редактирования документов, позволяя открывать, редактировать и сохранять документы."
type: docs
weight: 16
url: /ru/java/com.groupdocs.redaction/redactor/
---
**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
java.io.Closeable, [com.groupdocs.redaction.integration.IPreviewable](../../com.groupdocs.redaction.integration/ipreviewable)
```
public final class Redactor implements Closeable, IPreviewable
```

Представляет основной класс, который контролирует процесс редактирования документа, позволяя открывать, редактировать и сохранять документы.

*** ** * ** ***


**Learn more**

* More details about applying redactions: [Redaction basics](../https://docs.groupdocs.com/redaction/java/redaction-basics/)
* More advanced redaction topics: [Advanced usage](../https://docs.groupdocs.com/redaction/java/advanced-usage/)

<br />


## Конструкторы

| Конструктор | Описание |
| --- | --- |
|  | [Redactor(String filePath)](#Redactor-java.lang.String-) | Инициализирует новый экземпляр |
Redactor
класс, использующий путь к файлу.
|
|  | [Redactor(InputStream document)](#Redactor-java.io.InputStream-) | Инициализирует новый экземпляр |
Redactor
класс, использующий поток.
|
|  | [Redactor(String filePath, LoadOptions loadOptions)](#Redactor-java.lang.String-com.groupdocs.redaction.options.LoadOptions-) | Инициализирует новый экземпляр |
Redactor
класс для защищённого паролем документа, использующего его путь.
|
|  | [Redactor(String filePath, LoadOptions loadOptions, RedactorSettings settings)](#Redactor-java.lang.String-com.groupdocs.redaction.options.LoadOptions-com.groupdocs.redaction.options.RedactorSettings-) | Инициализирует новый экземпляр |
Redactor
класс для защищённого паролем документа, использующего его путь и настройки.
|
|  | [Redactor(InputStream document, LoadOptions loadOptions)](#Redactor-java.io.InputStream-com.groupdocs.redaction.options.LoadOptions-) | Инициализирует новый экземпляр |
Redactor
класс для защищённого паролем документа, использующего поток.
|
|  | [Redactor(InputStream document, LoadOptions loadOptions, RedactorSettings settings)](#Redactor-java.io.InputStream-com.groupdocs.redaction.options.LoadOptions-com.groupdocs.redaction.options.RedactorSettings-) | Инициализирует новый экземпляр |
Redactor
класс для защищённого паролем документа, использующего поток и настройки.
|
## Методы

| Метод | Описание |
| --- | --- |
|  | [close()](#close--) | Освобождает ресурсы. |
|
|  | [apply(Redaction redaction)](#apply-com.groupdocs.redaction.Redaction-) | Применяет редактирование к документу. |
|
|  | [apply(Redaction[] redactions)](#apply-com.groupdocs.redaction.Redaction---) | Применяет набор редактирований к документу. |
|
|  | [apply(RedactionPolicy policy)](#apply-com.groupdocs.redaction.RedactionPolicy-) | Применяет политику редактирования к документу. |
|
|  | [save()](#save--) | Сохраняет документ в файл со следующими параметрами: AddSuffix = true, RasterizeToPDF = true. |
|
|  | [save(SaveOptions saveOptions)](#save-com.groupdocs.redaction.options.SaveOptions-) | Сохраняет документ в файл. |
|
|  | [save(OutputStream document)](#save-java.io.OutputStream-) | Сохраняет документ в поток. |
|
|  | [save(OutputStream document, SaveOptions saveOptions)](#save-java.io.OutputStream-com.groupdocs.redaction.options.SaveOptions-) | Сохраняет документ в поток. |
|
|  | [save(OutputStream document, RasterizationOptions rasterizationOptions)](#save-java.io.OutputStream-com.groupdocs.redaction.options.RasterizationOptions-) | Сохраняет документ в поток, включая пользовательское расположение. |
|
|  | [generatePreview(PreviewOptions previewOptions)](#generatePreview-com.groupdocs.redaction.options.PreviewOptions-) | Создаёт изображения предварительного просмотра конкретных страниц в заданном формате изображения. |
|
|  | [getDocumentInfo()](#getDocumentInfo--) | Получает общую информацию о документе — размер, количество страниц и т.д. |
|
### Redactor(String filePath) {#Redactor-java.lang.String-}
```
public Redactor(String filePath)
```


Инициализирует новый экземпляр
Redactor
класс, использующий путь к файлу.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | filePath | java.lang.String | Путь к файлу |


Следующий пример демонстрирует, как открыть документ для редактирования.

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
// Здесь мы можем использовать экземпляр document для выполнения редактирования
}
}
 
``` 
````

|

### Redactor(String filePath, LoadOptions loadOptions) {#Redactor-java.lang.String-com.groupdocs.redaction.options.LoadOptions-}
```
public Redactor(String filePath, LoadOptions loadOptions)
```


Инициализирует новый экземпляр
Redactor
класс для защищённого паролем документа, использующего его путь.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | filePath | java.lang.String | Путь к файлу. |
|
|  | loadOptions | [LoadOptions](../../com.groupdocs.redaction.options/loadoptions) | Параметры, включая пароль. |
|

### Redactor(String filePath, LoadOptions loadOptions, RedactorSettings settings) {#Redactor-java.lang.String-com.groupdocs.redaction.options.LoadOptions-com.groupdocs.redaction.options.RedactorSettings-}
```
public Redactor(String filePath, LoadOptions loadOptions, RedactorSettings settings)
```


Инициализирует новый экземпляр
Redactor
класс для защищённого паролем документа, использующего его путь и настройки.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | filePath | java.lang.String | Путь к файлу. |
|
|  | loadOptions | [LoadOptions](../../com.groupdocs.redaction.options/loadoptions) | Зависящие от файла параметры, включая пароль. |
|
|  | settings | [RedactorSettings](../../com.groupdocs.redaction.options/redactorsettings) | Настройки по умолчанию для процесса редактирования. |
|

### Redactor(InputStream document, LoadOptions loadOptions) {#Redactor-java.io.InputStream-com.groupdocs.redaction.options.LoadOptions-}
```
public Redactor(InputStream document, LoadOptions loadOptions)
```


Инициализирует новый экземпляр
Redactor
класс для защищённого паролем документа, использующего поток.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | document | java.io.InputStream | Исходный входной поток. |
|
|  | loadOptions | [LoadOptions](../../com.groupdocs.redaction.options/loadoptions) | Параметры, включая пароль. |
|

### Redactor(InputStream document, LoadOptions loadOptions, RedactorSettings settings) {#Redactor-java.io.InputStream-com.groupdocs.redaction.options.LoadOptions-com.groupdocs.redaction.options.RedactorSettings-}
```
public Redactor(InputStream document, LoadOptions loadOptions, RedactorSettings settings)
```


Инициализирует новый экземпляр
Redactor
класс для защищённого паролем документа, использующего поток и настройки.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | document | java.io.InputStream | Исходный входной поток. |
|
|  | loadOptions | [LoadOptions](../../com.groupdocs.redaction.options/loadoptions) | Параметры, включая пароль. |
|
|  | settings | [RedactorSettings](../../com.groupdocs.redaction.options/redactorsettings) | Настройки по умолчанию для процесса редактирования. |
|

### close() {#close--}
```
public final void close()
```


Освобождает ресурсы.


### apply(Redaction redaction) {#apply-com.groupdocs.redaction.Redaction-}
```
public final RedactorChangeLog apply(Redaction redaction)
```


Применяет редактирование к документу.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | redaction | [Redaction](../../com.groupdocs.redaction/redaction) | Экземпляр  Redaction  для применения |
|

**Returns:**
[RedactorChangeLog](../../com.groupdocs.redaction/redactorchangelog) - Success or failure and error message in this case

### apply(Redaction[] redactions) {#apply-com.groupdocs.redaction.Redaction---}
```
public final RedactorChangeLog apply(Redaction[] redactions)
```


Применяет набор редактирований к документу.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | redactions | [Redaction\[\]](../../com.groupdocs.redaction/redaction) | Массив редактирований для применения |
|

**Returns:**
[RedactorChangeLog](../../com.groupdocs.redaction/redactorchangelog) - Success or failure and error message in this case

### apply(RedactionPolicy policy) {#apply-com.groupdocs.redaction.RedactionPolicy-}
```
public final RedactorChangeLog apply(RedactionPolicy policy)
```


Применяет политику редактирования к документу.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | policy | [RedactionPolicy](../../com.groupdocs.redaction/redactionpolicy) | Политика редактирования |
|

**Returns:**
[RedactorChangeLog](../../com.groupdocs.redaction/redactorchangelog) - Success or failure and error message in this case

### save() {#save--}
```
public final String save()
```


Сохраняет документ в файл со следующими параметрами: AddSuffix = true, RasterizeToPDF = true.


**Returns:**
java.lang.String - Путь к отредактированному документу

### save(SaveOptions saveOptions) {#save-com.groupdocs.redaction.options.SaveOptions-}
```
public final String save(SaveOptions saveOptions)
```


Сохраняет документ в файл.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | saveOptions | [SaveOptions](../../com.groupdocs.redaction.options/saveoptions) | Параметры для добавления суффикса или растеризации |
|

**Returns:**
java.lang.String - Путь к отредактированному документу

### save(OutputStream document) {#save-java.io.OutputStream-}
```
public final void save(OutputStream document)
```


Сохраняет документ в поток.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | document | java.io.OutputStream | Целевой поток |
|

### save(OutputStream document, SaveOptions saveOptions) {#save-java.io.OutputStream-com.groupdocs.redaction.options.SaveOptions-}
```
public final void save(OutputStream document, SaveOptions saveOptions)
```


Сохраняет документ в поток.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | document | java.io.OutputStream | Целевой поток |
|
|  | saveOptions | [SaveOptions](../../com.groupdocs.redaction.options/saveoptions) | Параметры сохранения |
|

### save(OutputStream document, RasterizationOptions rasterizationOptions) {#save-java.io.OutputStream-com.groupdocs.redaction.options.RasterizationOptions-}
```
public final void save(OutputStream document, RasterizationOptions rasterizationOptions)
```


Сохраняет документ в поток, включая пользовательское расположение.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | document | java.io.OutputStream | Целевой поток |
|
|  | rasterizationOptions | [RasterizationOptions](../../com.groupdocs.redaction.options/rasterizationoptions) | Параметры для растеризации или её отключения и указания страниц для растеризации |
|

### generatePreview(PreviewOptions previewOptions) {#generatePreview-com.groupdocs.redaction.options.PreviewOptions-}
```
public final void generatePreview(PreviewOptions previewOptions)
```


Создаёт изображения предварительного просмотра конкретных страниц в заданном формате изображения.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | previewOptions | [PreviewOptions](../../com.groupdocs.redaction.options/previewoptions) | Свойства изображения и настройки диапазона страниц |
|

### getDocumentInfo() {#getDocumentInfo--}
```
public final IDocumentInfo getDocumentInfo()
```


Получает общую информацию о документе — размер, количество страниц и т.д.


**Returns:**
[IDocumentInfo](../../com.groupdocs.redaction/idocumentinfo) - An instance of IDocumentInfo

