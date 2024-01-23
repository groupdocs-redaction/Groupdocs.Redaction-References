---
title: MetadataItem
second_title: GroupDocs.Redaction for Java API Reference
description: Represents an item of metadata common for all supported formats and used in metadata redactions.
type: docs
weight: 12
url: /java/com.groupdocs.redaction.integration/metadataitem/
---
**Inheritance:**
java.lang.Object
```
public class MetadataItem
```

Represents an item of metadata, common for all supported formats and used in metadata redactions.
## Constructors

| Constructor | Description |
| --- | --- |
| [MetadataItem()](#MetadataItem--) | Initializes a new instance. |
## Methods

| Method | Description |
| --- | --- |
| [getOriginalName()](#getOriginalName--) | Gets an original name of the metadata item, as it appears in the document. |
| [setOriginalName(String value)](#setOriginalName-java.lang.String-) | Sets an original name of the metadata item, as it appears in the document. |
| [getCategory()](#getCategory--) | Gets a category of the metadata item, for example resource ID for an embedded resource metadata item. |
| [setCategory(String value)](#setCategory-java.lang.String-) | Sets a category of the metadata item, for example resource ID for an embedded resource metadata item. |
| [getFilter()](#getFilter--) | Gets a value of  MetadataFilters , assigned to this metadata item which is used in item filtration. |
| [setFilter(int value)](#setFilter-int-) | Sets a value of  MetadataFilters , assigned to this metadata item which is used in item filtration. |
| [getValues()](#getValues--) | Gets the metadata item value. |
| [setValues(List<String> value)](#setValues-java.util.List-java.lang.String--) | Sets the metadata item value. |
| [isCustom()](#isCustom--) | Gets a value indicating whether this item is custom (added by the authors of the document). |
| [setCustom(boolean value)](#setCustom-boolean-) | Sets a value indicating whether this item is custom (added by the authors of the document). |
| [getDictionaryKey()](#getDictionaryKey--) | Gets a dictionary key for , using its OriginalName and other data. |
| [createClone()](#createClone--) | Creates a deep clone of current instance. |
| [getActualValue()](#getActualValue--) | Gets the string representation of the metadata item value. |
### MetadataItem() {#MetadataItem--}
```
public MetadataItem()
```


Initializes a new instance.

### getOriginalName() {#getOriginalName--}
```
public final String getOriginalName()
```


Gets an original name of the metadata item, as it appears in the document.

**Returns:**
java.lang.String - An original name of the metadata item, as it appears in the document.
### setOriginalName(String value) {#setOriginalName-java.lang.String-}
```
public final void setOriginalName(String value)
```


Sets an original name of the metadata item, as it appears in the document.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String | An original name of the metadata item, as it appears in the document. |

### getCategory() {#getCategory--}
```
public final String getCategory()
```


Gets a category of the metadata item, for example resource ID for an embedded resource metadata item.

**Returns:**
java.lang.String - A category of the metadata item, for example resource ID for an embedded resource metadata item.
### setCategory(String value) {#setCategory-java.lang.String-}
```
public final void setCategory(String value)
```


Sets a category of the metadata item, for example resource ID for an embedded resource metadata item.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String | A category of the metadata item, for example resource ID for an embedded resource metadata item. |

### getFilter() {#getFilter--}
```
public final int getFilter()
```


Gets a value of  MetadataFilters , assigned to this metadata item which is used in item filtration.

**Returns:**
int - A value of  MetadataFilters , assigned to this metadata item which is used in item filtration.
### setFilter(int value) {#setFilter-int-}
```
public final void setFilter(int value)
```


Sets a value of  MetadataFilters , assigned to this metadata item which is used in item filtration.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int | A value of  MetadataFilters , assigned to this metadata item which is used in item filtration. |

### getValues() {#getValues--}
```
public final List<String> getValues()
```


Gets the metadata item value.

**Returns:**
java.util.List<java.lang.String> - The metadata item value.
### setValues(List<String> value) {#setValues-java.util.List-java.lang.String--}
```
public final void setValues(List<String> value)
```


Sets the metadata item value.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.util.List<java.lang.String> | The metadata item value. |

### isCustom() {#isCustom--}
```
public final boolean isCustom()
```


Gets a value indicating whether this item is custom (added by the authors of the document).

**Returns:**
boolean - A value indicating whether this item is custom (added by the authors of the document).
### setCustom(boolean value) {#setCustom-boolean-}
```
public final void setCustom(boolean value)
```


Sets a value indicating whether this item is custom (added by the authors of the document).

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | A value indicating whether this item is custom (added by the authors of the document). |

### getDictionaryKey() {#getDictionaryKey--}
```
public String getDictionaryKey()
```


Gets a dictionary key for , using its OriginalName and other data.

**Returns:**
java.lang.String - A dictionary key for , using its OriginalName and other data.
### createClone() {#createClone--}
```
public MetadataItem createClone()
```


Creates a deep clone of current instance.

**Returns:**
[MetadataItem](../../com.groupdocs.redaction.integration/metadataitem) - Object clone
### getActualValue() {#getActualValue--}
```
public final String getActualValue()
```


Gets the string representation of the metadata item value.

**Returns:**
java.lang.String - The string representation of the metadata item value.
