---
title: RedactionDescription
second_title: Справочник по API GroupDocs.Redaction для .NET
description: Представляет информацию об одном действии изменения выполненном в процессе редактирования.
type: docs
weight: 570
url: /ru/net/groupdocs.redaction.redactions/redactiondescription/
---
## RedactionDescription class

Представляет информацию об одном действии изменения, выполненном в процессе редактирования.

```csharp
public class RedactionDescription
```

## Конструкторы

| Имя | Описание |
| --- | --- |
| [RedactionDescription](redactiondescription#constructor_1)(RedactionType, RedactionActionType, string) | Инициализирует новый экземпляр класса RedactionDescription без информации о замене. |
| [RedactionDescription](redactiondescription#constructor)(RedactionType, RedactionActionType, RegionReplacementOptions, string) | Инициализирует новый экземпляр класса RedactionDescription с информацией о замене области изображения. |
| [RedactionDescription](redactiondescription#constructor_2)(RedactionType, RedactionActionType, string, TextReplacement) | Инициализирует новый экземпляр класса RedactionDescription с информацией о замене. |

## Характеристики

| Имя | Описание |
| --- | --- |
| [ActionType](../../groupdocs.redaction.redactions/redactiondescription/actiontype) { get; } | Получает операцию редактирования: замену, очистку или удаление. |
| [Details](../../groupdocs.redaction.redactions/redactiondescription/details) { get; set; } | Получает или задает дополнительные сведения о редактируемом элементе. |
| [ImageAreaReplacement](../../groupdocs.redaction.redactions/redactiondescription/imageareareplacement) { get; } | Получает информацию о замене для исправлений области изображения, возвращает null для текстовых исправлений. |
| [OriginalText](../../groupdocs.redaction.redactions/redactiondescription/originaltext) { get; } | Получает соответствующий текст, если указано какое-либо выражение. |
| [RedactionType](../../groupdocs.redaction.redactions/redactiondescription/redactiontype) { get; } | Получает тип данных документа — текст, метаданные или аннотации. |
| [Replacement](../../groupdocs.redaction.redactions/redactiondescription/replacement) { get; } | Получает информацию о замене, может быть нулевым. |

### Примечания

**Узнать больше**

* Подробнее о классе RedactionDescription и интерфейсе IRedactionCallback: [Использовать обратный вызов редактирования](https://docs.groupdocs.com/redaction/net/use-redaction-callback/)

### Смотрите также

* пространство имен [GroupDocs.Redaction.Redactions](../../groupdocs.redaction.redactions)
* сборка [GroupDocs.Redaction](../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Redaction.dll -->
