---
title: RemovePageRedaction
second_title: Справочник по API GroupDocs.Redaction для .NET
description: Представляет редактирование которое удаляет страницу слайд рабочий лист и т. д. из документа.
type: docs
weight: 610
url: /ru/net/groupdocs.redaction.redactions/removepageredaction/
---
## RemovePageRedaction class

Представляет редактирование, которое удаляет страницу (слайд, рабочий лист и т. д.) из документа.

```csharp
public class RemovePageRedaction : Redaction
```

## Конструкторы

| Имя | Описание |
| --- | --- |
| [RemovePageRedaction](removepageredaction)(PageSeekOrigin, int, int) | Инициализирует новый экземпляр класса RemovePageRedaction. |

## Характеристики

| Имя | Описание |
| --- | --- |
| [Count](../../groupdocs.redaction.redactions/removepageredaction/count) { get; } | Получает количество страниц для удаления. |
| virtual [Description](../../groupdocs.redaction/redaction/description) { get; } | Возвращает строку, описывающую редактирование и его параметры. |
| [Index](../../groupdocs.redaction.redactions/removepageredaction/index) { get; } | Получает индекс начальной позиции (на основе 0). |
| [Origin](../../groupdocs.redaction.redactions/removepageredaction/origin) { get; } | Получает исходную позицию поиска, начало или конец документа. |

## Методы

| Имя | Описание |
| --- | --- |
| override [ApplyTo](../../groupdocs.redaction.redactions/removepageredaction/applyto)(DocumentFormatInstance) | Применяет редактирование к заданному экземпляру формата. |

### Примечания

**Узнать больше**

* Подробнее о применении правок: [Основы редактирования](https://docs.groupdocs.com/redaction/net/redaction-basics/)
* Подробнее об удалении страниц: [Удалить редактирование страницы](https://docs.groupdocs.com/redaction/net/remove-page-redaction/)

### Примеры

В следующем примере показано, как удалить последнюю страницу документа.

```csharp
using (Redactor redactor = new Redactor(@"C:\test.pdf"))
{
   redactor.Apply(new RemovePageRedaction(PageSeekOrigin.End, 0, 1));
   redactor.Save()
}
```

### Смотрите также

* class [Redaction](../../groupdocs.redaction/redaction)
* пространство имен [GroupDocs.Redaction.Redactions](../../groupdocs.redaction.redactions)
* сборка [GroupDocs.Redaction](../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Redaction.dll -->
