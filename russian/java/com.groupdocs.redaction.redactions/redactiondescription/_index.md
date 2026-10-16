---
title: "RedactionDescription"
second_title: "GroupDocs.Redaction для Java API Reference"
description: "Представляет информацию о единственном действии изменения, выполненном в процессе редактирования."
type: docs
weight: 25
url: /ru/java/com.groupdocs.redaction.redactions/redactiondescription/
---
**Inheritance:**
java.lang.Object
```
public class RedactionDescription
```

Представляет информацию о единственном действии изменения, выполненном в процессе редактирования.

*** ** * ** ***


**Learn more**

* More details about RedactionDescription class and IRedactionCallback interface: [Use redaction callback](../https://docs.groupdocs.com/redaction/java/use-redaction-callback/)

<br />


## Конструкторы

| Конструктор | Описание |
| --- | --- |
|  | [RedactionDescription(int redactionType, RedactionActionType actionType, String originalText)](#RedactionDescription-int-com.groupdocs.redaction.redactions.RedactionActionType-java.lang.String-) | Инициализирует новый экземпляр класса RedactionDescription без информации о замене. |
|
|  | [RedactionDescription(int redactionType, RedactionActionType actionType, String originalText, TextReplacement replacement)](#RedactionDescription-int-com.groupdocs.redaction.redactions.RedactionActionType-java.lang.String-com.groupdocs.redaction.redactions.TextReplacement-) | Инициализирует новый экземпляр класса RedactionDescription с информацией о замене. |
|
|  | [RedactionDescription(int redactionType, RedactionActionType actionType, RegionReplacementOptions imageAreaReplacement, String imageDetails)](#RedactionDescription-int-com.groupdocs.redaction.redactions.RedactionActionType-com.groupdocs.redaction.redactions.RegionReplacementOptions-java.lang.String-) | Инициализирует новый экземпляр класса RedactionDescription с информацией о замене области изображения. |
|
## Методы

| Метод | Описание |
| --- | --- |
|  | [getRedactionType()](#getRedactionType--) | Получает тип данных документа — текст, метаданные или аннотации. |
|
|  | [getActionType()](#getActionType--) | Получает операцию редактирования: замена, очистка или удаление. |
|
|  | [getOriginalText()](#getOriginalText--) | Получает совпавший текст, если предоставлено какое‑либо выражение. |
|
|  | [getReplacement()](#getReplacement--) | Получает информацию о замене, может быть null. |
|
|  | [getImageAreaReplacement()](#getImageAreaReplacement--) | Получает информацию о замене для редактирования областей изображения, возвращает null для текстовых редактирований. |
|
|  | [getDetails()](#getDetails--) | Получает необязательную детальную информацию о редактируемом элементе. |
|
|  | [setDetails(String value)](#setDetails-java.lang.String-) | Устанавливает необязательную детальную информацию о редактируемом элементе. |
|
### RedactionDescription(int redactionType, RedactionActionType actionType, String originalText) {#RedactionDescription-int-com.groupdocs.redaction.redactions.RedactionActionType-java.lang.String-}
```
public RedactionDescription(int redactionType, RedactionActionType actionType, String originalText)
```


Инициализирует новый экземпляр класса RedactionDescription без информации о замене.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | redactionType | int | Тип данных, подлежащих редактированию |
|
|  | actionType | [RedactionActionType](../../com.groupdocs.redaction.redactions/redactionactiontype) | Действие, которое будет выполнено над этими данными |
|
|  | originalText | java.lang.String | Совпавший текст, комментарий или тело аннотации |
|

### RedactionDescription(int redactionType, RedactionActionType actionType, String originalText, TextReplacement replacement) {#RedactionDescription-int-com.groupdocs.redaction.redactions.RedactionActionType-java.lang.String-com.groupdocs.redaction.redactions.TextReplacement-}
```
public RedactionDescription(int redactionType, RedactionActionType actionType, String originalText, TextReplacement replacement)
```


Инициализирует новый экземпляр класса RedactionDescription с информацией о замене.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | redactionType | int | Тип данных, подлежащих редактированию |
|
|  | actionType | [RedactionActionType](../../com.groupdocs.redaction.redactions/redactionactiontype) | Действие, которое будет выполнено над этими данными |
|
|  | originalText | java.lang.String | Совпавший текст, комментарий или тело аннотации |
|
|  | replacement | [TextReplacement](../../com.groupdocs.redaction.redactions/textreplacement) | Текст замены, совпавший текст и его позиция в оригинальной строке |
|

### RedactionDescription(int redactionType, RedactionActionType actionType, RegionReplacementOptions imageAreaReplacement, String imageDetails) {#RedactionDescription-int-com.groupdocs.redaction.redactions.RedactionActionType-com.groupdocs.redaction.redactions.RegionReplacementOptions-java.lang.String-}
```
public RedactionDescription(int redactionType, RedactionActionType actionType, RegionReplacementOptions imageAreaReplacement, String imageDetails)
```


Инициализирует новый экземпляр класса RedactionDescription с информацией о замене области изображения.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | redactionType | int | Тип данных, подлежащих редактированию |
|
|  | actionType | [RedactionActionType](../../com.groupdocs.redaction.redactions/redactionactiontype) | Действие, которое будет выполнено над этими данными |
|
|  | imageAreaReplacement | [RegionReplacementOptions](../../com.groupdocs.redaction.redactions/regionreplacementoptions) | Информация о замене области изображения |
|
|  | imageDetails | java.lang.String | Текстовое описание изображения, по умолчанию это String.Empty |
|

### getRedactionType() {#getRedactionType--}
```
public final int getRedactionType()
```


Получает тип данных документа — текст, метаданные или аннотации.


**Returns:**
int — Тип данных документа — текст, метаданные или аннотации.

### getActionType() {#getActionType--}
```
public final RedactionActionType getActionType()
```


Получает операцию редактирования: замена, очистка или удаление.


**Returns:**
[RedactionActionType](../../com.groupdocs.redaction.redactions/redactionactiontype) - The redaction operation: replacement, cleanup or deletion.

### getOriginalText() {#getOriginalText--}
```
public final String getOriginalText()
```


Получает совпавший текст, если предоставлено какое‑либо выражение.


**Returns:**
java.lang.String — Совпавший текст, если предоставлено какое‑либо выражение.

### getReplacement() {#getReplacement--}
```
public final TextReplacement getReplacement()
```


Получает информацию о замене, может быть null.


**Returns:**
[TextReplacement](../../com.groupdocs.redaction.redactions/textreplacement) - The replacement information, can be null.

### getImageAreaReplacement() {#getImageAreaReplacement--}
```
public final RegionReplacementOptions getImageAreaReplacement()
```


Получает информацию о замене для редактирования областей изображения, возвращает null для текстовых редактирований.


**Returns:**
[RegionReplacementOptions](../../com.groupdocs.redaction.redactions/regionreplacementoptions) - The replacement information for image area redactions, returns null for textual redactions.

### getDetails() {#getDetails--}
```
public final String getDetails()
```


Получает необязательную детальную информацию о редактируемом элементе.


**Returns:**
java.lang.String — Необязательная детальная информация о редактируемом элементе.

### setDetails(String value) {#setDetails-java.lang.String-}
```
public final void setDetails(String value)
```


Устанавливает необязательную детальную информацию о редактируемом элементе.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | значение | java.lang.String | Необязательная детальная информация о редактируемом элементе. |
|

