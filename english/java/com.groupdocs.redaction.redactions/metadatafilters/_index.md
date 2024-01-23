---
title: MetadataFilters
second_title: GroupDocs.Redaction for Java API Reference
description: Represents a list of the most common types of document metadata.
type: docs
weight: 17
url: /java/com.groupdocs.redaction.redactions/metadatafilters/
---
**Inheritance:**
java.lang.Object
```
public final class MetadataFilters
```

Represents a list of the most common types of document metadata.
## Constructors

| Constructor | Description |
| --- | --- |
| [MetadataFilters()](#MetadataFilters--) |  |
## Fields

| Field | Description |
| --- | --- |
| [None](#None) | Empty filter setting, matches no metadata items. |
| [Author](#Author) | Author of the document. |
| [Category](#Category) | Category of the document. |
| [Comments](#Comments) | Comment for the document. |
| [Company](#Company) | Company of the Author. |
| [ContentStatus](#ContentStatus) | Content status. |
| [CreatedTime](#CreatedTime) | Created time. |
| [HyperlinkBase](#HyperlinkBase) | Hyperlink base. |
| [LastPrinted](#LastPrinted) | Last printed date and time. |
| [LastSavedBy](#LastSavedBy) | Last saved by user. |
| [LastSavedTime](#LastSavedTime) | Last saved date and time. |
| [NameOfApplication](#NameOfApplication) | Name of application where the document was created. |
| [Manager](#Manager) | Author's manager name. |
| [RevisionNumber](#RevisionNumber) | Revision number. |
| [Subject](#Subject) | Subject of the document. |
| [Template](#Template) | Document template name. |
| [Title](#Title) | Document title. |
| [TotalEditingTime](#TotalEditingTime) | Total editing time. |
| [Version](#Version) | Document's version. |
| [Description](#Description) | Document's description. |
| [Keywords](#Keywords) | Document's keywords. |
| [ContentType](#ContentType) | Content type. |
| [All](#All) | All types of the metadata items. |
## Methods

| Method | Description |
| --- | --- |
| [getNames()](#getNames--) | Gets a set with all declared filter types. |
| [getValueByName(String valueName)](#getValueByName-java.lang.String-) | Gets value of MetadataFiler by its name. |
| [parse(String values)](#parse-java.lang.String-) | Parses a string of comma-delimited MetadataFilers values into an int. |
| [toString(int value)](#toString-int-) | Saves an integer as a string of comma-delimited MetadataFilers values. |
### MetadataFilters() {#MetadataFilters--}
```
public MetadataFilters()
```


### None {#None}
```
public static final int None
```


Empty filter setting, matches no metadata items.

### Author {#Author}
```
public static final int Author
```


Author of the document.

### Category {#Category}
```
public static final int Category
```


Category of the document.

### Comments {#Comments}
```
public static final int Comments
```


Comment for the document.

### Company {#Company}
```
public static final int Company
```


Company of the Author.

### ContentStatus {#ContentStatus}
```
public static final int ContentStatus
```


Content status.

### CreatedTime {#CreatedTime}
```
public static final int CreatedTime
```


Created time.

### HyperlinkBase {#HyperlinkBase}
```
public static final int HyperlinkBase
```


Hyperlink base.

### LastPrinted {#LastPrinted}
```
public static final int LastPrinted
```


Last printed date and time.

### LastSavedBy {#LastSavedBy}
```
public static final int LastSavedBy
```


Last saved by user.

### LastSavedTime {#LastSavedTime}
```
public static final int LastSavedTime
```


Last saved date and time.

### NameOfApplication {#NameOfApplication}
```
public static final int NameOfApplication
```


Name of application where the document was created.

### Manager {#Manager}
```
public static final int Manager
```


Author's manager name.

### RevisionNumber {#RevisionNumber}
```
public static final int RevisionNumber
```


Revision number.

### Subject {#Subject}
```
public static final int Subject
```


Subject of the document.

### Template {#Template}
```
public static final int Template
```


Document template name.

### Title {#Title}
```
public static final int Title
```


Document title.

### TotalEditingTime {#TotalEditingTime}
```
public static final int TotalEditingTime
```


Total editing time.

### Version {#Version}
```
public static final int Version
```


Document's version.

### Description {#Description}
```
public static final int Description
```


Document's description.

### Keywords {#Keywords}
```
public static final int Keywords
```


Document's keywords.

### ContentType {#ContentType}
```
public static final int ContentType
```


Content type.

### All {#All}
```
public static final int All
```


All types of the metadata items.

### getNames() {#getNames--}
```
public static Set<String> getNames()
```


Gets a set with all declared filter types.

**Returns:**
java.util.Set<java.lang.String> - A set with all declared filter types.
### getValueByName(String valueName) {#getValueByName-java.lang.String-}
```
public static int getValueByName(String valueName)
```


Gets value of MetadataFiler by its name.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| valueName | java.lang.String | Name of MetadataFilter. |

**Returns:**
int - Value of MetadataFiler.
### parse(String values) {#parse-java.lang.String-}
```
public static int parse(String values)
```


Parses a string of comma-delimited MetadataFilers values into an int.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| values | java.lang.String | A string of comma-delimited MetadataFilers values. |

**Returns:**
int - Value of MetadataFilers.
### toString(int value) {#toString-int-}
```
public static String toString(int value)
```


Saves an integer as a string of comma-delimited MetadataFilers values.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int | Value of MetadataFiler. |

**Returns:**
java.lang.String - A string of comma-delimited MetadataFiler values.
