---
title: CellColumnRedaction
second_title: GroupDocs.Redaction for Java API Reference
description: Represents a text redaction that replaces text in a spreadsheet documents CSV Excel etc..
type: docs
weight: 11
url: /java/com.groupdocs.redaction.redactions/cellcolumnredaction/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.redaction.Redaction](../../com.groupdocs.redaction/redaction), [com.groupdocs.redaction.redactions.TextRedaction](../../com.groupdocs.redaction.redactions/textredaction)
```
public class CellColumnRedaction extends TextRedaction
```

Represents a text redaction that replaces text in a spreadsheet documents (CSV, Excel, etc.).

--------------------

**Learn more**

 *  More details about applying redactions: [Redaction basics][]
 *  More details about spreadsheet redactions: [Spreadsheet redactions][]

The following example demonstrates removing user emails from a second column on "Customers" worksheet of a spreadsheet document.

```

  try (Redactor redactor = new Redactor("D:\\Sales in September.xslx"))
 {
    CellFilter filter = new CellFilter();
    filter.setColumnIndex(1); // zero-based 2nd column
    filter.setWorkSheetName("Customers");

    Pattern expression = Pattern.compile("^\\w+([-+.']\\w+)*@\\w+([-.]\\w+)*\\.\\w+([-.]\\w+)*$");
    RedactorChangeLog changeLog = redactor.apply(new CellColumnRedaction(filter, expression, new ReplacementOptions("[customer email]")));
    if (result.Status != RedactionStatus.Failed)
    {
       SaveOptions opt = new SaveOptions();
       opt.setAddSuffix(true);
       doc.save(opt);
    };
 }
 
```


[Redaction basics]: https://docs.groupdocs.com/redaction/java/redaction-basics/
[Spreadsheet redactions]: https://docs.groupdocs.com/redaction/java/spreadsheet-redactions/
## Constructors

| Constructor | Description |
| --- | --- |
| [CellColumnRedaction(CellFilter filter, Pattern regEx, ReplacementOptions options)](#CellColumnRedaction-com.groupdocs.redaction.redactions.CellFilter-java.util.regex.Pattern-com.groupdocs.redaction.redactions.ReplacementOptions-) | Initializes a new instance of CellColumnRedaction class. |
## Methods

| Method | Description |
| --- | --- |
| [getPattern()](#getPattern--) | Gets the regular expression to match. |
| [getFilter()](#getFilter--) | Gets the column and worksheet filter. |
| [getDescription()](#getDescription--) | Returns a string, describing the redaction and its parameters. |
| [applyTo(DocumentFormatInstance formatInstance)](#applyTo-com.groupdocs.redaction.integration.DocumentFormatInstance-) | Applies the redaction to a given format instance. |
### CellColumnRedaction(CellFilter filter, Pattern regEx, ReplacementOptions options) {#CellColumnRedaction-com.groupdocs.redaction.redactions.CellFilter-java.util.regex.Pattern-com.groupdocs.redaction.redactions.ReplacementOptions-}
```
public CellColumnRedaction(CellFilter filter, Pattern regEx, ReplacementOptions options)
```


Initializes a new instance of CellColumnRedaction class.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| filter | [CellFilter](../../com.groupdocs.redaction.redactions/cellfilter) | Column and worksheet filter |
| regEx | java.util.regex.Pattern | Regular expression to search and replace |
| options | [ReplacementOptions](../../com.groupdocs.redaction.redactions/replacementoptions) | Replacement options |

### getPattern() {#getPattern--}
```
public final Pattern getPattern()
```


Gets the regular expression to match.

**Returns:**
java.util.regex.Pattern - The regular expression to match.
### getFilter() {#getFilter--}
```
public final CellFilter getFilter()
```


Gets the column and worksheet filter.

**Returns:**
[CellFilter](../../com.groupdocs.redaction.redactions/cellfilter) - The column and worksheet filter.
### getDescription() {#getDescription--}
```
public String getDescription()
```


Returns a string, describing the redaction and its parameters.

**Returns:**
java.lang.String - Text, containing redaction name and parameters.
### applyTo(DocumentFormatInstance formatInstance) {#applyTo-com.groupdocs.redaction.integration.DocumentFormatInstance-}
```
public RedactorLogEntry applyTo(DocumentFormatInstance formatInstance)
```


Applies the redaction to a given format instance.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| formatInstance | [DocumentFormatInstance](../../com.groupdocs.redaction.integration/documentformatinstance) | An instance of a document to apply redaction |

**Returns:**
[RedactorLogEntry](../../com.groupdocs.redaction/redactorlogentry) - Status of the redaction: success/failure and error message if any
