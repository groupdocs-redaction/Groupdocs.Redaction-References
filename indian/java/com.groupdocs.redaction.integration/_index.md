---
title: "com.groupdocs.redaction.integration"
second_title: "GroupDocs.Redaction के लिए Java API Reference"
description: "पैकेज विभिन्न फ़ॉर्मैट के दस्तावेज़ों को GroupDocs.Redactions के साथ इंटीग्रेट करने के लिए उपयोग किए जाने वाले इंटरफ़ेसेज़ और क्लासेज़ प्रदान करता है।"
type: docs
weight: 13
url: /hi/java/com.groupdocs.redaction.integration/
---

पैकेज इंटरफ़ेस और क्लास प्रदान करता है, जो विभिन्न फ़ॉर्मेट के दस्तावेज़ों को GroupDocs.Redactions के साथ एकीकृत करने के लिए उपयोग होते हैं।



## क्लासेस

| क्लास | विवरण |
| --- | --- |
| [DocumentFormatInstance](../com.groupdocs.redaction.integration/documentformatinstance) | दस्तावेज़ के एक विशिष्ट फ़ॉर्मैट का प्रतिनिधित्व करता है। |
| [MetadataCollection](../com.groupdocs.redaction.integration/metadatacollection) | MetadataItem की शब्दकोश को उसके शीर्षक को कुंजी के रूप में दर्शाता है। |
| [MetadataItem](../com.groupdocs.redaction.integration/metadataitem) | सभी समर्थित स्वरूपों के लिए सामान्य मेटाडेटा आइटम को दर्शाता है, जो मेटाडेटा रेडैक्शन में उपयोग किया जाता है। |
| [RecognizedImage](../com.groupdocs.redaction.integration/recognizedimage) | छवि से निकाले गए पाठ को, उसकी पहचान प्रक्रिया के परिणामस्वरूप दर्शाता है। |
| [RedactableImage](../com.groupdocs.redaction.integration/redactableimage) | सभी रास्टर इमेज रेडैक्शन ऑपरेशनों के लिए एक फ़ेसाड प्रदान करता है। |
| [TextFragment](../com.groupdocs.redaction.integration/textfragment) | OCR इंजन द्वारा निकाले गए पहचाने गए पाठ (शब्द, प्रतीक, आदि) का भाग दर्शाता है। |
| [TextLine](../com.groupdocs.redaction.integration/textline) | OCR इंजन द्वारा छवि से निकाली गई पाठ की पंक्ति को दर्शाता है। |

## इंटरफ़ेस

| इंटरफ़ेस | विवरण |
| --- | --- |
| [IAnnotatedDocument](../com.groupdocs.redaction.integration/iannotateddocument) | टिप्पणियों जैसी एनोटेशन तक पहुँच के लिए आवश्यक विधियों को परिभाषित करता है। |
| [ICellularFormatInstance](../com.groupdocs.redaction.integration/icellularformatinstance) | एक या कई शीट्स वाले स्प्रेडशीट स्वरूपों तक पहुँच के लिए आवश्यक विधियों को परिभाषित करता है। |
| [IFixedFormatDocument](../com.groupdocs.redaction.integration/ifixedformatdocument) | PDF या प्रेजेंटेशन जैसे स्थिर संरचना वाले स्वरूपों तक पहुँच के लिए आवश्यक विधियों को परिभाषित करता है। |
| [IImageFormatInstance](../com.groupdocs.redaction.integration/iimageformatinstance) | रास्टर इमेज स्वरूप रेडैक्शन के लिए आवश्यक विधियों को परिभाषित करता है। |
| [IMetadataAccess](../com.groupdocs.redaction.integration/imetadataaccess) | यदि स्वरूप समर्थन करता है तो दस्तावेज़ के मेटाडेटा तक पहुँच के लिए आवश्यक विधियों को परिभाषित करता है। |
| [IMultipleAreaRedactable](../com.groupdocs.redaction.integration/imultiplearearedactable) | एक ही रंग से कई इमेज क्षेत्रों को एक साथ रेडैक्ट करने के लिए आवश्यक विधियों को परिभाषित करता है। |
| [IOcrConnector](../com.groupdocs.redaction.integration/iocrconnector) | इमेज दस्तावेज़ों और एम्बेडेड इमेजेज़ पर टेक्स्टुअल रेडैक्शन लागू करने के लिए आवश्यक विधियों को परिभाषित करता है। |
| [IPaginatedDocument](../com.groupdocs.redaction.integration/ipaginateddocument) | दस्तावेज़ के पृष्ठों को संशोधित करने के लिए आवश्यक विधियों को परिभाषित करता है। |
| [IPreviewable](../com.groupdocs.redaction.integration/ipreviewable) | दस्तावेज़ का प्रीव्यू बनाने के लिए विधियों को परिभाषित करता है। |
| [IRasterizableDocument](../com.groupdocs.redaction.integration/irasterizabledocument) | किसी भी बाइनरी रूप में दस्तावेज़ को सहेजने के लिए आवश्यक विधियों को परिभाषित करता है। |
| [ITextualFormatInstance](../com.groupdocs.redaction.integration/itextualformatinstance) | पाठ युक्त किसी भी दस्तावेज़ में टेक्स्टुअल डेटा को रेडैक्ट करने के लिए आवश्यक विधियों को परिभाषित करता है। |
