---
title: "RecognizedImage"
second_title: "GroupDocs.Redaction для Java API Reference"
description: "Представляет текст, извлечённый из изображения в результате процесса распознавания."
type: docs
weight: 13
url: /ru/java/com.groupdocs.redaction.integration/recognizedimage/
---
**Inheritance:**
java.lang.Object
```
public class RecognizedImage
```

Представляет текст, извлечённый из изображения в результате процесса распознавания.

*** ** * ** ***


**Learn more**

* More details about using OCR in GroupDocs.Redaction: [OCR Usage Basics](../https://docs.groupdocs.com/redaction/java/ocr-usage-basics/)

<br />


## Конструкторы

| Конструктор | Описание |
| --- | --- |
|  | [RecognizedImage(TextLine[] lines)](#RecognizedImage-com.groupdocs.redaction.integration.TextLine---) | Инициализирует новый экземпляр класса, используя набор распознанных строк. |
|
## Методы

| Метод | Описание |
| --- | --- |
|  | [getText()](#getText--) | Получает текстовый эквивалент структурированного текста. |
|
|  | [getLines()](#getLines--) | Получает строки текста с их фрагментами, распознанные в документе. |
|
|  | [toString()](#toString--) | Получает текстовый эквивалент структурированного текста. |
|
### RecognizedImage(TextLine[] lines) {#RecognizedImage-com.groupdocs.redaction.integration.TextLine---}
```
public RecognizedImage(TextLine[] lines)
```


Инициализирует новый экземпляр класса, используя набор распознанных строк.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | lines | [TextLine\[\]](../../com.groupdocs.redaction.integration/textline) | IEnumerable (например, список или массив) распознанных строк |
|

### getText() {#getText--}
```
public final String getText()
```


Получает текстовый эквивалент структурированного текста.


**Returns:**
java.lang.String — текстовый эквивалент структурированного текста.

### getLines() {#getLines--}
```
public final TextLine[] getLines()
```


Получает строки текста с их фрагментами, распознанные в документе.


**Returns:**
com.groupdocs.redaction.integration.TextLine[] — строки текста с их фрагментами, распознанные в документе.

### toString() {#toString--}
```
public String toString()
```


Получает текстовый эквивалент структурированного текста.


**Returns:**
java.lang.String — распознанный текст

