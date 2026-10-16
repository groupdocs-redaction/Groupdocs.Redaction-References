---
title: "PageAreaFilter"
second_title: "GroupDocs.Redaction for Java API 参考"
description: "表示在文档页面内设置区域以进行编辑的过滤器。"
type: docs
weight: 22
url: /zh/java/com.groupdocs.redaction.redactions/pageareafilter/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.redaction.redactions.RedactionFilter](../../com.groupdocs.redaction.redactions/redactionfilter)
```
public class PageAreaFilter extends RedactionFilter
```

表示编辑过滤器，设置文档页面内的区域以应用编辑。

*** ** * ** ***


**Learn more**

* More details about applying redactions: [Redaction basics](../https://docs.groupdocs.com/redaction/java/redaction-basics/)
* More details about redaction filters: [Use PDF redaction filters](../https://docs.groupdocs.com/redaction/java/use-pdf-redaction-filters/)

<br />


## 构造函数

| 构造函数 | 描述 |
| --- | --- |
|  | [PageAreaFilter(Point topLeft, Dimension size)](#PageAreaFilter-java.awt.Point-java.awt.Dimension-) | 初始化 PageAreaFilter 类的新实例，以编辑特定区域。 |
|
## 方法

| 方法 | 描述 |
| --- | --- |
|  | [getRectangle()](#getRectangle--) | 获取页面上矩形（区域的左上位置和大小）。 |
|
|  | [isInTheArea(Rectangle rectangle)](#isInTheArea-java.awt.Rectangle-) | 检查此过滤区域是否与给定矩形相交。 |
|
### PageAreaFilter(Point topLeft, Dimension size) {#PageAreaFilter-java.awt.Point-java.awt.Dimension-}
```
public PageAreaFilter(Point topLeft, Dimension size)
```


初始化 PageAreaFilter 类的新实例，以编辑特定区域。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | topLeft | java.awt.Point | 左上区域坐标 |
|
|  | 大小 | java.awt.Dimension | 区域大小和颜色 |
|

### getRectangle() {#getRectangle--}
```
public final Rectangle getRectangle()
```


获取页面上矩形（区域的左上位置和大小）。


**Returns:**
java.awt.Rectangle - 页面上矩形（区域的左上位置和大小）。

### isInTheArea(Rectangle rectangle) {#isInTheArea-java.awt.Rectangle-}
```
public final boolean isInTheArea(Rectangle rectangle)
```


检查此过滤区域是否与给定矩形相交。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | rectangle | java.awt.Rectangle | 要检查的矩形 |
|

**Returns:**
boolean - 如果此过滤区域相交，则为 true

