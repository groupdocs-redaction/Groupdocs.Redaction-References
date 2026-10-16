---
title: "Redaction"
second_title: "GroupDocs.Redaction для Java API Reference"
description: "Представляет базовый абстрактный класс для всех типов редактирования."
type: docs
weight: 13
url: /ru/java/com.groupdocs.redaction/redaction/
---
**Inheritance:**
java.lang.Object
```
public abstract class Redaction
```

Представляет базовый абстрактный класс для всех типов редактирования.

*** ** * ** ***


**Learn more**

* More details about redaction types: [Redaction basics](../https://docs.groupdocs.com/redaction/java/redaction-basics/)
* More advanced redaction topics: [Advanced usage](../https://docs.groupdocs.com/redaction/java/advanced-usage/)

<br />


## Конструкторы

| Конструктор | Описание |
| --- | --- |
| [Redaction()](#Redaction--) |  |
## Методы

| Метод | Описание |
| --- | --- |
|  | [getDescription()](#getDescription--) | Возвращает строку, описывающую редактирование и его параметры. |
|
|  | [applyTo(DocumentFormatInstance formatInstance)](#applyTo-com.groupdocs.redaction.integration.DocumentFormatInstance-) | Применяет редактирование к заданному экземпляру формата. |
|
### Redaction() {#Redaction--}
```
public Redaction()
```


### getDescription() {#getDescription--}
```
public String getDescription()
```


Возвращает строку, описывающую редактирование и его параметры.


**Returns:**
java.lang.String - Текст, содержащий название редактирования и параметры.

### applyTo(DocumentFormatInstance formatInstance) {#applyTo-com.groupdocs.redaction.integration.DocumentFormatInstance-}
```
public abstract RedactorLogEntry applyTo(DocumentFormatInstance formatInstance)
```


Применяет редактирование к заданному экземпляру формата.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | formatInstance | [DocumentFormatInstance](../../com.groupdocs.redaction.integration/documentformatinstance) | Экземпляр документа для применения редактирования |
|

**Returns:**
[RedactorLogEntry](../../com.groupdocs.redaction/redactorlogentry) - Status of the redaction: success/failure and error message if any

