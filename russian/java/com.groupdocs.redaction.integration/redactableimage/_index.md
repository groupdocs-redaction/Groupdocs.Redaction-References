---
title: "RedactableImage"
second_title: "GroupDocs.Redaction для Java API Reference"
description: "Предоставляет фасад для всех операций редактирования растровых изображений."
type: docs
weight: 14
url: /ru/java/com.groupdocs.redaction.integration/redactableimage/
---
**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.groupdocs.redaction.integration.IImageFormatInstance](../../com.groupdocs.redaction.integration/iimageformatinstance), [com.groupdocs.redaction.integration.IMultipleAreaRedactable](../../com.groupdocs.redaction.integration/imultiplearearedactable)
```
public class RedactableImage implements IImageFormatInstance, IMultipleAreaRedactable
```

Предоставляет фасад для всех операций редактирования растровых изображений.

## Конструкторы

| Конструктор | Описание |
| --- | --- |
|  | [RedactableImage(IImageFormatInstance img)](#RedactableImage-com.groupdocs.redaction.integration.IImageFormatInstance-) | Создаёт новый экземпляр, используя объект, реализующий |
IImageFormatInstance
интерфейс.
|
|  | [RedactableImage(IMultipleAreaRedactable img)](#RedactableImage-com.groupdocs.redaction.integration.IMultipleAreaRedactable-) | Создаёт новый экземпляр, используя объект, реализующий |
IMultipleAreaRedactable
интерфейс.
|
## Методы

| Метод | Описание |
| --- | --- |
|  | [getRawStream()](#getRawStream--) | Получает поток с реальным содержимым изображения. |
|
|  | [editAreas(Rectangle[] rectangles, Color boxColor)](#editAreas-java.awt.Rectangle---java.awt.Color-) | Редактирует несколько областей изображения одновременно одним и тем же цветом. |
|
|  | [editArea(Point topLeft, RegionReplacementOptions options)](#editArea-java.awt.Point-com.groupdocs.redaction.redactions.RegionReplacementOptions-) | Заменяет область в заданной точке прямоугольником определённого цвета и размера. |
|
### RedactableImage(IImageFormatInstance img) {#RedactableImage-com.groupdocs.redaction.integration.IImageFormatInstance-}
```
public RedactableImage(IImageFormatInstance img)
```


Создаёт новый экземпляр, используя объект, реализующий
IImageFormatInstance
интерфейс.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | img | [IImageFormatInstance](../../com.groupdocs.redaction.integration/iimageformatinstance) | Экземпляр, реализующий интерфейс IImageFormatInstance |
|

### RedactableImage(IMultipleAreaRedactable img) {#RedactableImage-com.groupdocs.redaction.integration.IMultipleAreaRedactable-}
```
public RedactableImage(IMultipleAreaRedactable img)
```


Создаёт новый экземпляр, используя объект, реализующий
IMultipleAreaRedactable
интерфейс.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | img | [IMultipleAreaRedactable](../../com.groupdocs.redaction.integration/imultiplearearedactable) | Экземпляр, реализующий интерфейс IMultipleAreaRedactable |
|

### getRawStream() {#getRawStream--}
```
public final InputStream getRawStream()
```


Получает поток с реальным содержимым изображения.


**Returns:**
java.io.InputStream — поток, содержащий данные изображения

### editAreas(Rectangle[] rectangles, Color boxColor) {#editAreas-java.awt.Rectangle---java.awt.Color-}
```
public final RedactionResult editAreas(Rectangle[] rectangles, Color boxColor)
```


Редактирует несколько областей изображения одновременно одним и тем же цветом.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | прямоугольники | java.awt.Rectangle[] | Массив областей прямоугольников |
|
|  | boxColor | java.awt.Color | Цвет для заполнения областей |
|

**Returns:**
[RedactionResult](../../com.groupdocs.redaction/redactionresult) - Image areas redaction result

### editArea(Point topLeft, RegionReplacementOptions options) {#editArea-java.awt.Point-com.groupdocs.redaction.redactions.RegionReplacementOptions-}
```
public final RedactionResult editArea(Point topLeft, RegionReplacementOptions options)
```


Заменяет область в заданной точке прямоугольником определённого цвета и размера.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | topLeft | java.awt.Point | Координаты левого верхнего угла заполненной области |
|
|  | options | [RegionReplacementOptions](../../com.groupdocs.redaction.redactions/regionreplacementoptions) | Настройки цвета и размера |
|

**Returns:**
[RedactionResult](../../com.groupdocs.redaction/redactionresult) - Image area redaction result

