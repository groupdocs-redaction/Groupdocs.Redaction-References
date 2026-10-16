---
title: "PageAreaFilter"
second_title: "GroupDocs.Redaction для Java API Reference"
description: "Представляет фильтр редактирования, задающий область внутри страницы документа для применения редактирования."
type: docs
weight: 22
url: /ru/java/com.groupdocs.redaction.redactions/pageareafilter/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.redaction.redactions.RedactionFilter](../../com.groupdocs.redaction.redactions/redactionfilter)
```
public class PageAreaFilter extends RedactionFilter
```

Представляет фильтр редактирования, задающий область внутри страницы документа для применения редактирования.

*** ** * ** ***


**Learn more**

* More details about applying redactions: [Redaction basics](../https://docs.groupdocs.com/redaction/java/redaction-basics/)
* More details about redaction filters: [Use PDF redaction filters](../https://docs.groupdocs.com/redaction/java/use-pdf-redaction-filters/)

<br />


## Конструкторы

| Конструктор | Описание |
| --- | --- |
|  | [PageAreaFilter(Point topLeft, Dimension size)](#PageAreaFilter-java.awt.Point-java.awt.Dimension-) | Инициализирует новый экземпляр класса PageAreaFilter для редактирования конкретной области. |
|
## Методы

| Метод | Описание |
| --- | --- |
|  | [getRectangle()](#getRectangle--) | Получает прямоугольник (позицию верхнего левого угла и размер области) на странице. |
|
|  | [isInTheArea(Rectangle rectangle)](#isInTheArea-java.awt.Rectangle-) | Проверяет, имеет ли эта область фильтра пересечение с заданным прямоугольником. |
|
### PageAreaFilter(Point topLeft, Dimension size) {#PageAreaFilter-java.awt.Point-java.awt.Dimension-}
```
public PageAreaFilter(Point topLeft, Dimension size)
```


Инициализирует новый экземпляр класса PageAreaFilter для редактирования конкретной области.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | topLeft | java.awt.Point | Координаты области верхнего левого угла |
|
|  | size | java.awt.Dimension | Размер и цвет области |
|

### getRectangle() {#getRectangle--}
```
public final Rectangle getRectangle()
```


Получает прямоугольник (позицию верхнего левого угла и размер области) на странице.


**Returns:**
java.awt.Rectangle - Прямоугольник (позиция верхнего левого угла и размер области) на странице.

### isInTheArea(Rectangle rectangle) {#isInTheArea-java.awt.Rectangle-}
```
public final boolean isInTheArea(Rectangle rectangle)
```


Проверяет, имеет ли эта область фильтра пересечение с заданным прямоугольником.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | rectangle | java.awt.Rectangle | Прямоугольник для проверки |
|

**Returns:**
boolean - true, если эта область фильтра имеет пересечение

