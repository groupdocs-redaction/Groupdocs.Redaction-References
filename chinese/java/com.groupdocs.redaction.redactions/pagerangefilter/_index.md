---
title: "PageRangeFilter"
second_title: "GroupDocs.Redaction for Java API 参考"
description: "表示在文档内部设置页面范围以应用编辑的过滤器。"
type: docs
weight: 24
url: /zh/java/com.groupdocs.redaction.redactions/pagerangefilter/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.redaction.redactions.RedactionFilter](../../com.groupdocs.redaction.redactions/redactionfilter)
```
public class PageRangeFilter extends RedactionFilter
```

表示编辑过滤器，设置文档内部的页范围以应用编辑。

*** ** * ** ***


**Learn more**

* More details about applying redactions: [Redaction basics](../https://docs.groupdocs.com/redaction/java/redaction-basics/)
* More details about redaction filters: [Use PDF redaction filters](../https://docs.groupdocs.com/redaction/java/use-pdf-redaction-filters/)

<br />


## 构造函数

| 构造函数 | 描述 |
| --- | --- |
|  | [PageRangeFilter(PageSeekOrigin origin, int index, int count)](#PageRangeFilter-com.groupdocs.redaction.redactions.PageSeekOrigin-int-int-) | 初始化 RemovePageRedaction 类的新实例。 |
|
## 方法

| 方法 | 描述 |
| --- | --- |
|  | [getOrigin()](#getOrigin--) | 获取查找参考位置，文档的开头或结尾。 |
|
|  | [getIndex()](#getIndex--) | 获取起始位置索引（从0开始）。 |
|
|  | [getCount()](#getCount--) | 获取要删除的页面数量。 |
|
|  | [isPageInRange(int pageIndex, int pageCount)](#isPageInRange-int-int-) | 检查此过滤器页面范围是否包含给定页面。 |
|
### PageRangeFilter(PageSeekOrigin origin, int index, int count) {#PageRangeFilter-com.groupdocs.redaction.redactions.PageSeekOrigin-int-int-}
```
public PageRangeFilter(PageSeekOrigin origin, int index, int count)
```


初始化 RemovePageRedaction 类的新实例。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | origin | [PageSeekOrigin](../../com.groupdocs.redaction.redactions/pageseekorigin) | 查找参考位置，文档的开头或结尾 |
|
|  | 索引 | int | 起始位置索引（从0开始） |
|
|  | 计数 | int | 要删除的页面计数 |
|

### getOrigin() {#getOrigin--}
```
public final PageSeekOrigin getOrigin()
```


获取查找参考位置，文档的开头或结尾。


**Returns:**
[PageSeekOrigin](../../com.groupdocs.redaction.redactions/pageseekorigin) - Seek reference position, the beginning or the end of a document.

### getIndex() {#getIndex--}
```
public final int getIndex()
```


获取起始位置索引（从0开始）。


**Returns:**
int - 起始位置索引（基于0）。

### getCount() {#getCount--}
```
public final int getCount()
```


获取要删除的页面数量。


**Returns:**
int - 要删除的页面计数。

### isPageInRange(int pageIndex, int pageCount) {#isPageInRange-int-int-}
```
public final boolean isPageInRange(int pageIndex, int pageCount)
```


检查此过滤器页面范围是否包含给定页面。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | pageIndex | int | 页面索引（基于0） |
|
|  | pageCount | int | 总页面计数 |
|

**Returns:**
boolean - 如果此过滤范围包含页面，则为 true

