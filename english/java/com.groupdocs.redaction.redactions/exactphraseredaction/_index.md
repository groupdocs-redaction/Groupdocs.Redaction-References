---
title: ExactPhraseRedaction
second_title: GroupDocs.Redaction for Java API Reference
description: Represents a text redaction that replaces exact phrase in the documents text case insensitive by default.
type: docs
weight: 15
url: /java/com.groupdocs.redaction.redactions/exactphraseredaction/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.redaction.Redaction](../../com.groupdocs.redaction/redaction), [com.groupdocs.redaction.redactions.TextRedaction](../../com.groupdocs.redaction.redactions/textredaction)
```
public class ExactPhraseRedaction extends TextRedaction
```

Represents a text redaction that replaces exact phrase in the document's text, case insensitive by default.

--------------------

**Learn more**

 *  More details about applying redactions: [Redaction basics][]
 *  More details about document text redactions: [Text redactions][]

The following example demonstrates performing case-sensitive phrase search and replacement.

```

  try (Redactor redactor = new Redactor("C:\\sample.pdf"))
 {
   // By default, the second parameter, isCaseSensitive = false;
   doc.apply(new ExactPhraseRedaction("John Doe", true, new ReplacementOptions("[personal]")));
   doc.save();
 }
 
```

The following example demonstrates replacing phrase (case insensitive) with solid red rectangle.

```

  try (Redactor redactor = new Redactor("C:\\sample.pdf"))
 {
   // By default, isCaseSensitive = false;
   doc.apply(new ExactPhraseRedaction("John Doe", new ReplacementOptions(System.Drawing.Color.Red)));
   doc.save();
 }
 
```


[Redaction basics]: https://docs.groupdocs.com/redaction/java/redaction-basics/
[Text redactions]: https://docs.groupdocs.com/redaction/java/text-redactions/
## Constructors

| Constructor | Description |
| --- | --- |
| [ExactPhraseRedaction(String searchPhrase, ReplacementOptions options)](#ExactPhraseRedaction-java.lang.String-com.groupdocs.redaction.redactions.ReplacementOptions-) | Initializes a new instance of ExactPhraseRedaction class in case insensitive mode. |
| [ExactPhraseRedaction(String searchPhrase, boolean isCaseSensitive, ReplacementOptions options)](#ExactPhraseRedaction-java.lang.String-boolean-com.groupdocs.redaction.redactions.ReplacementOptions-) | Initializes a new instance of ExactPhraseRedaction class. |
## Methods

| Method | Description |
| --- | --- |
| [getSearchPhrase()](#getSearchPhrase--) | Gets the string to search and replace. |
| [isCaseSensitive()](#isCaseSensitive--) | Gets a value indicating whether the search is case-sensitive or not. |
| [isRightToLeft()](#isRightToLeft--) | Gets a value indicating if this text is right-to-Left or not, false by default. |
| [setRightToLeft(boolean value)](#setRightToLeft-boolean-) | Sets a value indicating if this text is right-to-Left or not, false by default. |
| [getDescription()](#getDescription--) | Returns a string, describing the redaction and its parameters. |
| [applyTo(DocumentFormatInstance formatInstance)](#applyTo-com.groupdocs.redaction.integration.DocumentFormatInstance-) | Applies the redaction to a given format instance. |
### ExactPhraseRedaction(String searchPhrase, ReplacementOptions options) {#ExactPhraseRedaction-java.lang.String-com.groupdocs.redaction.redactions.ReplacementOptions-}
```
public ExactPhraseRedaction(String searchPhrase, ReplacementOptions options)
```


Initializes a new instance of ExactPhraseRedaction class in case insensitive mode.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| searchPhrase | java.lang.String | String to search and replace |
| options | [ReplacementOptions](../../com.groupdocs.redaction.redactions/replacementoptions) | Replacement options (textual, color) |

### ExactPhraseRedaction(String searchPhrase, boolean isCaseSensitive, ReplacementOptions options) {#ExactPhraseRedaction-java.lang.String-boolean-com.groupdocs.redaction.redactions.ReplacementOptions-}
```
public ExactPhraseRedaction(String searchPhrase, boolean isCaseSensitive, ReplacementOptions options)
```


Initializes a new instance of ExactPhraseRedaction class.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| searchPhrase | java.lang.String | String to search and replace |
| isCaseSensitive | boolean | True if case sensitive search is required |
| options | [ReplacementOptions](../../com.groupdocs.redaction.redactions/replacementoptions) | Replacement options (textual, color) |

### getSearchPhrase() {#getSearchPhrase--}
```
public final String getSearchPhrase()
```


Gets the string to search and replace.

**Returns:**
java.lang.String - The string to search and replace.
### isCaseSensitive() {#isCaseSensitive--}
```
public final boolean isCaseSensitive()
```


Gets a value indicating whether the search is case-sensitive or not.

**Returns:**
boolean - A value indicating whether the search is case-sensitive or not.
### isRightToLeft() {#isRightToLeft--}
```
public final boolean isRightToLeft()
```


Gets a value indicating if this text is right-to-Left or not, false by default.

**Returns:**
boolean - A value indicating if this text is right-to-Left or not, false by default.
### setRightToLeft(boolean value) {#setRightToLeft-boolean-}
```
public final void setRightToLeft(boolean value)
```


Sets a value indicating if this text is right-to-Left or not, false by default.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | A value indicating if this text is right-to-Left or not, false by default. |

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
