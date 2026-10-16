---
title: "PreviewOptions"
second_title: "GroupDocs.Redaction для Java API Reference"
description: "Предоставляет параметры для установки требований и делегатов потоков для генерации предварительного просмотра."
type: docs
weight: 11
url: /ru/java/com.groupdocs.redaction.options/previewoptions/
---
**Inheritance:**
java.lang.Object
```
public class PreviewOptions
```

Предоставляет параметры для установки требований и делегатов потоков для генерации предварительного просмотра.

## Конструкторы

| Конструктор | Описание |
| --- | --- |
|  | [PreviewOptions(ICreatePageStream createPageStream)](#PreviewOptions-com.groupdocs.redaction.options.ICreatePageStream-) | Инициализирует новый экземпляр класса PreviewOptions, вызывая закрытие выходного потока. |
|
|  | [PreviewOptions(ICreatePageStream createPageStream, IReleasePageStream releasePageStream)](#PreviewOptions-com.groupdocs.redaction.options.ICreatePageStream-com.groupdocs.redaction.options.IReleasePageStream-) | Инициализирует новый экземпляр класса PreviewOptions, вызывая возврат выходного потока клиенту для дальнейшего использования. |
|
## Методы

| Метод | Описание |
| --- | --- |
|  | [getWidth()](#getWidth--) | Получает или задает ширину предварительного просмотра страницы. |
|
|  | [setWidth(int value)](#setWidth-int-) | Получает или задает ширину предварительного просмотра страницы. |
|
|  | [getHeight()](#getHeight--) | Получает или задает высоту предварительного просмотра страницы. |
|
|  | [setHeight(int value)](#setHeight-int-) | Получает или задает высоту предварительного просмотра страницы. |
|
|  | [getPageNumbers()](#getPageNumbers--) | Получает или задает массив номеров страниц для создания предварительного просмотра. |
|
|  | [setPageNumbers(int[] value)](#setPageNumbers-int---) | Получает или задает массив номеров страниц для создания предварительного просмотра. |
|
|  | [getPreviewFormat()](#getPreviewFormat--) | Получает или задает формат изображения предварительного просмотра. |
|
|  | [setPreviewFormat(PreviewFormats value)](#setPreviewFormat-com.groupdocs.redaction.options.PreviewFormats-) | Получает или задает формат изображения предварительного просмотра. |
|
|  | [getCreatePageStream()](#getCreatePageStream--) | Получает или задает экземпляр делегата создания потока страницы. |
|
|  | [setCreatePageStream(ICreatePageStream value)](#setCreatePageStream-com.groupdocs.redaction.options.ICreatePageStream-) | Получает или задает экземпляр делегата создания потока страницы. |
|
|  | [getReleasePageStream()](#getReleasePageStream--) | Получает или задает экземпляр делегата завершения предварительного просмотра страницы. |
|
|  | [setReleasePageStream(IReleasePageStream value)](#setReleasePageStream-com.groupdocs.redaction.options.IReleasePageStream-) | Получает или задает экземпляр делегата завершения предварительного просмотра страницы. |
|
### PreviewOptions(ICreatePageStream createPageStream) {#PreviewOptions-com.groupdocs.redaction.options.ICreatePageStream-}
```
public PreviewOptions(ICreatePageStream createPageStream)
```


Инициализирует новый экземпляр класса PreviewOptions, вызывая закрытие выходного потока.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | createPageStream | [ICreatePageStream](../../com.groupdocs.redaction.options/icreatepagestream) | Создает поток для конкретного предварительного просмотра страницы |
|

### PreviewOptions(ICreatePageStream createPageStream, IReleasePageStream releasePageStream) {#PreviewOptions-com.groupdocs.redaction.options.ICreatePageStream-com.groupdocs.redaction.options.IReleasePageStream-}
```
public PreviewOptions(ICreatePageStream createPageStream, IReleasePageStream releasePageStream)
```


Инициализирует новый экземпляр класса PreviewOptions, вызывая возврат выходного потока клиенту для дальнейшего использования.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | createPageStream | [ICreatePageStream](../../com.groupdocs.redaction.options/icreatepagestream) | Создает поток для конкретного предварительного просмотра страницы |
|
|  | releasePageStream | [IReleasePageStream](../../com.groupdocs.redaction.options/ireleasepagestream) | Уведомляет о завершении генерации предварительного просмотра страницы и получает выходной поток |
|

### getWidth() {#getWidth--}
```
public final int getWidth()
```


Получает или задает ширину предварительного просмотра страницы.


**Returns:**
int — Ширина предварительного просмотра страницы.

### setWidth(int value) {#setWidth-int-}
```
public final void setWidth(int value)
```


Получает или задает ширину предварительного просмотра страницы.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | значение | int | Ширина предварительного просмотра страницы. |
|

### getHeight() {#getHeight--}
```
public final int getHeight()
```


Получает или задает высоту предварительного просмотра страницы.


**Returns:**
int — Высота предварительного просмотра страницы.

### setHeight(int value) {#setHeight-int-}
```
public final void setHeight(int value)
```


Получает или задает высоту предварительного просмотра страницы.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | значение | int | Высота предварительного просмотра страницы. |
|

### getPageNumbers() {#getPageNumbers--}
```
public final int[] getPageNumbers()
```


Получает или задает массив номеров страниц для создания предварительного просмотра.


**Returns:**
int[] — Массив номеров страниц для создания предварительного просмотра.

### setPageNumbers(int[] value) {#setPageNumbers-int---}
```
public final void setPageNumbers(int[] value)
```


Получает или задает массив номеров страниц для создания предварительного просмотра.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | значение | int[] | Массив номеров страниц для создания предварительного просмотра. |
|

### getPreviewFormat() {#getPreviewFormat--}
```
public final PreviewFormats getPreviewFormat()
```


Получает или задает формат изображения предварительного просмотра.


**Returns:**
[PreviewFormats](../../com.groupdocs.redaction.options/previewformats) - Preview image format.

### setPreviewFormat(PreviewFormats value) {#setPreviewFormat-com.groupdocs.redaction.options.PreviewFormats-}
```
public final void setPreviewFormat(PreviewFormats value)
```


Получает или задает формат изображения предварительного просмотра.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | value | [PreviewFormats](../../com.groupdocs.redaction.options/previewformats) | Формат изображения предварительного просмотра. |
|

### getCreatePageStream() {#getCreatePageStream--}
```
public final ICreatePageStream getCreatePageStream()
```


Получает или задает экземпляр делегата создания потока страницы.


**Returns:**
[ICreatePageStream](../../com.groupdocs.redaction.options/icreatepagestream) - An instance of page stream creation delegate.

### setCreatePageStream(ICreatePageStream value) {#setCreatePageStream-com.groupdocs.redaction.options.ICreatePageStream-}
```
public final void setCreatePageStream(ICreatePageStream value)
```


Получает или задает экземпляр делегата создания потока страницы.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | value | [ICreatePageStream](../../com.groupdocs.redaction.options/icreatepagestream) | Экземпляр делегата создания потока страницы. |
|

### getReleasePageStream() {#getReleasePageStream--}
```
public final IReleasePageStream getReleasePageStream()
```


Получает или задает экземпляр делегата завершения предварительного просмотра страницы.


**Returns:**
[IReleasePageStream](../../com.groupdocs.redaction.options/ireleasepagestream) - An instance of page preview completion delegate.

### setReleasePageStream(IReleasePageStream value) {#setReleasePageStream-com.groupdocs.redaction.options.IReleasePageStream-}
```
public final void setReleasePageStream(IReleasePageStream value)
```


Получает или задает экземпляр делегата завершения предварительного просмотра страницы.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | value | [IReleasePageStream](../../com.groupdocs.redaction.options/ireleasepagestream) | Экземпляр делегата завершения предварительного просмотра страницы. |
|

