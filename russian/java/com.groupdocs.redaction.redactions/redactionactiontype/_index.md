---
title: "RedactionActionType"
second_title: "GroupDocs.Redaction для Java API Reference"
description: "Представляет действия, которые можно выполнить для редактирования."
type: docs
weight: 37
url: /ru/java/com.groupdocs.redaction.redactions/redactionactiontype/
---
**Inheritance:**
java.lang.Object, java.lang.Enum
```
public enum RedactionActionType extends Enum<RedactionActionType>
```

Представляет действия, которые можно выполнить для редактирования.

## Поля

| Поле | Описание |
| --- | --- |
|  | [Replacement](#Replacement) | Редактированный текст был заменён другим или покрыт блоком. |
|
|  | [Cleanup](#Cleanup) | Данные были удалены, но в документе остаётся пустой объект. |
|
|  | [Deletion](#Deletion) | Данные и связанные структуры были удалены из документа. |
|
## Методы

| Метод | Описание |
| --- | --- |
| [values()](#values--) |  |
| [valueOf(String name)](#valueOf-java.lang.String-) |  |
### Replacement {#Replacement}
```
public static final RedactionActionType Replacement
```


Редактированный текст был заменён другим или покрыт блоком.


### Cleanup {#Cleanup}
```
public static final RedactionActionType Cleanup
```


Данные были удалены, но в документе остаётся пустой объект.


### Deletion {#Deletion}
```
public static final RedactionActionType Deletion
```


Данные и связанные структуры были удалены из документа.


### values() {#values--}
```
public static RedactionActionType[] values()
```




**Returns:**
com.groupdocs.redaction.redactions.RedactionActionType[]
### valueOf(String name) {#valueOf-java.lang.String-}
```
public static RedactionActionType valueOf(String name)
```




**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| имя | java.lang.String |  |

**Returns:**
[RedactionActionType](../../com.groupdocs.redaction.redactions/redactionactiontype)
