---
title: FileType
second_title: .NET API संदर्भ के लिए GroupDocs.Redaction
description: फ़इल प्रकर क प्रतनधत्व करत है GroupDocs.Redaction द्वर समर्थत सभ फ़इल प्रकरं क सूच प्रप्त करने के तरके प्रदन करत है एक्सटेंशन द्वर फ़इल प्रकर क पत लगत है आद
type: docs
weight: 90
url: /hi/net/groupdocs.redaction/filetype/
---
## FileType class

फ़ाइल प्रकार का प्रतिनिधित्व करता है। GroupDocs.Redaction द्वारा समर्थित सभी फ़ाइल प्रकारों की सूची प्राप्त करने के तरीके प्रदान करता है, एक्सटेंशन द्वारा फ़ाइल प्रकार का पता लगाता है, आदि

```csharp
public sealed class FileType : IEquatable<FileType>
```

## गुण

| नाम | विवरण |
| --- | --- |
| static [BMP](../../groupdocs.redaction/filetype/bmp) { get; } | बिटमैप छवि फ़ाइल (.bmp) |
| static [CSV](../../groupdocs.redaction/filetype/csv) { get; } | कॉमा सेपरेटेड वैल्यू फ़ाइल (.csv) |
| static [DOC](../../groupdocs.redaction/filetype/doc) { get; } | माइक्रोसॉफ्ट वर्ड दस्तावेज़ (.doc) |
| static [DOCM](../../groupdocs.redaction/filetype/docm) { get; } | वर्ड ओपन एक्सएमएल मैक्रो-सक्षम दस्तावेज़ (.docm) |
| static [DOCX](../../groupdocs.redaction/filetype/docx) { get; } | माइक्रोसॉफ्ट वर्ड ओपन एक्सएमएल दस्तावेज़ (.docx) |
| static [DOT](../../groupdocs.redaction/filetype/dot) { get; } | वर्ड दस्तावेज़ टेम्पलेट (.डॉट) |
| static [DOTM](../../groupdocs.redaction/filetype/dotm) { get; } | वर्ड ओपन एक्सएमएल मैक्रो-सक्षम दस्तावेज़ टेम्पलेट (.dotm) |
| static [DOTX](../../groupdocs.redaction/filetype/dotx) { get; } | वर्ड ओपन एक्सएमएल दस्तावेज़ टेम्पलेट (.dotx) |
| static [GIF](../../groupdocs.redaction/filetype/gif) { get; } | ग्राफ़िकल इंटरचेंज फ़ॉर्मेट फ़ाइल (.gif) |
| static [HTM](../../groupdocs.redaction/filetype/htm) { get; } | हाइपरटेक्स्ट मार्कअप भाषा फ़ाइल (.htm) |
| static [HTML](../../groupdocs.redaction/filetype/html) { get; } | हाइपरटेक्स्ट मार्कअप भाषा फ़ाइल (.html) |
| static [JP2](../../groupdocs.redaction/filetype/jp2) { get; } | JPEG 2000 कोर इमेज फ़ाइल (.jp2) |
| static [JPEG](../../groupdocs.redaction/filetype/jpeg) { get; } | JPEG इमेज (.jpeg) |
| static [JPG](../../groupdocs.redaction/filetype/jpg) { get; } | JPEG इमेज (.jpg) |
| static [MD](../../groupdocs.redaction/filetype/md) { get; } | मार्कडाउन दस्तावेज़ फ़ाइल (.md) |
| static [NUMBERS](../../groupdocs.redaction/filetype/numbers) { get; } | Apple नंबर स्प्रेडशीट (.नंबर) |
| static [ODP](../../groupdocs.redaction/filetype/odp) { get; } | OpenDocument प्रस्तुति (.odp) |
| static [ODS](../../groupdocs.redaction/filetype/ods) { get; } | OpenDocument स्प्रेडशीट (.ods) |
| static [ODT](../../groupdocs.redaction/filetype/odt) { get; } | OpenDocument टेक्स्ट दस्तावेज़ (.odt) |
| static [OTS](../../groupdocs.redaction/filetype/ots) { get; } | OpenDocument स्प्रेडशीट टेम्पलेट (.ots) |
| static [OTT](../../groupdocs.redaction/filetype/ott) { get; } | OpenDocument दस्तावेज़ टेम्पलेट (.ott) |
| static [PDF](../../groupdocs.redaction/filetype/pdf) { get; } | पोर्टेबल दस्तावेज़ स्वरूप फ़ाइल (.pdf) |
| static [PNG](../../groupdocs.redaction/filetype/png) { get; } | पोर्टेबल नेटवर्क ग्राफ़िक (.png) |
| static [PPT](../../groupdocs.redaction/filetype/ppt) { get; } | पॉवरपॉइंट प्रस्तुति (.पीपीटी) |
| static [PPTX](../../groupdocs.redaction/filetype/pptx) { get; } | PowerPoint ओपन XML प्रस्तुति (.pptx) |
| static [RTF](../../groupdocs.redaction/filetype/rtf) { get; } | रिच टेक्स्ट फ़ॉर्मेट फ़ाइल (.rtf) |
| static [TIF](../../groupdocs.redaction/filetype/tif) { get; } | टैग की गई छवि फ़ाइल (.tif) |
| static [TIFF](../../groupdocs.redaction/filetype/tiff) { get; } | टैग की गई छवि फ़ाइल प्रारूप (.tiff) |
| static [TSV](../../groupdocs.redaction/filetype/tsv) { get; } | टैब सेपरेटेड वैल्यू फ़ाइल (.tsv) |
| static [TXT](../../groupdocs.redaction/filetype/txt) { get; } | सादा पाठ फ़ाइल (.txt) |
| static [Unknown](../../groupdocs.redaction/filetype/unknown) { get; } | अज्ञात फ़ाइल प्रकार का प्रतिनिधित्व करता है। |
| static [XLS](../../groupdocs.redaction/filetype/xls) { get; } | एक्सेल स्प्रेडशीट (.xls) |
| static [XLSB](../../groupdocs.redaction/filetype/xlsb) { get; } | एक्सेल बाइनरी स्प्रेडशीट (.xlsb) |
| static [XLSM](../../groupdocs.redaction/filetype/xlsm) { get; } | एक्सेल ओपन एक्सएमएल मैक्रो-सक्षम स्प्रेडशीट (.xlsm) |
| static [XLSX](../../groupdocs.redaction/filetype/xlsx) { get; } | माइक्रोसॉफ्ट एक्सेल ओपन एक्सएमएल स्प्रेडशीट (.xlsx) |
| [Extension](../../groupdocs.redaction/filetype/extension) { get; } | फ़ाइल नाम प्रत्यय प्राप्त करता है (अवधि "।" सहित), उदाहरण के लिए ".doc"। |
| [FileFormat](../../groupdocs.redaction/filetype/fileformat) { get; } | फ़ाइल प्रकार का नाम प्राप्त करता है, उदाहरण के लिए "माइक्रोसॉफ्ट वर्ड दस्तावेज़"। |

## तरीकों

| नाम | विवरण |
| --- | --- |
| static [FromExtension](../../groupdocs.redaction/filetype/fromextension)(string) | फ़ाइल प्रकार के लिए मानचित्र फ़ाइल एक्सटेंशन. |
| [Equals](../../groupdocs.redaction/filetype/equals#equals)(FileType) | निर्धारित करता है कि क्या वर्तमान[`FileType`](../filetype) निर्दिष्ट के समान है[`FileType`](../filetype) वस्तु. |
| override [Equals](../../groupdocs.redaction/filetype/equals#equals_1)(object) | निर्धारित करता है कि क्या वर्तमान[`FileType`](../filetype) निर्दिष्ट वस्तु के समान है। |
| override [GetHashCode](../../groupdocs.redaction/filetype/gethashcode)() | वर्तमान के लिए हैश कोड लौटाता है[`FileType`](../filetype) वस्तु. |
| override [ToString](../../groupdocs.redaction/filetype/tostring)() | एक स्ट्रिंग लौटाता है जो वर्तमान वस्तु का प्रतिनिधित्व करता है। |
| static [GetSupportedFileTypes](../../groupdocs.redaction/filetype/getsupportedfiletypes)() | समर्थित फ़ाइल प्रकारों को पुनः प्राप्त करता है |
| [operator ==](../../groupdocs.redaction/filetype/op_equality) | निर्धारित करता है कि क्या दो[`FileType`](../filetype) वस्तुएं समान हैं। |
| [operator !=](../../groupdocs.redaction/filetype/op_inequality) | निर्धारित करता है कि क्या दो[`FileType`](../filetype) वस्तुएं समान नहीं हैं। |

### टिप्पणियों

**और अधिक जानें**

* [समर्थित दस्तावेज़ प्रारूप](https://docs.groupdocs.com/redaction/net/supported-document-formats/)
* [समर्थित फ़ाइल स्वरूप प्राप्त करें](https://docs.groupdocs.com/redaction/net/get-supported-file-formats/)
* [फ़ाइल जानकारी प्राप्त करें](https://docs.groupdocs.com/redaction/net/get-file-info/)

### यह सभी देखें

* नाम स्थान [GroupDocs.Redaction](../../groupdocs.redaction)
* सभा [GroupDocs.Redaction](../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Redaction.dll -->
