---
title: "WordProcessingComplianceLevel"
second_title: "GroupDocs.Redaction для Java API Reference"
description: "Уровни соответствия OOXML для документов обработки текста."
type: docs
weight: 22
url: /ru/java/com.groupdocs.redaction.options/wordprocessingcompliancelevel/
---
**Inheritance:**
java.lang.Object, java.lang.Enum
```
public enum WordProcessingComplianceLevel extends Enum<WordProcessingComplianceLevel>
```

Уровни соответствия OOXML для документов обработки текста. Strict может быть понижен только до Transitional, но не до Ecma.

## Поля

| Поле | Описание |
| --- | --- |
|  | [Ecma](#Ecma) | ECMA-376 1-е издание, 2006. |
|
|  | [Transitional](#Transitional) | ISO/IEC 29500:2008 Transitional. |
|
|  | [Strict](#Strict) | ISO/IEC 29500:2008 Strict. |
|
## Методы

| Метод | Описание |
| --- | --- |
| [values()](#values--) |  |
| [valueOf(String name)](#valueOf-java.lang.String-) |  |
### Ecma {#Ecma}
```
public static final WordProcessingComplianceLevel Ecma
```


ECMA-376 1-е издание, 2006.


### Transitional {#Transitional}
```
public static final WordProcessingComplianceLevel Transitional
```


ISO/IEC 29500:2008 Transitional.


### Strict {#Strict}
```
public static final WordProcessingComplianceLevel Strict
```


ISO/IEC 29500:2008 Strict.


### values() {#values--}
```
public static WordProcessingComplianceLevel[] values()
```




**Returns:**
com.groupdocs.redaction.options.WordProcessingComplianceLevel[]
### valueOf(String name) {#valueOf-java.lang.String-}
```
public static WordProcessingComplianceLevel valueOf(String name)
```




**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| имя | java.lang.String |  |

**Returns:**
[WordProcessingComplianceLevel](../../com.groupdocs.redaction.options/wordprocessingcompliancelevel)
