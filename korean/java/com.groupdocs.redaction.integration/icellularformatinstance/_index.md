---
title: "ICellularFormatInstance"
second_title: "GroupDocs.Redaction for Java API Reference"
description: "하나 이상의 워크시트를 포함하는 스프레드시트 형식에 접근하기 위해 필요한 메서드를 정의합니다."
type: docs
weight: 18
url: /ko/java/com.groupdocs.redaction.integration/icellularformatinstance/
---```
public interface ICellularFormatInstance
```

Defines methods that are required for access to spreadsheet formats, having one or many worksheets.

*** ** * ** ***


**Learn more**

* More details about applying redactions: [Redaction basics](../https://docs.groupdocs.com/redaction/java/redaction-basics/)
* More details about spreadsheet redactions: [Spreadsheet redactions](../https://docs.groupdocs.com/redaction/java/spreadsheet-redactions/)
* More details about implementing custom formats: [Create custom format handler](../https://docs.groupdocs.com/redaction/java/create-custom-format-handler/)

<br />


## Methods

| Method | Description |
| --- | --- |
| [getSheetIndex(String sheetName)](#getSheetIndex-java.lang.String-) | Gets the worksheet index by worksheet name, if possible.
 |
| [replaceInColumn(Pattern regularExpression, String replacement, int column, int sheet)](#replaceInColumn-java.util.regex.Pattern-java.lang.String-int-int-) | Replaces all matches with a given replacement in the specified column and worksheet.
 |
| [replaceInColumn(Pattern regularExpression, String replacement, int column)](#replaceInColumn-java.util.regex.Pattern-java.lang.String-int-) | Replaces all matches with a given replacement in the specified column on all worksheets.
 |
### getSheetIndex(String sheetName) {#getSheetIndex-java.lang.String-}
```
public abstract int getSheetIndex(String sheetName)
```


Gets the worksheet index by worksheet name, if possible.


**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| sheetName | java.lang.String | Worksheet name
 |

**Returns:**
int - Worksheet index or -1 if not found

### replaceInColumn(Pattern regularExpression, String replacement, int column, int sheet) {#replaceInColumn-java.util.regex.Pattern-java.lang.String-int-int-}
```
public abstract RedactionResult replaceInColumn(Pattern regularExpression, String replacement, int column, int sheet)
```


Replaces all matches with a given replacement in the specified column and worksheet.


**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| regularExpression | java.util.regex.Pattern | Regular expression to search and replace
 |
| replacement | java.lang.String | Textual replacement
 |
| column | int | Zero-based column index
 |
| sheet | int | Zero-based worksheet index
 |

**Returns:**
[RedactionResult](../../com.groupdocs.redaction/redactionresult) - Replacement result

### replaceInColumn(Pattern regularExpression, String replacement, int column) {#replaceInColumn-java.util.regex.Pattern-java.lang.String-int-}
```
public abstract RedactionResult replaceInColumn(Pattern regularExpression, String replacement, int column)
```


Replaces all matches with a given replacement in the specified column on all worksheets.


**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| regularExpression | java.util.regex.Pattern | Regular expression to search and replace
 |
| replacement | java.lang.String | Textual replacement
 |
| column | int | Zero-based column index
 |

**Returns:**
[RedactionResult](../../com.groupdocs.redaction/redactionresult) - Replacement result

