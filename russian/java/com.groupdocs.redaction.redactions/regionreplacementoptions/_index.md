---
title: "RegionReplacementOptions"
second_title: "GroupDocs.Redaction для Java API Reference"
description: "Представляет параметры цвета и области для замены региона изображения."
type: docs
weight: 29
url: /ru/java/com.groupdocs.redaction.redactions/regionreplacementoptions/
---
**Inheritance:**
java.lang.Object
```
public class RegionReplacementOptions
```

Представляет параметры цвета и области для замены региона изображения. См.
ImageAreaRedaction
.

*** ** * ** ***


**Learn more**

* More details about image redactions: [Image redactions](../https://docs.groupdocs.com/redaction/java/image-redactions/)

<br />


## Конструкторы

| Конструктор | Описание |
| --- | --- |
|  | [RegionReplacementOptions(Color fillColor, Dimension size)](#RegionReplacementOptions-java.awt.Color-java.awt.Dimension-) | Инициализирует новый экземпляр класса RegionReplacementOptions. |
|
|  | [RegionReplacementOptions(Color fillColor, Font font, String expectedText)](#RegionReplacementOptions-java.awt.Color-java.awt.Font-java.lang.String-) | Инициализирует новый экземпляр класса RegionReplacementOptions, размер которого соответствует заданному тексту. |
|
## Методы

| Метод | Описание |
| --- | --- |
|  | [getFillColor()](#getFillColor--) | Получает цвет для заполнения отредактированной области. |
|
|  | [setFillColor(Color value)](#setFillColor-java.awt.Color-) | Устанавливает цвет для заполнения отредактированной области. |
|
|  | [getSize()](#getSize--) | Получает прямоугольник с шириной и высотой. |
|
|  | [setSize(Dimension value)](#setSize-java.awt.Dimension-) | Устанавливает прямоугольник с шириной и высотой. |
|
### RegionReplacementOptions(Color fillColor, Dimension size) {#RegionReplacementOptions-java.awt.Color-java.awt.Dimension-}
```
public RegionReplacementOptions(Color fillColor, Dimension size)
```


Инициализирует новый экземпляр класса RegionReplacementOptions.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | fillColor | java.awt.Color | Цвет для заполнения области |
|
|  | size | java.awt.Dimension | Размер заполненной области |
|

### RegionReplacementOptions(Color fillColor, Font font, String expectedText) {#RegionReplacementOptions-java.awt.Color-java.awt.Font-java.lang.String-}
```
public RegionReplacementOptions(Color fillColor, Font font, String expectedText)
```


Инициализирует новый экземпляр класса RegionReplacementOptions, размер которого соответствует заданному тексту.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | fillColor | java.awt.Color | Цвет для заполнения области |
|
|  | font | java.awt.Font | Ожидаемый шрифт текста |
|
|  | expectedText | java.lang.String | Ожидаемый текст |
|

### getFillColor() {#getFillColor--}
```
public final Color getFillColor()
```


Получает цвет для заполнения отредактированной области.


**Returns:**
java.awt.Color - Цвет для заполнения редактируемой области.

### setFillColor(Color value) {#setFillColor-java.awt.Color-}
```
public final void setFillColor(Color value)
```


Устанавливает цвет для заполнения отредактированной области.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | значение | java.awt.Color | Цвет для заполнения редактируемой области. |
|

### getSize() {#getSize--}
```
public final Dimension getSize()
```


Получает прямоугольник с шириной и высотой.


**Returns:**
java.awt.Dimension - Прямоугольник с шириной и высотой.

### setSize(Dimension value) {#setSize-java.awt.Dimension-}
```
public final void setSize(Dimension value)
```


Устанавливает прямоугольник с шириной и высотой.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | значение | java.awt.Dimension | Прямоугольник с шириной и высотой. |
|

