---
title: "CustomRedactionResult"
second_title: "GroupDocs.Redaction для Java API Reference"
description: "Представляет результат, возвращаемый ."
type: docs
weight: 14
url: /ru/java/com.groupdocs.redaction.redactions/customredactionresult/
---
**Inheritance:**
java.lang.Object
```
public class CustomRedactionResult
```

Представляет результат, возвращаемый [ICustomRedactionHandler](../../com.groupdocs.redaction.redactions/icustomredactionhandler).

## Конструкторы

| Конструктор | Описание |
| --- | --- |
| [CustomRedactionResult()](#CustomRedactionResult--) |  |
## Методы

| Метод | Описание |
| --- | --- |
|  | [getApply()](#getApply--) | Получает значение, указывающее, следует ли применять замену. |
|
|  | [setApply(boolean value)](#setApply-boolean-) | Устанавливает значение, указывающее, следует ли применять замену. |
|
|  | [getText()](#getText--) | Получает текст замены, используемый, когда #getApply().getApply() равно |
true
.
|
|  | [setText(String value)](#setText-java.lang.String-) | Устанавливает текст замены, используемый, когда #getApply().getApply() равно |
true
.
|
### CustomRedactionResult() {#CustomRedactionResult--}
```
public CustomRedactionResult()
```


### getApply() {#getApply--}
```
public final boolean getApply()
```


Получает значение, указывающее, следует ли применять замену.


**Returns:**
boolean -  true  для замены найденного текста на #getText().getText(); иначе,  false .

### setApply(boolean value) {#setApply-boolean-}
```
public final void setApply(boolean value)
```


Устанавливает значение, указывающее, следует ли применять замену.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | значение | boolean | true  для применения замены; иначе,  false . |
|

### getText() {#getText--}
```
public final String getText()
```


Получает текст замены, используемый, когда #getApply().getApply() равно
true
.


**Returns:**
java.lang.String - Текст замены.

### setText(String value) {#setText-java.lang.String-}
```
public final void setText(String value)
```


Устанавливает текст замены, используемый, когда #getApply().getApply() равно
true
.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | значение | java.lang.String | Текст замены. |
|

