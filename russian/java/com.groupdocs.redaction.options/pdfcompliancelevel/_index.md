---
title: "PdfComplianceLevel"
second_title: "GroupDocs.Redaction для Java API Reference"
description: "Представляет список поддерживаемых уровней соответствия PDF."
type: docs
weight: 20
url: /ru/java/com.groupdocs.redaction.options/pdfcompliancelevel/
---
**Inheritance:**
java.lang.Object, java.lang.Enum
```
public enum PdfComplianceLevel extends Enum<PdfComplianceLevel>
```

Представляет список поддерживаемых уровней соответствия PDF.

## Поля

| Поле | Описание |
| --- | --- |
|  | [Auto](#Auto) | По умолчанию выходной файл будет соответствовать стандарту PDF/A-1b. |
|
|  | [PdfA1a](#PdfA1a) | Выходной файл будет соответствовать стандарту PDF/A-1a. |
|
## Методы

| Метод | Описание |
| --- | --- |
| [values()](#values--) |  |
| [valueOf(String name)](#valueOf-java.lang.String-) |  |
### Auto {#Auto}
```
public static final PdfComplianceLevel Auto
```


По умолчанию выходной файл будет соответствовать стандарту PDF/A-1b.


### PdfA1a {#PdfA1a}
```
public static final PdfComplianceLevel PdfA1a
```


Выходной файл будет соответствовать стандарту PDF/A-1a.


### values() {#values--}
```
public static PdfComplianceLevel[] values()
```




**Returns:**
com.groupdocs.redaction.options.PdfComplianceLevel[]
### valueOf(String name) {#valueOf-java.lang.String-}
```
public static PdfComplianceLevel valueOf(String name)
```




**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| имя | java.lang.String |  |

**Returns:**
[PdfComplianceLevel](../../com.groupdocs.redaction.options/pdfcompliancelevel)
