---
title: "ExactPhraseRedaction"
second_title: "GroupDocs.Redaction для Java API Reference"
description: "Представляет редактирование текста, которое заменяет точную фразу в тексте документа без учёта регистра по умолчанию."
type: docs
weight: 17
url: /ru/java/com.groupdocs.redaction.redactions/exactphraseredaction/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.redaction.Redaction](../../com.groupdocs.redaction/redaction), [com.groupdocs.redaction.redactions.TextRedaction](../../com.groupdocs.redaction.redactions/textredaction)
```
public class ExactPhraseRedaction extends TextRedaction
```

Представляет текстовое редактирование, которое заменяет точную фразу в тексте документа, по умолчанию без учёта регистра.

*** ** * ** ***


**Learn more**

* More details about applying redactions: [Redaction basics](../https://docs.groupdocs.com/redaction/java/redaction-basics/)
* More details about document text redactions: [Text redactions](../https://docs.groupdocs.com/redaction/java/text-redactions/)

<br />

Следующий пример демонстрирует выполнение поиска и замены фразы с учётом регистра.

````

  try (Redactor redactor = new Redactor("C:\\sample.pdf"))
 {
   // By default, the second parameter, isCaseSensitive = false;
   doc.apply(new ExactPhraseRedaction("John Doe", true, new ReplacementOptions("[personal]")));
   doc.save();
 }
 
``` 
````

The following example demonstrates replacing phrase (case insensitive) with solid red rectangle.

````

try (Redactor redactor = new Redactor("C:\\sample.pdf"))
{
// By default, isCaseSensitive = false;
doc.apply(new ExactPhraseRedaction("John Doe", new ReplacementOptions(System.Drawing.Color.Red)));
doc.save();
}
 
``` 
````


## Конструкторы

| Конструктор | Описание |
| --- | --- |
|  | [ExactPhraseRedaction(String searchPhrase, ReplacementOptions options)](#ExactPhraseRedaction-java.lang.String-com.groupdocs.redaction.redactions.ReplacementOptions-) | Инициализирует новый экземпляр класса ExactPhraseRedaction в режиме без учёта регистра. |
|
|  | [ExactPhraseRedaction(String searchPhrase, boolean isCaseSensitive, ReplacementOptions options)](#ExactPhraseRedaction-java.lang.String-boolean-com.groupdocs.redaction.redactions.ReplacementOptions-) | Инициализирует новый экземпляр класса ExactPhraseRedaction. |
|
## Методы

| Метод | Описание |
| --- | --- |
|  | [getSearchPhrase()](#getSearchPhrase--) | Получает строку для поиска и замены. |
|
|  | [isCaseSensitive()](#isCaseSensitive--) | Получает значение, указывающее, чувствителен ли поиск к регистру или нет. |
|
|  | [isRightToLeft()](#isRightToLeft--) | Получает значение, указывающее, является ли этот текст справа налево, или нет; по умолчанию false. |
|
|  | [setRightToLeft(boolean value)](#setRightToLeft-boolean-) | Устанавливает значение, указывающее, является ли этот текст справа налево, или нет; по умолчанию false. |
|
|  | [getDescription()](#getDescription--) | Возвращает строку, описывающую редактирование и его параметры. |
|
|  | [applyTo(DocumentFormatInstance formatInstance)](#applyTo-com.groupdocs.redaction.integration.DocumentFormatInstance-) | Применяет редактирование к заданному экземпляру формата. |
|
### ExactPhraseRedaction(String searchPhrase, ReplacementOptions options) {#ExactPhraseRedaction-java.lang.String-com.groupdocs.redaction.redactions.ReplacementOptions-}
```
public ExactPhraseRedaction(String searchPhrase, ReplacementOptions options)
```


Инициализирует новый экземпляр класса ExactPhraseRedaction в режиме без учёта регистра.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | searchPhrase | java.lang.String | Строка для поиска и замены |
|
|  | options | [ReplacementOptions](../../com.groupdocs.redaction.redactions/replacementoptions) | Параметры замены (текстовые, цветовые) |
|

### ExactPhraseRedaction(String searchPhrase, boolean isCaseSensitive, ReplacementOptions options) {#ExactPhraseRedaction-java.lang.String-boolean-com.groupdocs.redaction.redactions.ReplacementOptions-}
```
public ExactPhraseRedaction(String searchPhrase, boolean isCaseSensitive, ReplacementOptions options)
```


Инициализирует новый экземпляр класса ExactPhraseRedaction.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | searchPhrase | java.lang.String | Строка для поиска и замены |
|
|  | isCaseSensitive | boolean | True если требуется поиск с учётом регистра |
|
|  | options | [ReplacementOptions](../../com.groupdocs.redaction.redactions/replacementoptions) | Параметры замены (текстовые, цветовые) |
|

### getSearchPhrase() {#getSearchPhrase--}
```
public final String getSearchPhrase()
```


Получает строку для поиска и замены.


**Returns:**
java.lang.String - Строка для поиска и замены.

### isCaseSensitive() {#isCaseSensitive--}
```
public final boolean isCaseSensitive()
```


Получает значение, указывающее, чувствителен ли поиск к регистру или нет.


**Returns:**
boolean - Значение, указывающее, чувствителен ли поиск к регистру или нет.

### isRightToLeft() {#isRightToLeft--}
```
public final boolean isRightToLeft()
```


Получает значение, указывающее, является ли этот текст справа налево, или нет; по умолчанию false.


**Returns:**
boolean - Значение, указывающее, является ли этот текст справа налево, или нет; по умолчанию false.

### setRightToLeft(boolean value) {#setRightToLeft-boolean-}
```
public final void setRightToLeft(boolean value)
```


Устанавливает значение, указывающее, является ли этот текст справа налево, или нет; по умолчанию false.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | значение | boolean | Значение, указывающее, является ли этот текст справа налево, или нет; по умолчанию false. |
|

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

