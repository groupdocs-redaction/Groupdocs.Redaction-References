---
title: "RedactorLogEntry"
second_title: "GroupDocs.Redaction для Java API Reference"
description: "Представляет результаты применения редактирования."
type: docs
weight: 18
url: /ru/java/com.groupdocs.redaction/redactorlogentry/
---
**Inheritance:**
java.lang.Object
```
public class RedactorLogEntry
```

Представляет результаты применения редактирования.

*** ** * ** ***


**Learn more**

* More details about redaction log entries: [Redaction basics](../https://docs.groupdocs.com/redaction/java/redaction-basics/)

<br />


## Конструкторы

| Конструктор | Описание |
| --- | --- |
|  | [RedactorLogEntry(Redaction redaction, RedactionResult result)](#RedactorLogEntry-com.groupdocs.redaction.Redaction-com.groupdocs.redaction.RedactionResult-) | Инициализирует новый экземпляр класса RedactorLogEntry для редактирования. |
|
## Методы

| Метод | Описание |
| --- | --- |
|  | [getResult()](#getResult--) | Получает результат, возвращаемый |
GroupDocs.Redaction.Integration.DocumentFormatInstance
.
|
|  | [getRedaction()](#getRedaction--) | Получает ссылку на редактирование и его параметры. |
|
### RedactorLogEntry(Redaction redaction, RedactionResult result) {#RedactorLogEntry-com.groupdocs.redaction.Redaction-com.groupdocs.redaction.RedactionResult-}
```
public RedactorLogEntry(Redaction redaction, RedactionResult result)
```


Инициализирует новый экземпляр класса RedactorLogEntry для редактирования.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | redaction | [Redaction](../../com.groupdocs.redaction/redaction) | Ссылка на редактирование |
|
|  | result | [RedactionResult](../../com.groupdocs.redaction/redactionresult) | Результат редактирования, сообщаемый обработчиком формата |
|

### getResult() {#getResult--}
```
public final RedactionResult getResult()
```


Получает результат, возвращаемый
GroupDocs.Redaction.Integration.DocumentFormatInstance
.


**Returns:**
[RedactionResult](../../com.groupdocs.redaction/redactionresult) - The result, returned by  GroupDocs.Redaction.Integration.DocumentFormatInstance .

### getRedaction() {#getRedaction--}
```
public final Redaction getRedaction()
```


Получает ссылку на редактирование и его параметры.


**Returns:**
[Redaction](../../com.groupdocs.redaction/redaction) - The reference to redaction and its options.

