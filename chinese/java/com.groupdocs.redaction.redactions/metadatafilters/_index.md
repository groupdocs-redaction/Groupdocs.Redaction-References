---
title: "MetadataFilters"
second_title: "GroupDocs.Redaction for Java API 参考"
description: "表示最常见的文档元数据类型列表。"
type: docs
weight: 19
url: /zh/java/com.groupdocs.redaction.redactions/metadatafilters/
---
**Inheritance:**
java.lang.Object
```
public final class MetadataFilters
```

表示最常见的文档元数据类型列表。

## 构造函数

| 构造函数 | 描述 |
| --- | --- |
| [MetadataFilters()](#MetadataFilters--) |  |
## 字段

| 字段 | 描述 |
| --- | --- |
|  | [None](#None) | 空过滤设置，不匹配任何元数据项。 |
|
|  | [Author](#Author) | 文档的作者。 |
|
|  | [Category](#Category) | 文档的类别。 |
|
|  | [Comments](#Comments) | 文档的注释。 |
|
|  | [Company](#Company) | 作者的公司。 |
|
|  | [ContentStatus](#ContentStatus) | 内容状态。 |
|
|  | [CreatedTime](#CreatedTime) | 创建时间。 |
|
|  | [HyperlinkBase](#HyperlinkBase) | 超链接基址。 |
|
|  | [LastPrinted](#LastPrinted) | 上次打印的日期和时间。 |
|
|  | [LastSavedBy](#LastSavedBy) | 上次由用户保存。 |
|
|  | [LastSavedTime](#LastSavedTime) | 上次保存的日期和时间。 |
|
|  | [NameOfApplication](#NameOfApplication) | 创建文档的应用程序名称。 |
|
|  | [Manager](#Manager) | 作者的经理姓名。 |
|
|  | [RevisionNumber](#RevisionNumber) | 修订号。 |
|
|  | [Subject](#Subject) | 文档的主题。 |
|
|  | [Template](#Template) | 文档模板名称。 |
|
|  | [Title](#Title) | 文档标题。 |
|
|  | [TotalEditingTime](#TotalEditingTime) | 总编辑时间。 |
|
|  | [Version](#Version) | 文档版本。 |
|
|  | [Description](#Description) | 文档描述。 |
|
|  | [Keywords](#Keywords) | 文档关键字。 |
|
|  | [ContentType](#ContentType) | 内容类型。 |
|
|  | [All](#All) | 所有元数据项的类型。 |
|
## 方法

| 方法 | 描述 |
| --- | --- |
|  | [getNames()](#getNames--) | 获取包含所有声明的过滤器类型的集合。 |
|
|  | [getValueByName(String valueName)](#getValueByName-java.lang.String-) | 通过名称获取 MetadataFiler 的值。 |
|
|  | [parse(String values)](#parse-java.lang.String-) | 将逗号分隔的 MetadataFilers 值字符串解析为整数。 |
|
|  | [toString(int value)](#toString-int-) | 将整数保存为逗号分隔的 MetadataFilers 值的字符串。 |
|
### MetadataFilters() {#MetadataFilters--}
```
public MetadataFilters()
```


### None {#None}
```
public static final int None
```


空过滤设置，不匹配任何元数据项。


### Author {#Author}
```
public static final int Author
```


文档的作者。


### Category {#Category}
```
public static final int Category
```


文档的类别。


### Comments {#Comments}
```
public static final int Comments
```


文档的注释。


### Company {#Company}
```
public static final int Company
```


作者的公司。


### ContentStatus {#ContentStatus}
```
public static final int ContentStatus
```


内容状态。


### CreatedTime {#CreatedTime}
```
public static final int CreatedTime
```


创建时间。


### HyperlinkBase {#HyperlinkBase}
```
public static final int HyperlinkBase
```


超链接基址。


### LastPrinted {#LastPrinted}
```
public static final int LastPrinted
```


上次打印的日期和时间。


### LastSavedBy {#LastSavedBy}
```
public static final int LastSavedBy
```


上次由用户保存。


### LastSavedTime {#LastSavedTime}
```
public static final int LastSavedTime
```


上次保存的日期和时间。


### NameOfApplication {#NameOfApplication}
```
public static final int NameOfApplication
```


创建文档的应用程序名称。


### Manager {#Manager}
```
public static final int Manager
```


作者的经理姓名。


### RevisionNumber {#RevisionNumber}
```
public static final int RevisionNumber
```


修订号。


### Subject {#Subject}
```
public static final int Subject
```


文档的主题。


### Template {#Template}
```
public static final int Template
```


文档模板名称。


### Title {#Title}
```
public static final int Title
```


文档标题。


### TotalEditingTime {#TotalEditingTime}
```
public static final int TotalEditingTime
```


总编辑时间。


### Version {#Version}
```
public static final int Version
```


文档版本。


### Description {#Description}
```
public static final int Description
```


文档描述。


### Keywords {#Keywords}
```
public static final int Keywords
```


文档关键字。


### ContentType {#ContentType}
```
public static final int ContentType
```


内容类型。


### All {#All}
```
public static final int All
```


所有元数据项的类型。


### getNames() {#getNames--}
```
public static Set<String> getNames()
```


获取包含所有声明的过滤器类型的集合。


**Returns:**
java.util.Set<java.lang.String> - 包含所有已声明过滤器类型的集合。

### getValueByName(String valueName) {#getValueByName-java.lang.String-}
```
public static int getValueByName(String valueName)
```


通过名称获取 MetadataFiler 的值。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | valueName | java.lang.String | MetadataFilter 的名称。 |
|

**Returns:**
int - MetadataFiler 的值。

### parse(String values) {#parse-java.lang.String-}
```
public static int parse(String values)
```


将逗号分隔的 MetadataFilers 值字符串解析为整数。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | values | java.lang.String | 逗号分隔的 MetadataFilers 值的字符串。 |
|

**Returns:**
int - MetadataFilers 的值。

### toString(int value) {#toString-int-}
```
public static String toString(int value)
```


将整数保存为逗号分隔的 MetadataFilers 值的字符串。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | 值 | int | MetadataFiler 的值。 |
|

**Returns:**
java.lang.String - 逗号分隔的 MetadataFiler 值的字符串。

