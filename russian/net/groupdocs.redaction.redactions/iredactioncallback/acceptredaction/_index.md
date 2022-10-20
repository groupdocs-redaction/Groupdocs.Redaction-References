---
title: AcceptRedaction
second_title: Справочник по API GroupDocs.Redaction для .NET
description: Этот вызов запускается непосредственно перед внесением какихлибо правок в документ и позволяет зарегистрировать или запретить их.
type: docs
weight: 10
url: /ru/net/groupdocs.redaction.redactions/iredactioncallback/acceptredaction/
---
## IRedactionCallback.AcceptRedaction method

Этот вызов запускается непосредственно перед внесением каких-либо правок в документ и позволяет зарегистрировать или запретить их.

```csharp
public bool AcceptRedaction(RedactionDescription description)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| description | RedactionDescription | Содержит информацию о конкретном типе соответствия, критериях, тексте и позиции |

### Возвращаемое значение

Возвратите true, чтобы принять или false, чтобы отклонить редактирование конкретного совпадения.

### Смотрите также

* class [RedactionDescription](../../redactiondescription)
* interface [IRedactionCallback](../../iredactioncallback)
* пространство имен [GroupDocs.Redaction.Redactions](../../iredactioncallback)
* сборка [GroupDocs.Redaction](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Redaction.dll -->