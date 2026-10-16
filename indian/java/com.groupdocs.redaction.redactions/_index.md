---
title: "com.groupdocs.redaction.redactions"
second_title: "GroupDocs.Redaction के लिए Java API Reference"
description: "पैकेज विभिन्न प्रकार के रेडैक्शन के लिए क्लास प्रदान करता है।"
type: docs
weight: 16
url: /hi/java/com.groupdocs.redaction.redactions/
---

पैकेज विभिन्न प्रकार के रेडैक्शन के लिए क्लास प्रदान करता है।



## क्लासेस

| क्लास | विवरण |
| --- | --- |
| [AnnotationRedaction](../com.groupdocs.redaction.redactions/annotationredaction) | एक रेडैक्शन को दर्शाता है जो दिए गए रेगुलर एक्सप्रेशन से मेल खाने वाले एनोटेशन टेक्स्ट (टिप्पणियाँ, आदि) को बदलता है। |
| [CellColumnRedaction](../com.groupdocs.redaction.redactions/cellcolumnredaction) | एक टेक्स्ट रेडैक्शन को दर्शाता है जो स्प्रेडशीट दस्तावेज़ों (CSV, Excel, आदि) में टेक्स्ट को बदलता है। |
| [CellFilter](../com.groupdocs.redaction.redactions/cellfilter) | CellColumnRedaction की सीमा को एक वर्कशीट और एक कॉलम तक सीमित करने का विकल्प प्रदान करता है। |
| [CustomRedactionContext](../com.groupdocs.redaction.redactions/customredactioncontext) | [ICustomRedactionHandler](../com.groupdocs.redaction.redactions/icustomredactionhandler) के लिए इनपुट डेटा प्रदान करता है। |
| [CustomRedactionResult](../com.groupdocs.redaction.redactions/customredactionresult) | [ICustomRedactionHandler](../com.groupdocs.redaction.redactions/icustomredactionhandler) द्वारा लौटाए गए परिणाम को दर्शाता है। |
| [DeleteAnnotationRedaction](../com.groupdocs.redaction.redactions/deleteannotationredaction) | एक टेक्स्ट रेडैक्शन को दर्शाता है जो यदि टेक्स्ट दिए गए रेगुलर एक्सप्रेशन से मेल खाता है तो एनोटेशन को हटाता है (वैकल्पिक रूप से सभी एनोटेशन हटाता है)। |
| [EraseMetadataRedaction](../com.groupdocs.redaction.redactions/erasemetadataredaction) | एक मेटाडाटा रेडैक्शन को दर्शाता है जो दस्तावेज़ से सभी मेटाडाटा या विशिष्ट MetadataFilters से मेल खाने वाले मेटाडाटा को मिटा देता है। |
| [ExactPhraseRedaction](../com.groupdocs.redaction.redactions/exactphraseredaction) | एक टेक्स्ट रेडैक्शन को दर्शाता है जो दस्तावेज़ के टेक्स्ट में सटीक वाक्यांश को बदलता है, डिफ़ॉल्ट रूप से केस-इंसेंसिटिव। |
| [ImageAreaRedaction](../com.groupdocs.redaction.redactions/imagearearedaction) | एक रेडैक्शन को दर्शाता है जो इमेज दस्तावेज़ के दिए गए क्षेत्र में रंगीन आयत रखता है। |
| [MetadataFilters](../com.groupdocs.redaction.redactions/metadatafilters) | दस्तावेज़ मेटाडाटा के सबसे सामान्य प्रकारों की सूची को दर्शाता है। |
| [MetadataRedaction](../com.groupdocs.redaction.redactions/metadataredaction) | दस्तावेज़ मेटाडेटा रिडैक्शन के लिए एक बेस एब्स्ट्रैक्ट क्लास का प्रतिनिधित्व करता है। |
| [MetadataSearchRedaction](../com.groupdocs.redaction.redactions/metadatasearchredaction) | रेगुलर एक्सप्रेशन का उपयोग करके कुंजियों और/या मानों को मिलाते हुए मेटाडेटा खोजता और रिडैक्ट करता है, ऐसी मेटाडेटा रिडैक्शन का प्रतिनिधित्व करता है। |
| [PageAreaFilter](../com.groupdocs.redaction.redactions/pageareafilter) | रिडैक्शन फ़िल्टर का प्रतिनिधित्व करता है, जो दस्तावेज़ के पृष्ठ के भीतर एक क्षेत्र निर्धारित करता है जहाँ रिडैक्शन लागू किया जाता है। |
| [PageAreaRedaction](../com.groupdocs.redaction.redactions/pagearearedaction) | पृष्ठ के एक क्षेत्र में टेक्स्ट, इमेज और एनोटेशन को प्रभावित करने वाली जटिल टेक्स्टुअल रिडैक्शन का प्रतिनिधित्व करता है। |
| [PageRangeFilter](../com.groupdocs.redaction.redactions/pagerangefilter) | रिडैक्शन फ़िल्टर का प्रतिनिधित्व करता है, जो दस्तावेज़ के भीतर पृष्ठ रेंज निर्धारित करता है जहाँ रिडैक्शन लागू किया जाता है। |
| [RedactionDescription](../com.groupdocs.redaction.redactions/redactiondescription) | रिडैक्शन प्रक्रिया के दौरान किए गए एकल परिवर्तन कार्रवाई जानकारी का प्रतिनिधित्व करता है। |
| [RedactionFilter](../com.groupdocs.redaction.redactions/redactionfilter) | रिडैक्शन फ़िल्टर का प्रतिनिधित्व करता है, जो दस्तावेज़ के भीतर स्कोप निर्धारित करता है जहाँ रिडैक्शन लागू किया जाता है। |
| [RedactionType](../com.groupdocs.redaction.redactions/redactiontype) | रिडैक्शन द्वारा प्रभावित दस्तावेज़ डेटा के प्रकार का प्रतिनिधित्व करता है। |
| [RegexRedaction](../com.groupdocs.redaction.redactions/regexredaction) | प्रदान किए गए रेगुलर एक्सप्रेशन से मिलाते हुए दस्तावेज़ में टेक्स्ट खोजता और बदलता है, ऐसी टेक्स्ट रिडैक्शन का प्रतिनिधित्व करता है। |
| [RegionReplacementOptions](../com.groupdocs.redaction.redactions/regionreplacementoptions) | इमेज रीजन प्रतिस्थापन के लिए रंग और क्षेत्र पैरामीटर का प्रतिनिधित्व करता है। |
| [RemovePageRedaction](../com.groupdocs.redaction.redactions/removepageredaction) | दस्तावेज़ से एक पृष्ठ (स्लाइड, वर्कशीट आदि) हटाने वाली रिडैक्शन का प्रतिनिधित्व करता है। |
| [ReplacementOptions](../com.groupdocs.redaction.redactions/replacementoptions) | मिलाए गए टेक्स्ट प्रतिस्थापन के विकल्पों का प्रतिनिधित्व करता है। |
| [TextRedaction](../com.groupdocs.redaction.redactions/textredaction) | दस्तावेज़ टेक्स्ट रिडैक्शन के लिए एक बेस एब्स्ट्रैक्ट क्लास का प्रतिनिधित्व करता है। |
| [TextReplacement](../com.groupdocs.redaction.redactions/textreplacement) | टेक्स्टुअल प्रतिस्थापन जानकारी का प्रतिनिधित्व करता है। |

## इंटरफ़ेस

| इंटरफ़ेस | विवरण |
| --- | --- |
| [ICustomRedactionHandler](../com.groupdocs.redaction.redactions/icustomredactionhandler) | एक कस्टम रिडैक्शन कॉलबैक को परिभाषित करता है। |
| [IRedactionCallback](../com.groupdocs.redaction.redactions/iredactioncallback) | प्रत्येक रिडैक्शन परिवर्तन पर जानकारी प्राप्त करने और वैकल्पिक रूप से उसे रोकने के लिए आवश्यक मेथड्स को परिभाषित करता है। |

## एन्यूमरेशन

| एन्यूम | विवरण |
| --- | --- |
| [PageSeekOrigin](../com.groupdocs.redaction.redactions/pageseekorigin) | दस्तावेज़ में खोज के लिए रेफ़रेंस पॉइंट्स का प्रतिनिधित्व करने वाले फ़ील्ड्स प्रदान करता है। |
| [RedactionActionType](../com.groupdocs.redaction.redactions/redactionactiontype) | रिडैक्शन करने के लिए ली जा सकने वाली कार्रवाइयों का प्रतिनिधित्व करता है। |
| [ReplacementType](../com.groupdocs.redaction.redactions/replacementtype) | मिलाए गए टेक्स्ट के लिए प्रतिस्थापन के प्रकार का प्रतिनिधित्व करता है। |
