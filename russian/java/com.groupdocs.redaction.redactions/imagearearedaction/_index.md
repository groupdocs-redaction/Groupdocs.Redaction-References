---
title: "ImageAreaRedaction"
second_title: "GroupDocs.Redaction для Java API Reference"
description: "Представляет редактирование, которое размещает цветной прямоугольник в указанной области изображения документа."
type: docs
weight: 18
url: /ru/java/com.groupdocs.redaction.redactions/imagearearedaction/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.redaction.Redaction](../../com.groupdocs.redaction/redaction)
```
public class ImageAreaRedaction extends Redaction
```

Представляет редактирование, которое размещает цветной прямоугольник в указанной области изображения документа.

*** ** * ** ***


**Learn more**

* More details about applying redactions: [Redaction basics](../https://docs.groupdocs.com/redaction/java/redaction-basics/)
* More details about image redactions: [Image redactions](../https://docs.groupdocs.com/redaction/java/image-redactions/)

<br />


## Конструкторы

| Конструктор | Описание |
| --- | --- |
|  | [ImageAreaRedaction(Point topLeft, RegionReplacementOptions options)](#ImageAreaRedaction-java.awt.Point-com.groupdocs.redaction.redactions.RegionReplacementOptions-) | Инициализирует новый экземпляр класса ImageAreaRedaction для редактирования области заданного размера. |
|
## Методы

| Метод | Описание |
| --- | --- |
|  | [getOptions()](#getOptions--) | Получает |
RegionReplacementOptions
опции с параметрами цвета и области.
|
|  | [getTopLeft()](#getTopLeft--) | Получает позицию верхнего левого угла области для удаления |
|
|  | [getDescription()](#getDescription--) | Возвращает строку, описывающую редактирование и его параметры. |
|
|  | [applyTo(DocumentFormatInstance formatInstance)](#applyTo-com.groupdocs.redaction.integration.DocumentFormatInstance-) | Применяет редактирование к заданному экземпляру формата. |
|
### ImageAreaRedaction(Point topLeft, RegionReplacementOptions options) {#ImageAreaRedaction-java.awt.Point-com.groupdocs.redaction.redactions.RegionReplacementOptions-}
```
public ImageAreaRedaction(Point topLeft, RegionReplacementOptions options)
```


Инициализирует новый экземпляр класса ImageAreaRedaction для редактирования области заданного размера.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | topLeft | java.awt.Point | Координаты области верхнего левого угла |
|
|  | options | [RegionReplacementOptions](../../com.groupdocs.redaction.redactions/regionreplacementoptions) | Размер и цвет области |
|

### getOptions() {#getOptions--}
```
public final RegionReplacementOptions getOptions()
```


Получает
RegionReplacementOptions
опции с параметрами цвета и области.


**Returns:**
[RegionReplacementOptions](../../com.groupdocs.redaction.redactions/regionreplacementoptions) - The  RegionReplacementOptions  options with color and area parameters.

### getTopLeft() {#getTopLeft--}
```
public final Point getTopLeft()
```


Получает позицию верхнего левого угла области для удаления


**Returns:**
java.awt.Point - Позиция верхнего левого угла области для удаления

### getDescription() {#getDescription--}
```
public String getDescription()
```


Возвращает строку, описывающую редактирование и его параметры.


**Returns:**
java.lang.String - Текст, содержащий название редактирования и параметры.

### applyTo(DocumentFormatInstance formatInstance) {#applyTo-com.groupdocs.redaction.integration.DocumentFormatInstance-}
```
public RedactorLogEntry applyTo(DocumentFormatInstance formatInstance)
```


Применяет редактирование к заданному экземпляру формата.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | formatInstance | [DocumentFormatInstance](../../com.groupdocs.redaction.integration/documentformatinstance) | Экземпляр документа для применения редактирования |
|

**Returns:**
[RedactorLogEntry](../../com.groupdocs.redaction/redactorlogentry) - Status of the redaction: success/failure and error message if any

