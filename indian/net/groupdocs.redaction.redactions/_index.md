---
title: GroupDocs.Redaction.Redactions
second_title: .NET API संदर्भ के लिए GroupDocs.Redaction
description: दRedactions नेमस्पेस वभन्न प्रकर के संपदन के लए कक्षएं प्रदन करत है
type: docs
weight: 70
url: /hi/net/groupdocs.redaction.redactions/
---
दRedactions नेमस्पेस विभिन्न प्रकार के संपादन के लिए कक्षाएं प्रदान करता है।

## कक्षाओं

| कक्षा | विवरण |
| --- | --- |
| [AnnotationRedaction](./annotationredaction) | एक सुधार का प्रतिनिधित्व करता है जो किसी दिए गए नियमित अभिव्यक्ति से मेल खाने वाले एनोटेशन टेक्स्ट (टिप्पणियां, आदि) को प्रतिस्थापित करता है। |
| [CellColumnRedaction](./cellcolumnredaction) | एक टेक्स्ट रिडक्शन का प्रतिनिधित्व करता है जो टेक्स्ट को स्प्रेडशीट दस्तावेज़ों (CSV, Excel, आदि) में बदल देता है। |
| [CellFilter](./cellfilter) | के दायरे को सीमित करने के लिए एक विकल्प प्रदान करता है[`CellColumnRedaction`](../groupdocs.redaction.redactions/cellcolumnredaction) एक कार्यपत्रक और एक स्तंभ के लिए. |
| [DeleteAnnotationRedaction](./deleteannotationredaction) | एक टेक्स्ट रिडक्शन का प्रतिनिधित्व करता है जो एनोटेशन को हटा देता है यदि टेक्स्ट रेगुलर एक्सप्रेशन से मेल खाता है (वैकल्पिक रूप से सभी एनोटेशन हटा देता है)। |
| [EraseMetadataRedaction](./erasemetadataredaction) | एक मेटाडेटा रिडक्शन का प्रतिनिधित्व करता है जो दस्तावेज़ से विशिष्ट मेटाडेटा फ़िल्टर से मेल खाने वाले सभी मेटाडेटा या मेटाडेटा को मिटा देता है। |
| [ExactPhraseRedaction](./exactphraseredaction) | एक टेक्स्ट रिडक्शन का प्रतिनिधित्व करता है जो दस्तावेज़ के टेक्स्ट में सटीक वाक्यांश को बदल देता है, डिफ़ॉल्ट रूप से केस असंवेदनशील। |
| [ImageAreaRedaction](./imagearearedaction) | एक सुधार का प्रतिनिधित्व करता है जो एक छवि दस्तावेज़ के दिए गए क्षेत्र में रंगीन आयत रखता है। |
| [MetadataRedaction](./metadataredaction) | दस्तावेज़ मेटाडेटा संशोधनों के लिए आधार सार वर्ग का प्रतिनिधित्व करता है। |
| [MetadataSearchRedaction](./metadatasearchredaction) | एक मेटाडेटा रिडक्शन का प्रतिनिधित्व करता है जो रेगुलर एक्सप्रेशंस, मिलान कुंजियों और/या मानों का उपयोग करके मेटाडेटा को खोजता और संपादित करता है। |
| [RedactionDescription](./redactiondescription) | एक एकल परिवर्तन क्रिया जानकारी का प्रतिनिधित्व करता है जो संपादन प्रक्रिया के दौरान की जाती है। |
| [RegexRedaction](./regexredaction) | एक टेक्स्ट रिडक्शन का प्रतिनिधित्व करता है जो प्रदान की गई रेगुलर एक्सप्रेशन से मिलान करके दस्तावेज़ में टेक्स्ट को खोजता है और बदलता है। |
| [RegionReplacementOptions](./regionreplacementoptions) | छवि क्षेत्र प्रतिस्थापन के लिए रंग और क्षेत्र पैरामीटर का प्रतिनिधित्व करता है। देखना[`ImageAreaRedaction`](../groupdocs.redaction.redactions/imagearearedaction) . |
| [RemovePageRedaction](./removepageredaction) | एक संपादन का प्रतिनिधित्व करता है जो एक दस्तावेज़ से एक पृष्ठ (स्लाइड, वर्कशीट, आदि) को हटा देता है। |
| [ReplacementOptions](./replacementoptions) | मिलान किए गए पाठ प्रतिस्थापन के लिए विकल्पों का प्रतिनिधित्व करता है। |
| [TextRedaction](./textredaction) | दस्तावेज़ पाठ संपादन के लिए आधार सार वर्ग का प्रतिनिधित्व करता है। |
| [TextReplacement](./textreplacement) | एक पाठ्य प्रतिस्थापन जानकारी का प्रतिनिधित्व करता है। |
## इंटरफेस

| इंटरफेस | विवरण |
| --- | --- |
| [IRedactionCallback](./iredactioncallback) | उन विधियों को परिभाषित करता है जो प्रत्येक संपादन परिवर्तन पर जानकारी प्राप्त करने के लिए आवश्यक हैं और वैकल्पिक रूप से इसे रोकते हैं। |
## गणना

| गणना | विवरण |
| --- | --- |
| [MetadataFilters](./metadatafilters) | सबसे सामान्य प्रकार के दस्तावेज़ मेटाडेटा की सूची का प्रतिनिधित्व करता है। |
| [PageSeekOrigin](./pageseekorigin) | फ़ील्ड प्रदान करता है जो दस्तावेज़ में खोज के लिए संदर्भ बिंदुओं का प्रतिनिधित्व करता है। |
| [RedactionActionType](./redactionactiontype) | उन कार्रवाइयों का प्रतिनिधित्व करता है जिन्हें सुधार करने के लिए लिया जा सकता है। |
| [RedactionType](./redactiontype) | एक प्रकार के दस्तावेज़ के डेटा का प्रतिनिधित्व करता है, जो संपादन से प्रभावित होता है। |
| [ReplacementType](./replacementtype) | मिलान किए गए पाठ के लिए एक प्रकार के प्रतिस्थापन का प्रतिनिधित्व करता है। |

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Redaction.dll -->
