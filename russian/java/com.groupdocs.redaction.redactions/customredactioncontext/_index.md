---
title: "CustomRedactionContext"
second_title: "GroupDocs.Redaction для Java API Reference"
description: "Предоставляет входные данные для ."
type: docs
weight: 13
url: /ru/java/com.groupdocs.redaction.redactions/customredactioncontext/
---
**Inheritance:**
java.lang.Object
```
public class CustomRedactionContext
```

Предоставляет входные данные для [ICustomRedactionHandler](../../com.groupdocs.redaction.redactions/icustomredactionhandler).

## Конструкторы

| Конструктор | Описание |
| --- | --- |
| [CustomRedactionContext()](#CustomRedactionContext--) |  |
## Методы

| Метод | Описание |
| --- | --- |
|  | [getPageNumber()](#getPageNumber--) | Получает номер страницы совпавшего фрагмента, если доступно. |
|
|  | [setPageNumber(int value)](#setPageNumber-int-) | Устанавливает номер страницы совпавшего фрагмента. |
|
|  | [getText()](#getText--) | Получает текст, совпавший для редактирования. |
|
|  | [setText(String value)](#setText-java.lang.String-) | Устанавливает текст, совпавший для редактирования. |
|
### CustomRedactionContext() {#CustomRedactionContext--}
```
public CustomRedactionContext()
```


### getPageNumber() {#getPageNumber--}
```
public final int getPageNumber()
```


Получает номер страницы совпавшего фрагмента, если доступно.


**Returns:**
int - Номер страницы или значение, специфичное для формата, если страница неизвестна.

### setPageNumber(int value) {#setPageNumber-int-}
```
public final void setPageNumber(int value)
```


Устанавливает номер страницы совпавшего фрагмента.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | значение | int | Номер страницы. |
|

### getText() {#getText--}
```
public final String getText()
```


Получает текст, совпавший для редактирования.


**Returns:**
java.lang.String - Совпавший текст.

### setText(String value) {#setText-java.lang.String-}
```
public final void setText(String value)
```


Устанавливает текст, совпавший для редактирования.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | значение | java.lang.String | Совпавший текст. |
|

