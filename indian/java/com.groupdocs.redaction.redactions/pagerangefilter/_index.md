---
title: "PageRangeFilter"
second_title: "GroupDocs.Redaction के लिए Java API Reference"
description: "दस्तावेज़ के भीतर पृष्ठ रेंज सेट करने वाले रेडैक्शन फ़िल्टर को दर्शाता है, जिससे रेडैक्शन लागू किया जाता है।"
type: docs
weight: 24
url: /hi/java/com.groupdocs.redaction.redactions/pagerangefilter/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.redaction.redactions.RedactionFilter](../../com.groupdocs.redaction.redactions/redactionfilter)
```
public class PageRangeFilter extends RedactionFilter
```

रिडैक्शन फ़िल्टर का प्रतिनिधित्व करता है, जो दस्तावेज़ के भीतर पृष्ठ रेंज निर्धारित करता है जहाँ रिडैक्शन लागू किया जाता है।

*** ** * ** ***


**Learn more**

* More details about applying redactions: [Redaction basics](../https://docs.groupdocs.com/redaction/java/redaction-basics/)
* More details about redaction filters: [Use PDF redaction filters](../https://docs.groupdocs.com/redaction/java/use-pdf-redaction-filters/)

<br />


## कन्स्ट्रक्टर

| कन्स्ट्रक्टर | विवरण |
| --- | --- |
|  | [PageRangeFilter(PageSeekOrigin origin, int index, int count)](#PageRangeFilter-com.groupdocs.redaction.redactions.PageSeekOrigin-int-int-) | RemovePageRedaction क्लास का एक नया इंस्टेंस इनिशियलाइज़ करता है। |
|
## विधियाँ

| विधि | विवरण |
| --- | --- |
|  | [getOrigin()](#getOrigin--) | सीक रेफ़रेंस पोज़िशन प्राप्त करता है, जो दस्तावेज़ की शुरुआत या अंत होता है। |
|
|  | [getIndex()](#getIndex--) | स्टार्ट पोज़िशन इंडेक्स प्राप्त करता है (0-आधारित)। |
|
|  | [getCount()](#getCount--) | हटाने के लिए पृष्ठों की संख्या प्राप्त करता है। |
|
|  | [isPageInRange(int pageIndex, int pageCount)](#isPageInRange-int-int-) | जाँचता है कि यह फ़िल्टर पेज रेंज दिए गए पेज को शामिल करता है या नहीं। |
|
### PageRangeFilter(PageSeekOrigin origin, int index, int count) {#PageRangeFilter-com.groupdocs.redaction.redactions.PageSeekOrigin-int-int-}
```
public PageRangeFilter(PageSeekOrigin origin, int index, int count)
```


RemovePageRedaction क्लास का एक नया इंस्टेंस इनिशियलाइज़ करता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | origin | [PageSeekOrigin](../../com.groupdocs.redaction.redactions/pageseekorigin) | सीक रेफ़रेंस पोज़िशन, दस्तावेज़ की शुरुआत या अंत |
|
|  | इंडेक्स | int | स्टार्ट पोज़िशन इंडेक्स (0-आधारित) |
|
|  | गिनती | int | हटाने के लिए पृष्ठों की संख्या |
|

### getOrigin() {#getOrigin--}
```
public final PageSeekOrigin getOrigin()
```


सीक रेफ़रेंस पोज़िशन प्राप्त करता है, जो दस्तावेज़ की शुरुआत या अंत होता है।


**Returns:**
[PageSeekOrigin](../../com.groupdocs.redaction.redactions/pageseekorigin) - Seek reference position, the beginning or the end of a document.

### getIndex() {#getIndex--}
```
public final int getIndex()
```


स्टार्ट पोज़िशन इंडेक्स प्राप्त करता है (0-आधारित)।


**Returns:**
int - शुरूआती स्थिति सूचकांक (0-आधारित).

### getCount() {#getCount--}
```
public final int getCount()
```


हटाने के लिए पृष्ठों की संख्या प्राप्त करता है।


**Returns:**
int - हटाने के लिए पृष्ठों की संख्या।

### isPageInRange(int pageIndex, int pageCount) {#isPageInRange-int-int-}
```
public final boolean isPageInRange(int pageIndex, int pageCount)
```


जाँचता है कि यह फ़िल्टर पेज रेंज दिए गए पेज को शामिल करता है या नहीं।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | pageIndex | int | पृष्ठ का सूचकांक (शून्य-आधारित) |
|
|  | pageCount | int | कुल पृष्ठों की संख्या |
|

**Returns:**
boolean - true, यदि यह फ़िल्टर रेंज पृष्ठ शामिल करती है

