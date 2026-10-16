---
title: "PreviewOptions"
second_title: "GroupDocs.Redaction के लिए Java API Reference"
description: "पूर्वावलोकन जनरेशन के लिए आवश्यकताओं और स्ट्रीम डेलीगेट सेट करने के विकल्प प्रदान करता है।"
type: docs
weight: 11
url: /hi/java/com.groupdocs.redaction.options/previewoptions/
---
**Inheritance:**
java.lang.Object
```
public class PreviewOptions
```

पूर्वावलोकन जनरेशन के लिए आवश्यकताओं और स्ट्रीम डेलीगेट सेट करने के विकल्प प्रदान करता है।

## कन्स्ट्रक्टर

| कन्स्ट्रक्टर | विवरण |
| --- | --- |
|  | [PreviewOptions(ICreatePageStream createPageStream)](#PreviewOptions-com.groupdocs.redaction.options.ICreatePageStream-) | PreviewOptions क्लास का एक नया उदाहरण प्रारंभ करता है, जिससे आउटपुट स्ट्रीम बंद हो जाता है। |
|
|  | [PreviewOptions(ICreatePageStream createPageStream, IReleasePageStream releasePageStream)](#PreviewOptions-com.groupdocs.redaction.options.ICreatePageStream-com.groupdocs.redaction.options.IReleasePageStream-) | PreviewOptions क्लास का एक नया उदाहरण प्रारंभ करता है, जिससे आउटपुट स्ट्रीम क्लाइंट को आगे उपयोग के लिए वापस किया जाता है। |
|
## विधियाँ

| विधि | विवरण |
| --- | --- |
|  | [getWidth()](#getWidth--) | पृष्ठ पूर्वावलोकन की चौड़ाई प्राप्त करता है या सेट करता है। |
|
|  | [setWidth(int value)](#setWidth-int-) | पृष्ठ पूर्वावलोकन की चौड़ाई प्राप्त करता है या सेट करता है। |
|
|  | [getHeight()](#getHeight--) | पृष्ठ पूर्वावलोकन की ऊँचाई प्राप्त करता है या सेट करता है। |
|
|  | [setHeight(int value)](#setHeight-int-) | पृष्ठ पूर्वावलोकन की ऊँचाई प्राप्त करता है या सेट करता है। |
|
|  | [getPageNumbers()](#getPageNumbers--) | पूर्वावलोकन बनाने के लिए पृष्ठ संख्याओं की एक सरणी प्राप्त करता है या सेट करता है। |
|
|  | [setPageNumbers(int[] value)](#setPageNumbers-int---) | पूर्वावलोकन बनाने के लिए पृष्ठ संख्याओं की एक सरणी प्राप्त करता है या सेट करता है। |
|
|  | [getPreviewFormat()](#getPreviewFormat--) | पूर्वावलोकन छवि प्रारूप प्राप्त करता है या सेट करता है। |
|
|  | [setPreviewFormat(PreviewFormats value)](#setPreviewFormat-com.groupdocs.redaction.options.PreviewFormats-) | पूर्वावलोकन छवि प्रारूप प्राप्त करता है या सेट करता है। |
|
|  | [getCreatePageStream()](#getCreatePageStream--) | पृष्ठ स्ट्रीम निर्माण प्रतिनिधि का एक उदाहरण प्राप्त करता है या सेट करता है। |
|
|  | [setCreatePageStream(ICreatePageStream value)](#setCreatePageStream-com.groupdocs.redaction.options.ICreatePageStream-) | पृष्ठ स्ट्रीम निर्माण प्रतिनिधि का एक उदाहरण प्राप्त करता है या सेट करता है। |
|
|  | [getReleasePageStream()](#getReleasePageStream--) | पृष्ठ पूर्वावलोकन पूर्णता प्रतिनिधि का एक उदाहरण प्राप्त करता है या सेट करता है। |
|
|  | [setReleasePageStream(IReleasePageStream value)](#setReleasePageStream-com.groupdocs.redaction.options.IReleasePageStream-) | पृष्ठ पूर्वावलोकन पूर्णता प्रतिनिधि का एक उदाहरण प्राप्त करता है या सेट करता है। |
|
### PreviewOptions(ICreatePageStream createPageStream) {#PreviewOptions-com.groupdocs.redaction.options.ICreatePageStream-}
```
public PreviewOptions(ICreatePageStream createPageStream)
```


PreviewOptions क्लास का एक नया उदाहरण प्रारंभ करता है, जिससे आउटपुट स्ट्रीम बंद हो जाता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | createPageStream | [ICreatePageStream](../../com.groupdocs.redaction.options/icreatepagestream) | एक विशिष्ट पृष्ठ पूर्वावलोकन के लिए स्ट्रीम बनाता है |
|

### PreviewOptions(ICreatePageStream createPageStream, IReleasePageStream releasePageStream) {#PreviewOptions-com.groupdocs.redaction.options.ICreatePageStream-com.groupdocs.redaction.options.IReleasePageStream-}
```
public PreviewOptions(ICreatePageStream createPageStream, IReleasePageStream releasePageStream)
```


PreviewOptions क्लास का एक नया उदाहरण प्रारंभ करता है, जिससे आउटपुट स्ट्रीम क्लाइंट को आगे उपयोग के लिए वापस किया जाता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | createPageStream | [ICreatePageStream](../../com.groupdocs.redaction.options/icreatepagestream) | एक विशिष्ट पृष्ठ पूर्वावलोकन के लिए स्ट्रीम बनाता है |
|
|  | releasePageStream | [IReleasePageStream](../../com.groupdocs.redaction.options/ireleasepagestream) | सूचित करता है कि पृष्ठ पूर्वावलोकन निर्माण समाप्त हो गया है और आउटपुट स्ट्रीम प्राप्त करता है |
|

### getWidth() {#getWidth--}
```
public final int getWidth()
```


पृष्ठ पूर्वावलोकन की चौड़ाई प्राप्त करता है या सेट करता है।


**Returns:**
int - पृष्ठ पूर्वावलोकन की चौड़ाई।

### setWidth(int value) {#setWidth-int-}
```
public final void setWidth(int value)
```


पृष्ठ पूर्वावलोकन की चौड़ाई प्राप्त करता है या सेट करता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | मान | int | पृष्ठ पूर्वावलोकन की चौड़ाई। |
|

### getHeight() {#getHeight--}
```
public final int getHeight()
```


पृष्ठ पूर्वावलोकन की ऊँचाई प्राप्त करता है या सेट करता है।


**Returns:**
int - पृष्ठ पूर्वावलोकन की ऊँचाई।

### setHeight(int value) {#setHeight-int-}
```
public final void setHeight(int value)
```


पृष्ठ पूर्वावलोकन की ऊँचाई प्राप्त करता है या सेट करता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | मान | int | पृष्ठ पूर्वावलोकन की ऊँचाई। |
|

### getPageNumbers() {#getPageNumbers--}
```
public final int[] getPageNumbers()
```


पूर्वावलोकन बनाने के लिए पृष्ठ संख्याओं की एक सरणी प्राप्त करता है या सेट करता है।


**Returns:**
int[] - पूर्वावलोकन बनाने के लिए पृष्ठ संख्याओं की एक सरणी।

### setPageNumbers(int[] value) {#setPageNumbers-int---}
```
public final void setPageNumbers(int[] value)
```


पूर्वावलोकन बनाने के लिए पृष्ठ संख्याओं की एक सरणी प्राप्त करता है या सेट करता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | मान | int[] | पूर्वावलोकन बनाने के लिए पृष्ठ संख्याओं की एक सरणी। |
|

### getPreviewFormat() {#getPreviewFormat--}
```
public final PreviewFormats getPreviewFormat()
```


पूर्वावलोकन छवि प्रारूप प्राप्त करता है या सेट करता है।


**Returns:**
[PreviewFormats](../../com.groupdocs.redaction.options/previewformats) - Preview image format.

### setPreviewFormat(PreviewFormats value) {#setPreviewFormat-com.groupdocs.redaction.options.PreviewFormats-}
```
public final void setPreviewFormat(PreviewFormats value)
```


पूर्वावलोकन छवि प्रारूप प्राप्त करता है या सेट करता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | value | [PreviewFormats](../../com.groupdocs.redaction.options/previewformats) | पूर्वावलोकन छवि प्रारूप। |
|

### getCreatePageStream() {#getCreatePageStream--}
```
public final ICreatePageStream getCreatePageStream()
```


पृष्ठ स्ट्रीम निर्माण प्रतिनिधि का एक उदाहरण प्राप्त करता है या सेट करता है।


**Returns:**
[ICreatePageStream](../../com.groupdocs.redaction.options/icreatepagestream) - An instance of page stream creation delegate.

### setCreatePageStream(ICreatePageStream value) {#setCreatePageStream-com.groupdocs.redaction.options.ICreatePageStream-}
```
public final void setCreatePageStream(ICreatePageStream value)
```


पृष्ठ स्ट्रीम निर्माण प्रतिनिधि का एक उदाहरण प्राप्त करता है या सेट करता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | value | [ICreatePageStream](../../com.groupdocs.redaction.options/icreatepagestream) | पृष्ठ स्ट्रीम निर्माण प्रतिनिधि का एक उदाहरण। |
|

### getReleasePageStream() {#getReleasePageStream--}
```
public final IReleasePageStream getReleasePageStream()
```


पृष्ठ पूर्वावलोकन पूर्णता प्रतिनिधि का एक उदाहरण प्राप्त करता है या सेट करता है।


**Returns:**
[IReleasePageStream](../../com.groupdocs.redaction.options/ireleasepagestream) - An instance of page preview completion delegate.

### setReleasePageStream(IReleasePageStream value) {#setReleasePageStream-com.groupdocs.redaction.options.IReleasePageStream-}
```
public final void setReleasePageStream(IReleasePageStream value)
```


पृष्ठ पूर्वावलोकन पूर्णता प्रतिनिधि का एक उदाहरण प्राप्त करता है या सेट करता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | value | [IReleasePageStream](../../com.groupdocs.redaction.options/ireleasepagestream) | पृष्ठ पूर्वावलोकन पूर्णता प्रतिनिधि का एक उदाहरण। |
|

