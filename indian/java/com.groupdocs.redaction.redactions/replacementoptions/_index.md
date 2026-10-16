---
title: "ReplacementOptions"
second_title: "GroupDocs.Redaction के लिए Java API Reference"
description: "मिलाए गए टेक्स्ट प्रतिस्थापन के विकल्पों का प्रतिनिधित्व करता है।"
type: docs
weight: 31
url: /hi/java/com.groupdocs.redaction.redactions/replacementoptions/
---
**Inheritance:**
java.lang.Object
```
public class ReplacementOptions
```

मिलाए गए टेक्स्ट प्रतिस्थापन के विकल्पों का प्रतिनिधित्व करता है।

*** ** * ** ***


**Learn more**

* More details about document text redactions: [Text redactions](../https://docs.groupdocs.com/redaction/java/text-redactions/)
* More details about redaction filters: [Use PDF redaction filters](../https://docs.groupdocs.com/redaction/java/use-pdf-redaction-filters/)

<br />


## कन्स्ट्रक्टर

| कन्स्ट्रक्टर | विवरण |
| --- | --- |
|  | [ReplacementOptions(String replacement)](#ReplacementOptions-java.lang.String-) | ReplacementOptions क्लास का नया इंस्टेंस प्रारंभ करता है जिसमें प्रतिस्थापन पाठ विकल्प के रूप में होता है। |
|
|  | [ReplacementOptions(Color color)](#ReplacementOptions-java.awt.Color-) | ReplacementOptions क्लास का नया इंस्टेंस प्रारंभ करता है जिसमें रंगीन आयत विकल्प के रूप में होती है। |
|
## विधियाँ

| विधि | विवरण |
| --- | --- |
|  | [getActionType()](#getActionType--) | प्रतिस्थापन कार्रवाई प्राप्त करता है: बॉक्स बनाएं या पाठ को प्रतिस्थापित करें। |
|
|  | [getReplacement()](#getReplacement--) | पाठ्य प्रतिस्थापन मान प्राप्त करता है। |
|
|  | [setReplacement(String value)](#setReplacement-java.lang.String-) | पाठ्य प्रतिस्थापन मान सेट करता है। |
|
|  | [getBoxColor()](#getBoxColor--) | एक के लिए रंग प्राप्त करता है। |
ReplacementType.DrawBox
विकल्प (अन्यथा अनदेखा किया जाता है)।
|
|  | [setBoxColor(Color value)](#setBoxColor-java.awt.Color-) | एक के लिए रंग सेट करता है |
ReplacementType.DrawBox
विकल्प (अन्यथा अनदेखा किया जाता है)।
|
|  | [getFilters()](#getFilters--) | इस रेडैक्शन के साथ लागू करने के लिए फ़िल्टरों की एक सरणी प्राप्त करता है। |
|
|  | [setFilters(RedactionFilter[] value)](#setFilters-com.groupdocs.redaction.redactions.RedactionFilter---) | इस रेडैक्शन के साथ लागू करने के लिए फ़िल्टरों की एक सरणी सेट करता है। |
|
|  | [getCustomRedaction()](#getCustomRedaction--) | एक कस्टम रेडैक्शन हैंडलर प्राप्त करता है। |
|
|  | [setCustomRedaction(ICustomRedactionHandler value)](#setCustomRedaction-com.groupdocs.redaction.redactions.ICustomRedactionHandler-) | एक कस्टम रेडैक्शन हैंडलर सेट करता है। |
|
| [fromFilters(RedactionFilter[] filters)](#fromFilters-com.groupdocs.redaction.redactions.RedactionFilter---) |  |
### ReplacementOptions(String replacement) {#ReplacementOptions-java.lang.String-}
```
public ReplacementOptions(String replacement)
```


ReplacementOptions क्लास का नया इंस्टेंस प्रारंभ करता है जिसमें प्रतिस्थापन पाठ विकल्प के रूप में होता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | प्रतिस्थापन | java.lang.String | पाठ्य प्रतिस्थापन |
|

### ReplacementOptions(Color color) {#ReplacementOptions-java.awt.Color-}
```
public ReplacementOptions(Color color)
```


ReplacementOptions क्लास का नया इंस्टेंस प्रारंभ करता है जिसमें रंगीन आयत विकल्प के रूप में होती है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | रंग | java.awt.Color | आयत का रंग |
|

### getActionType() {#getActionType--}
```
public final ReplacementType getActionType()
```


प्रतिस्थापन कार्रवाई प्राप्त करता है: बॉक्स बनाएं या पाठ को प्रतिस्थापित करें।


**Returns:**
[ReplacementType](../../com.groupdocs.redaction.redactions/replacementtype) - The replacement action: draw box or replace text.

### getReplacement() {#getReplacement--}
```
public final String getReplacement()
```


पाठ्य प्रतिस्थापन मान प्राप्त करता है।


**Returns:**
java.lang.String - पाठ्य प्रतिस्थापन मान।

### setReplacement(String value) {#setReplacement-java.lang.String-}
```
public final void setReplacement(String value)
```


पाठ्य प्रतिस्थापन मान सेट करता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | मान | java.lang.String | पाठ्य प्रतिस्थापन मान। |
|

### getBoxColor() {#getBoxColor--}
```
public final Color getBoxColor()
```


एक के लिए रंग प्राप्त करता है।
ReplacementType.DrawBox
विकल्प (अन्यथा अनदेखा किया जाता है)।


**Returns:**
java.awt.Color - ReplacementType.DrawBox विकल्प के लिए रंग (अन्यथा अनदेखा किया जाता है)।

### setBoxColor(Color value) {#setBoxColor-java.awt.Color-}
```
public final void setBoxColor(Color value)
```


एक के लिए रंग सेट करता है
ReplacementType.DrawBox
विकल्प (अन्यथा अनदेखा किया जाता है)।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | मान | java.awt.Color | ReplacementType.DrawBox विकल्प के लिए रंग (अन्यथा अनदेखा किया जाता है)। |
|

### getFilters() {#getFilters--}
```
public final RedactionFilter[] getFilters()
```


इस रेडैक्शन के साथ लागू करने के लिए फ़िल्टरों की एक सरणी प्राप्त करता है।


**Returns:**
com.groupdocs.redaction.redactions.RedactionFilter[] - इस रेडैक्शन के साथ लागू करने के लिए फ़िल्टरों की एक सरणी।

### setFilters(RedactionFilter[] value) {#setFilters-com.groupdocs.redaction.redactions.RedactionFilter---}
```
public final void setFilters(RedactionFilter[] value)
```


इस रेडैक्शन के साथ लागू करने के लिए फ़िल्टरों की एक सरणी सेट करता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | value | [RedactionFilter\[\]](../../com.groupdocs.redaction.redactions/redactionfilter) | इस रेडैक्शन के साथ लागू करने के लिए फ़िल्टरों की एक सरणी। |
|

### getCustomRedaction() {#getCustomRedaction--}
```
public final ICustomRedactionHandler getCustomRedaction()
```


एक कस्टम रेडैक्शन हैंडलर प्राप्त करता है। केवल PDF [PageAreaRedaction](../../com.groupdocs.redaction.redactions/pagearearedaction) के लिए समर्थित।


**Returns:**
[ICustomRedactionHandler](../../com.groupdocs.redaction.redactions/icustomredactionhandler) - An instance of [ICustomRedactionHandler](../../com.groupdocs.redaction.redactions/icustomredactionhandler), or  null  if not set.

### setCustomRedaction(ICustomRedactionHandler value) {#setCustomRedaction-com.groupdocs.redaction.redactions.ICustomRedactionHandler-}
```
public final void setCustomRedaction(ICustomRedactionHandler value)
```


एक कस्टम रेडैक्शन हैंडलर सेट करता है। केवल PDF [PageAreaRedaction](../../com.groupdocs.redaction.redactions/pagearearedaction) के लिए समर्थित।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | value | [ICustomRedactionHandler](../../com.groupdocs.redaction.redactions/icustomredactionhandler) | एक उदाहरण [ICustomRedactionHandler](../../com.groupdocs.redaction.redactions/icustomredactionhandler) का। |
|

### fromFilters(RedactionFilter[] filters) {#fromFilters-com.groupdocs.redaction.redactions.RedactionFilter---}
```
public static ReplacementOptions fromFilters(RedactionFilter[] filters)
```




**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| filters | [RedactionFilter\[\]](../../com.groupdocs.redaction.redactions/redactionfilter) |  |

**Returns:**
[ReplacementOptions](../../com.groupdocs.redaction.redactions/replacementoptions)
