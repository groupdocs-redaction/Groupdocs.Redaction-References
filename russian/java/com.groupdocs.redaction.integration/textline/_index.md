---
title: "TextLine"
second_title: "GroupDocs.Redaction для Java API Reference"
description: "Представляет строку текста, извлечённую OCR‑движком из изображения."
type: docs
weight: 16
url: /ru/java/com.groupdocs.redaction.integration/textline/
---
**Inheritance:**
java.lang.Object
```
public class TextLine
```

Представляет строку текста, извлечённую OCR‑движком из изображения.

*** ** * ** ***


**Learn more**

* More details about using OCR in GroupDocs.Redaction: [OCR Usage Basics](../https://docs.groupdocs.com/redaction/java/ocr-usage-basics/)

<br />


## Конструкторы

| Конструктор | Описание |
| --- | --- |
|  | [TextLine(TextFragment[] fragments)](#TextLine-com.groupdocs.redaction.integration.TextFragment---) | Инициализирует новый экземпляр строки текста, извлечённой OCR‑движком из изображения. |
|
## Методы

| Метод | Описание |
| --- | --- |
|  | [getFragments()](#getFragments--) | Получает массив текстовых фрагментов, таких как символы и слова, распознанных в строке. |
|
|  | [toString()](#toString--) | Возвращает текстовое содержание распознанной строки текста. |
|
### TextLine(TextFragment[] fragments) {#TextLine-com.groupdocs.redaction.integration.TextFragment---}
```
public TextLine(TextFragment[] fragments)
```


Инициализирует новый экземпляр строки текста, извлечённой OCR‑движком из изображения.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | fragments | [TextFragment\[\]](../../com.groupdocs.redaction.integration/textfragment) | начальный набор текстовых фрагментов |
|

### getFragments() {#getFragments--}
```
public final TextFragment[] getFragments()
```


Получает массив текстовых фрагментов, таких как символы и слова, распознанных в строке.


**Returns:**
com.groupdocs.redaction.integration.TextFragment[] - Массив текстовых фрагментов, таких как символы и слова, распознанных в строке.

### toString() {#toString--}
```
public String toString()
```


Возвращает текстовое содержание распознанной строки текста.


**Returns:**
java.lang.String - текстовое содержание распознанной строки текста

