---
title: "PdfComplianceLevel"
second_title: "GroupDocs.Redaction for Java API Reference"
description: "지원되는 PDF 호환성 수준 목록을 나타냅니다."
type: docs
weight: 20
url: /ko/java/com.groupdocs.redaction.options/pdfcompliancelevel/
---
**Inheritance:**
java.lang.Object, java.lang.Enum
```
public enum PdfComplianceLevel extends Enum<PdfComplianceLevel>
```

지원되는 PDF 호환성 수준 목록을 나타냅니다.

## 필드

| 필드 | 설명 |
| --- | --- |
|  | [Auto](#Auto) | 출력 파일은 기본적으로 PDF/A-1b 표준을 준수합니다. |
|
|  | [PdfA1a](#PdfA1a) | 출력 파일은 PDF/A-1a 표준을 준수합니다. |
|
## 메서드

| 메서드 | 설명 |
| --- | --- |
| [values()](#values--) |  |
| [valueOf(String name)](#valueOf-java.lang.String-) |  |
### Auto {#Auto}
```
public static final PdfComplianceLevel Auto
```


출력 파일은 기본적으로 PDF/A-1b 표준을 준수합니다.


### PdfA1a {#PdfA1a}
```
public static final PdfComplianceLevel PdfA1a
```


출력 파일은 PDF/A-1a 표준을 준수합니다.


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
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| name | java.lang.String |  |

**Returns:**
[PdfComplianceLevel](../../com.groupdocs.redaction.options/pdfcompliancelevel)
