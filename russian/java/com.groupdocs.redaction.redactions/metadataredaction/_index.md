---
title: "MetadataRedaction"
second_title: "GroupDocs.Redaction для Java API Reference"
description: "Представляет базовый абстрактный класс для редактирования метаданных документа."
type: docs
weight: 20
url: /ru/java/com.groupdocs.redaction.redactions/metadataredaction/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.redaction.Redaction](../../com.groupdocs.redaction/redaction)
```
public abstract class MetadataRedaction extends Redaction
```

Представляет базовый абстрактный класс для редактирования метаданных документа.

*** ** * ** ***


**Learn more**

* More details about document metadata redactions: [Metadata redactions](../https://docs.groupdocs.com/redaction/java/metadata-redactions/)

<br />


## Методы

| Метод | Описание |
| --- | --- |
|  | [getFilter()](#getFilter--) | Получает фильтр, который используется для выбора всех или конкретных метаданных, например Author или Company. |
|
|  | [setFilter(int value)](#setFilter-int-) | Устанавливает фильтр, который используется для выбора всех или конкретных метаданных, например Author или Company. |
|
|  | [applyTo(DocumentFormatInstance formatInstance)](#applyTo-com.groupdocs.redaction.integration.DocumentFormatInstance-) | Применяет редактирование к заданному экземпляру формата. |
|
### getFilter() {#getFilter--}
```
public final int getFilter()
```


Получает фильтр, который используется для выбора всех или конкретных метаданных, например Author или Company.


**Returns:**
int - Фильтр, который используется для выбора всех или конкретных метаданных, например Author или Company.

### setFilter(int value) {#setFilter-int-}
```
public final void setFilter(int value)
```


Устанавливает фильтр, который используется для выбора всех или конкретных метаданных, например Author или Company.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | значение | int | Фильтр, который используется для выбора всех или конкретных метаданных, например Author или Company. |
|

### applyTo(DocumentFormatInstance formatInstance) {#applyTo-com.groupdocs.redaction.integration.DocumentFormatInstance-}
```
public RedactorLogEntry applyTo(DocumentFormatInstance formatInstance)
```


Применяет редактирование к заданному экземпляру формата.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | formatInstance | [DocumentFormatInstance](../../com.groupdocs.redaction.integration/documentformatinstance) | Экземпляр документа для применения редактирования |
|

**Returns:**
[RedactorLogEntry](../../com.groupdocs.redaction/redactorlogentry) - Status of the redaction: success/failure and error message if any

