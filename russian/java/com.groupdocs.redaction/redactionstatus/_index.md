---
title: "RedactionStatus"
second_title: "GroupDocs.Redaction для Java API Reference"
description: "Представляет статус завершения редактирования."
type: docs
weight: 20
url: /ru/java/com.groupdocs.redaction/redactionstatus/
---
**Inheritance:**
java.lang.Object, java.lang.Enum
```
public enum RedactionStatus extends Enum<RedactionStatus>
```

Представляет статус завершения редактирования.

## Поля

| Поле | Описание |
| --- | --- |
|  | [Applied](#Applied) | Редактирование было полностью и успешно применено. |
|
|  | [PartiallyApplied](#PartiallyApplied) | Редактирование было применено только к части совпадений. |
|
|  | [Skipped](#Skipped) | Редактирование было пропущено (не применено). |
|
|  | [Failed](#Failed) | Редактирование завершилось неудачей с исключением. |
|
## Методы

| Метод | Описание |
| --- | --- |
| [values()](#values--) |  |
| [valueOf(String name)](#valueOf-java.lang.String-) |  |
### Applied {#Applied}
```
public static final RedactionStatus Applied
```


Редактирование было полностью и успешно применено.


### PartiallyApplied {#PartiallyApplied}
```
public static final RedactionStatus PartiallyApplied
```


Редактирование было применено только к части совпадений.


### Skipped {#Skipped}
```
public static final RedactionStatus Skipped
```


Редактирование было пропущено (не применено).


### Failed {#Failed}
```
public static final RedactionStatus Failed
```


Редактирование завершилось неудачей с исключением.


### values() {#values--}
```
public static RedactionStatus[] values()
```




**Returns:**
com.groupdocs.redaction.RedactionStatus[]
### valueOf(String name) {#valueOf-java.lang.String-}
```
public static RedactionStatus valueOf(String name)
```




**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| имя | java.lang.String |  |

**Returns:**
[RedactionStatus](../../com.groupdocs.redaction/redactionstatus)
