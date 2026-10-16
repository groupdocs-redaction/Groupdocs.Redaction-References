---
title: "TextReplacement"
second_title: "GroupDocs.Redaction для Java API Reference"
description: "Представляет информацию о текстовой замене."
type: docs
weight: 33
url: /ru/java/com.groupdocs.redaction.redactions/textreplacement/
---
**Inheritance:**
java.lang.Object
```
public class TextReplacement
```

Представляет информацию о текстовой замене.

*** ** * ** ***


**Learn more**

* More details about RedactionDescription class and IRedactionCallback interface: [Use redaction callback](../https://docs.groupdocs.com/redaction/java/use-redaction-callback/)

<br />


## Конструкторы

| Конструктор | Описание |
| --- | --- |
|  | [TextReplacement(int index, String original, String replacement)](#TextReplacement-int-java.lang.String-java.lang.String-) | Инициализирует новый экземпляр класса TextReplacement. |
|
## Методы

| Метод | Описание |
| --- | --- |
|  | [getIndex()](#getIndex--) | Получает индекс найденного текста в исходной строке. |
|
|  | [getOriginalText()](#getOriginalText--) | Получает оригинальную найденную строку. |
|
|  | [getReplacement()](#getReplacement--) | Получает строку, заменяя OriginalText. |
|
|  | [toString()](#toString--) | Предоставляет описание замены текста и его позицию. |
|
### TextReplacement(int index, String original, String replacement) {#TextReplacement-int-java.lang.String-java.lang.String-}
```
public TextReplacement(int index, String original, String replacement)
```


Инициализирует новый экземпляр класса TextReplacement.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | индекс | int | Индекс найденного текста в исходной строке |
|
|  | оригинальный | java.lang.String | Исходная найденная строка |
|
|  | замена | java.lang.String | Строка, заменяющая OriginalText в исходной строке |
|

### getIndex() {#getIndex--}
```
public final int getIndex()
```


Получает индекс найденного текста в исходной строке.


**Returns:**
int - Индекс найденного текста в исходной строке.

### getOriginalText() {#getOriginalText--}
```
public final String getOriginalText()
```


Получает оригинальную найденную строку.


**Returns:**
java.lang.String - Исходная найденная строка.

### getReplacement() {#getReplacement--}
```
public final String getReplacement()
```


Получает строку, заменяя OriginalText.


**Returns:**
java.lang.String - Строка, заменяющая OriginalText.

### toString() {#toString--}
```
public String toString()
```


Предоставляет описание замены текста и его позицию.


**Returns:**
java.lang.String - Описание замены

