---
title: WordprocessingSaveOptions
second_title: GroupDocs.Redaction for Java API Reference
description: Word processing save options.
type: docs
weight: 15
url: /java/com.groupdocs.redaction.options/wordprocessingsaveoptions/
---
**Inheritance:**
java.lang.Object
```
public class WordprocessingSaveOptions
```

Word processing save options.

## Constructors

| Constructor | Description |
| --- | --- |
| [WordprocessingSaveOptions()](#WordprocessingSaveOptions--) |  |
## Methods

| Method | Description |
| --- | --- |
| [getOoxmlCompliance()](#getOoxmlCompliance--) | OOXML compliance to apply on save.
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


OOXML compliance to apply on save.  null  keeps the original document level. Strict cannot be saved as Ecma directly; use Transitional first.


**Returns:**
[WordProcessingComplianceLevel](../../com.groupdocs.redaction.options/wordprocessingcompliancelevel)
### setOoxmlCompliance(WordProcessingComplianceLevel value) {#setOoxmlCompliance-com.groupdocs.redaction.options.WordProcessingComplianceLevel-}
```
public final void setOoxmlCompliance(WordProcessingComplianceLevel value)
```




**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [WordProcessingComplianceLevel](../../com.groupdocs.redaction.options/wordprocessingcompliancelevel) |  |

