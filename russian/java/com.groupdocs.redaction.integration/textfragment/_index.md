---
title: "TextFragment"
second_title: "GroupDocs.Redaction для Java API Reference"
description: "Представляет часть распознанного текста, слова, символа и т.д., извлечённую OCR‑движком."
type: docs
weight: 15
url: /ru/java/com.groupdocs.redaction.integration/textfragment/
---
**Inheritance:**
java.lang.Object
```
public class TextFragment
```

Представляет часть распознанного текста (слово, символ и т.д.), извлечённую OCR‑движком.

*** ** * ** ***


**Learn more**

* More details about using OCR in GroupDocs.Redaction: [OCR Usage Basics](../https://docs.groupdocs.com/redaction/java/ocr-usage-basics/)

<br />


## Конструкторы

| Конструктор | Описание |
| --- | --- |
|  | [TextFragment(String text, Rectangle rectangle)](#TextFragment-java.lang.String-java.awt.Rectangle-) | Инициализирует новый экземпляр распознанного фрагмента текста. |
|
## Методы

| Метод | Описание |
| --- | --- |
|  | [getText()](#getText--) | Получает текстовое содержание распознанного фрагмента текста. |
|
|  | [getRectangle()](#getRectangle--) | Получает ограничивающий прямоугольник распознанного фрагмента текста. |
|
|  | [toString()](#toString--) | Возвращает текстовое содержание распознанного фрагмента текста. |
|
### TextFragment(String text, Rectangle rectangle) {#TextFragment-java.lang.String-java.awt.Rectangle-}
```
public TextFragment(String text, Rectangle rectangle)
```


Инициализирует новый экземпляр распознанного фрагмента текста.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | текст | java.lang.String | текстовое содержание распознанного фрагмента текста |
|
|  | rectangle | java.awt.Rectangle | ограничивающий прямоугольник распознанного фрагмента текста |
|

### getText() {#getText--}
```
public final String getText()
```


Получает текстовое содержание распознанного фрагмента текста.


**Returns:**
java.lang.String - Текстовое содержание распознанного фрагмента текста.

### getRectangle() {#getRectangle--}
```
public final Rectangle getRectangle()
```


Получает ограничивающий прямоугольник распознанного фрагмента текста.


**Returns:**
java.awt.Rectangle - Ограничивающий прямоугольник распознанного фрагмента текста.

### toString() {#toString--}
```
public String toString()
```


Возвращает текстовое содержание распознанного фрагмента текста.


**Returns:**
java.lang.String - текстовое содержание распознанного фрагмента текста

