---
title: "WordprocessingSaveOptions"
second_title: "GroupDocs.Redaction для Java API Reference"
description: "Параметры сохранения обработки текста."
type: docs
weight: 15
url: /ru/java/com.groupdocs.redaction.options/wordprocessingsaveoptions/
---
**Inheritance:**
java.lang.Object
```
public class WordprocessingSaveOptions
```

Параметры сохранения обработки текста.

## Конструкторы

| Конструктор | Описание |
| --- | --- |
| [WordprocessingSaveOptions()](#WordprocessingSaveOptions--) |  |
## Методы

| Метод | Описание |
| --- | --- |
|  | [getOoxmlCompliance()](#getOoxmlCompliance--) | Соответствие OOXML, применяемое при сохранении. |
|
| [setOoxmlCompliance(WordProcessingComplianceLevel value)](#setOoxmlCompliance-com.groupdocs.redaction.options.WordProcessingComplianceLevel-) |  |
### WordprocessingSaveOptions() {#WordprocessingSaveOptions--}
```
public WordprocessingSaveOptions()
```


### getOoxmlCompliance() {#getOoxmlCompliance--}
```
public final WordProcessingComplianceLevel getOoxmlCompliance()
```


Соответствие OOXML, применяемое при сохранении.  null  сохраняет исходный уровень документа. Strict нельзя сохранить напрямую как Ecma; сначала используйте Transitional.


**Returns:**
[WordProcessingComplianceLevel](../../com.groupdocs.redaction.options/wordprocessingcompliancelevel)
### setOoxmlCompliance(WordProcessingComplianceLevel value) {#setOoxmlCompliance-com.groupdocs.redaction.options.WordProcessingComplianceLevel-}
```
public final void setOoxmlCompliance(WordProcessingComplianceLevel value)
```




**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| value | [WordProcessingComplianceLevel](../../com.groupdocs.redaction.options/wordprocessingcompliancelevel) |  |

