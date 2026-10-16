---
title: "RegexRedaction"
second_title: "GroupDocs.Redaction для Java API Reference"
description: "Представляет текстовое редактирование, которое ищет и заменяет текст в документе, сопоставляя предоставленное регулярное выражение."
type: docs
weight: 28
url: /ru/java/com.groupdocs.redaction.redactions/regexredaction/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.redaction.Redaction](../../com.groupdocs.redaction/redaction), [com.groupdocs.redaction.redactions.TextRedaction](../../com.groupdocs.redaction.redactions/textredaction)
```
public class RegexRedaction extends TextRedaction
```

Представляет текстовое редактирование, которое ищет и заменяет текст в документе, сопоставляя предоставленное регулярное выражение.

*** ** * ** ***


**Learn more**

* More details about applying redactions: [Redaction basics](../https://docs.groupdocs.com/redaction/java/redaction-basics/)
* More details about document text redactions: [Text redactions](../https://docs.groupdocs.com/redaction/java/text-redactions/)

<br />


## Конструкторы

| Конструктор | Описание |
| --- | --- |
|  | [RegexRedaction(String pattern, ReplacementOptions options)](#RegexRedaction-java.lang.String-com.groupdocs.redaction.redactions.ReplacementOptions-) | Инициализирует новый экземпляр класса RegexRedaction. |
|
|  | [RegexRedaction(Pattern regex, ReplacementOptions options)](#RegexRedaction-java.util.regex.Pattern-com.groupdocs.redaction.redactions.ReplacementOptions-) | Инициализирует новый экземпляр класса RegexRedaction. |
|
## Методы

| Метод | Описание |
| --- | --- |
|  | [getRegularExpression()](#getRegularExpression--) | Получает регулярное выражение для сопоставления. |
|
|  | [getDescription()](#getDescription--) | Возвращает строку, описывающую редактирование и его параметры. |
|
|  | [applyTo(DocumentFormatInstance formatInstance)](#applyTo-com.groupdocs.redaction.integration.DocumentFormatInstance-) | Применяет редактирование к заданному экземпляру формата. |
|
### RegexRedaction(String pattern, ReplacementOptions options) {#RegexRedaction-java.lang.String-com.groupdocs.redaction.redactions.ReplacementOptions-}
```
public RegexRedaction(String pattern, ReplacementOptions options)
```


Инициализирует новый экземпляр класса RegexRedaction.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | шаблон | java.lang.String | Регулярное выражение для поиска и замены |
|
|  | options | [ReplacementOptions](../../com.groupdocs.redaction.redactions/replacementoptions) | Параметры замены (текстовые, цветовые) |
|

### RegexRedaction(Pattern regex, ReplacementOptions options) {#RegexRedaction-java.util.regex.Pattern-com.groupdocs.redaction.redactions.ReplacementOptions-}
```
public RegexRedaction(Pattern regex, ReplacementOptions options)
```


Инициализирует новый экземпляр класса RegexRedaction.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | регулярное выражение | java.util.regex.Pattern | Регулярное выражение для поиска и замены |
|
|  | options | [ReplacementOptions](../../com.groupdocs.redaction.redactions/replacementoptions) | Параметры замены (текстовые, цветовые) |
|

### getRegularExpression() {#getRegularExpression--}
```
public final Pattern getRegularExpression()
```


Получает регулярное выражение для сопоставления.


**Returns:**
java.util.regex.Pattern - Регулярное выражение для сопоставления.

### getDescription() {#getDescription--}
```
public String getDescription()
```


Возвращает строку, описывающую редактирование и его параметры.


**Returns:**
java.lang.String - Текст, содержащий название редактирования и параметры.

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

