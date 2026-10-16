---
title: "TextRedaction"
second_title: "GroupDocs.Redaction для Java API Reference"
description: "Представляет базовый абстрактный класс для текстовых редактирований документа."
type: docs
weight: 32
url: /ru/java/com.groupdocs.redaction.redactions/textredaction/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.redaction.Redaction](../../com.groupdocs.redaction/redaction)
```
public abstract class TextRedaction extends Redaction
```

Представляет базовый абстрактный класс для текстовых редактирований документа.

*** ** * ** ***


**Learn more**

* More details about applying redactions: [Redaction basics](../https://docs.groupdocs.com/redaction/java/redaction-basics/)
* More details about document text redactions: [Text redactions](../https://docs.groupdocs.com/redaction/java/text-redactions/)

<br />


## Методы

| Метод | Описание |
| --- | --- |
|  | [getActionOptions()](#getActionOptions--) | Получает |
ReplacementOptions
экземпляр, указывающий тип замены текста.
|
|  | [getOcrConnector()](#getOcrConnector--) | Получает |
IOcrConnector
реализация, необходимая для извлечения текста из графического содержимого.
|
|  | [setOcrConnector(IOcrConnector value)](#setOcrConnector-com.groupdocs.redaction.integration.IOcrConnector-) | Устанавливает |
IOcrConnector
реализация, необходимая для извлечения текста из графического содержимого.
|
### getActionOptions() {#getActionOptions--}
```
public final ReplacementOptions getActionOptions()
```


Получает
ReplacementOptions
экземпляр, указывающий тип замены текста.


**Returns:**
[ReplacementOptions](../../com.groupdocs.redaction.redactions/replacementoptions) - The  ReplacementOptions  instance, specifying type of text replacement.

### getOcrConnector() {#getOcrConnector--}
```
public final IOcrConnector getOcrConnector()
```


Получает
IOcrConnector
реализация, необходимая для извлечения текста из графического содержимого.


**Returns:**
[IOcrConnector](../../com.groupdocs.redaction.integration/iocrconnector) - The  IOcrConnector  implementation, required to extract text from graphic content.

### setOcrConnector(IOcrConnector value) {#setOcrConnector-com.groupdocs.redaction.integration.IOcrConnector-}
```
public final void setOcrConnector(IOcrConnector value)
```


Устанавливает
IOcrConnector
реализация, необходимая для извлечения текста из графического содержимого.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | value | [IOcrConnector](../../com.groupdocs.redaction.integration/iocrconnector) | Реализация IOcrConnector, необходимая для извлечения текста из графического содержимого. |
|

