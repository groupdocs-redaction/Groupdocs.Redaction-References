---
title: "ReplacementOptions"
second_title: "GroupDocs.Redaction для Java API Reference"
description: "Представляет параметры для замены найденного текста."
type: docs
weight: 31
url: /ru/java/com.groupdocs.redaction.redactions/replacementoptions/
---
**Inheritance:**
java.lang.Object
```
public class ReplacementOptions
```

Представляет параметры для замены найденного текста.

*** ** * ** ***


**Learn more**

* More details about document text redactions: [Text redactions](../https://docs.groupdocs.com/redaction/java/text-redactions/)
* More details about redaction filters: [Use PDF redaction filters](../https://docs.groupdocs.com/redaction/java/use-pdf-redaction-filters/)

<br />


## Конструкторы

| Конструктор | Описание |
| --- | --- |
|  | [ReplacementOptions(String replacement)](#ReplacementOptions-java.lang.String-) | Инициализирует новый экземпляр класса ReplacementOptions с текстом замены в качестве опции. |
|
|  | [ReplacementOptions(Color color)](#ReplacementOptions-java.awt.Color-) | Инициализирует новый экземпляр класса ReplacementOptions с цветным прямоугольником в качестве опции. |
|
## Методы

| Метод | Описание |
| --- | --- |
|  | [getActionType()](#getActionType--) | Получает действие замены: нарисовать рамку или заменить текст. |
|
|  | [getReplacement()](#getReplacement--) | Получает текстовое значение замены. |
|
|  | [setReplacement(String value)](#setReplacement-java.lang.String-) | Устанавливает текстовое значение замены. |
|
|  | [getBoxColor()](#getBoxColor--) | Получает цвет для |
ReplacementType.DrawBox
опция (игнорируется в остальных случаях).
|
|  | [setBoxColor(Color value)](#setBoxColor-java.awt.Color-) | Устанавливает цвет для |
ReplacementType.DrawBox
опция (игнорируется в остальных случаях).
|
|  | [getFilters()](#getFilters--) | Получает массив фильтров для применения с этой редактировкой. |
|
|  | [setFilters(RedactionFilter[] value)](#setFilters-com.groupdocs.redaction.redactions.RedactionFilter---) | Устанавливает массив фильтров для применения с этой редактировкой. |
|
|  | [getCustomRedaction()](#getCustomRedaction--) | Получает пользовательский обработчик редактирования. |
|
|  | [setCustomRedaction(ICustomRedactionHandler value)](#setCustomRedaction-com.groupdocs.redaction.redactions.ICustomRedactionHandler-) | Устанавливает пользовательский обработчик редактирования. |
|
| [fromFilters(RedactionFilter[] filters)](#fromFilters-com.groupdocs.redaction.redactions.RedactionFilter---) |  |
### ReplacementOptions(String replacement) {#ReplacementOptions-java.lang.String-}
```
public ReplacementOptions(String replacement)
```


Инициализирует новый экземпляр класса ReplacementOptions с текстом замены в качестве опции.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | замена | java.lang.String | Текстовая замена |
|

### ReplacementOptions(Color color) {#ReplacementOptions-java.awt.Color-}
```
public ReplacementOptions(Color color)
```


Инициализирует новый экземпляр класса ReplacementOptions с цветным прямоугольником в качестве опции.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | цвет | java.awt.Color | Цвет прямоугольника |
|

### getActionType() {#getActionType--}
```
public final ReplacementType getActionType()
```


Получает действие замены: нарисовать рамку или заменить текст.


**Returns:**
[ReplacementType](../../com.groupdocs.redaction.redactions/replacementtype) - The replacement action: draw box or replace text.

### getReplacement() {#getReplacement--}
```
public final String getReplacement()
```


Получает текстовое значение замены.


**Returns:**
java.lang.String - Текстовое значение замены.

### setReplacement(String value) {#setReplacement-java.lang.String-}
```
public final void setReplacement(String value)
```


Устанавливает текстовое значение замены.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | значение | java.lang.String | Текстовое значение замены. |
|

### getBoxColor() {#getBoxColor--}
```
public final Color getBoxColor()
```


Получает цвет для
ReplacementType.DrawBox
опция (игнорируется в остальных случаях).


**Returns:**
java.awt.Color - Цвет для опции  ReplacementType.DrawBox  (игнорируется в остальных случаях).

### setBoxColor(Color value) {#setBoxColor-java.awt.Color-}
```
public final void setBoxColor(Color value)
```


Устанавливает цвет для
ReplacementType.DrawBox
опция (игнорируется в остальных случаях).


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | значение | java.awt.Color | Цвет для опции  ReplacementType.DrawBox  (игнорируется в остальных случаях). |
|

### getFilters() {#getFilters--}
```
public final RedactionFilter[] getFilters()
```


Получает массив фильтров для применения с этой редактировкой.


**Returns:**
com.groupdocs.redaction.redactions.RedactionFilter[] - Массив фильтров для применения с этой редактировкой.

### setFilters(RedactionFilter[] value) {#setFilters-com.groupdocs.redaction.redactions.RedactionFilter---}
```
public final void setFilters(RedactionFilter[] value)
```


Устанавливает массив фильтров для применения с этой редактировкой.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | value | [RedactionFilter\[\]](../../com.groupdocs.redaction.redactions/redactionfilter) | Массив фильтров для применения с этой редактировкой. |
|

### getCustomRedaction() {#getCustomRedaction--}
```
public final ICustomRedactionHandler getCustomRedaction()
```


Получает пользовательский обработчик редактирования. Поддерживается только для PDF [PageAreaRedaction](../../com.groupdocs.redaction.redactions/pagearearedaction).


**Returns:**
[ICustomRedactionHandler](../../com.groupdocs.redaction.redactions/icustomredactionhandler) - An instance of [ICustomRedactionHandler](../../com.groupdocs.redaction.redactions/icustomredactionhandler), or  null  if not set.

### setCustomRedaction(ICustomRedactionHandler value) {#setCustomRedaction-com.groupdocs.redaction.redactions.ICustomRedactionHandler-}
```
public final void setCustomRedaction(ICustomRedactionHandler value)
```


Устанавливает пользовательский обработчик редактирования. Поддерживается только для PDF [PageAreaRedaction](../../com.groupdocs.redaction.redactions/pagearearedaction).


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | value | [ICustomRedactionHandler](../../com.groupdocs.redaction.redactions/icustomredactionhandler) | Экземпляр [ICustomRedactionHandler](../../com.groupdocs.redaction.redactions/icustomredactionhandler). |
|

### fromFilters(RedactionFilter[] filters) {#fromFilters-com.groupdocs.redaction.redactions.RedactionFilter---}
```
public static ReplacementOptions fromFilters(RedactionFilter[] filters)
```




**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| filters | [RedactionFilter\[\]](../../com.groupdocs.redaction.redactions/redactionfilter) |  |

**Returns:**
[ReplacementOptions](../../com.groupdocs.redaction.redactions/replacementoptions)
