---
title: "RedactionResult"
second_title: "GroupDocs.Redaction для Java API Reference"
description: "Представляет результат операции редактирования."
type: docs
weight: 15
url: /ru/java/com.groupdocs.redaction/redactionresult/
---
**Inheritance:**
java.lang.Object
```
public class RedactionResult
```

Представляет результат операции редактирования.

*** ** * ** ***


**Learn more**

* More details about redaction results: [Redaction basics](../https://docs.groupdocs.com/redaction/java/redaction-basics/)

<br />


## Методы

| Метод | Описание |
| --- | --- |
|  | [getStatus()](#getStatus--) | Получает статус выполнения. |
|
|  | [getErrorMessage()](#getErrorMessage--) | Получает сообщение об ошибке для диагностики. |
|
|  | [skipped(String description)](#skipped-java.lang.String-) | Инициализирует новый экземпляр класса RedactionResult со статусом Skipped. |
|
|  | [partial(String description)](#partial-java.lang.String-) | Инициализирует новый экземпляр класса RedactionResult со статусом PartiallyApplied. |
|
|  | [failed(String description)](#failed-java.lang.String-) | Инициализирует новый экземпляр класса RedactionResult со статусом Failed. |
|
|  | [successful()](#successful--) | Инициализирует новый экземпляр класса RedactionResult со статусом Applied (успешный). |
|
### getStatus() {#getStatus--}
```
public final RedactionStatus getStatus()
```


Получает статус выполнения.


**Returns:**
[RedactionStatus](../../com.groupdocs.redaction/redactionstatus) - The execution status.

### getErrorMessage() {#getErrorMessage--}
```
public final String getErrorMessage()
```


Получает сообщение об ошибке для диагностики.


**Returns:**
java.lang.String - сообщение об ошибке для диагностики.

### skipped(String description) {#skipped-java.lang.String-}
```
public static RedactionResult skipped(String description)
```


Инициализирует новый экземпляр класса RedactionResult со статусом Skipped.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | описание | java.lang.String | Причина, по которой операция была пропущена |
|

**Returns:**
[RedactionResult](../../com.groupdocs.redaction/redactionresult) - Sskipped redaction result

### partial(String description) {#partial-java.lang.String-}
```
public static RedactionResult partial(String description)
```


Инициализирует новый экземпляр класса RedactionResult со статусом PartiallyApplied.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | описание | java.lang.String | Причина, по которой операция не была полностью применена |
|

**Returns:**
[RedactionResult](../../com.groupdocs.redaction/redactionresult) - Partially applied redaction result

### failed(String description) {#failed-java.lang.String-}
```
public static RedactionResult failed(String description)
```


Инициализирует новый экземпляр класса RedactionResult со статусом Failed.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | описание | java.lang.String | Подробности сбоя или исключения |
|

**Returns:**
[RedactionResult](../../com.groupdocs.redaction/redactionresult) - Failed redaction result

### successful() {#successful--}
```
public static RedactionResult successful()
```


Инициализирует новый экземпляр класса RedactionResult со статусом Applied (успешный).


**Returns:**
[RedactionResult](../../com.groupdocs.redaction/redactionresult) - Successful redaction result

