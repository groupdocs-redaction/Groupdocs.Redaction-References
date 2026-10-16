---
title: "FileType"
second_title: "GroupDocs.Redaction के लिए .NET API रेफ़रेंस"
description: "फ़ाइल प्रकार का प्रतिनिधित्व करता है। GroupDocs.Redaction द्वारा समर्थित सभी फ़ाइल प्रकारों की सूची प्राप्त करने, एक्सटेंशन द्वारा फ़ाइल प्रकार का पता लगाने आदि के लिए मेथड प्रदान करता है।"
type: docs
weight: 90
url: /hi/net/groupdocs.redaction/filetype/
---
## FileType class

फ़ाइल प्रकार का प्रतिनिधित्व करता है। सभी फ़ाइल प्रकारों की सूची प्राप्त करने के लिए मेथड प्रदान करता है जो GroupDocs.Redaction द्वारा समर्थित हैं, एक्सटेंशन द्वारा फ़ाइल प्रकार का पता लगाता है, आदि।

```csharp
public sealed class FileType : IEquatable<FileType>
```

## Properties

| नाम | विवरण |
| --- | --- |
| static [BMP](../../groupdocs.redaction/filetype/bmp) { get; } | बिटमैप इमेज फ़ाइल (.bmp) |
| static [CSV](../../groupdocs.redaction/filetype/csv) { get; } | कॉमा सेपरेटेड वैल्यूज़ फ़ाइल (.csv) |
| static [DJVU](../../groupdocs.redaction/filetype/djvu) { get; } | DjVu छवि (.djvu) |
| static [DOC](../../groupdocs.redaction/filetype/doc) { get; } | Microsoft Word दस्तावेज़ (.doc) |
| static [DOCM](../../groupdocs.redaction/filetype/docm) { get; } | Word Open XML मैक्रो-सक्षम दस्तावेज़ (.docm) |
| static [DOCX](../../groupdocs.redaction/filetype/docx) { get; } | Microsoft Word Open XML दस्तावेज़ (.docx) |
| static [DOT](../../groupdocs.redaction/filetype/dot) { get; } | Word दस्तावेज़ टेम्पलेट (.dot) |
| static [DOTM](../../groupdocs.redaction/filetype/dotm) { get; } | Word Open XML मैक्रो-सक्षम दस्तावेज़ टेम्पलेट (.dotm) |
| static [DOTX](../../groupdocs.redaction/filetype/dotx) { get; } | Word Open XML दस्तावेज़ टेम्पलेट (.dotx) |
| static [GIF](../../groupdocs.redaction/filetype/gif) { get; } | ग्राफ़िकल इंटरचेंज फ़ॉर्मेट फ़ाइल (.gif) |
| static [HTM](../../groupdocs.redaction/filetype/htm) { get; } | हाइपरटेक्स्ट मार्कअप लैंग्वेज फ़ाइल (.htm) |
| static [HTML](../../groupdocs.redaction/filetype/html) { get; } | हाइपरटेक्स्ट मार्कअप लैंग्वेज फ़ाइल (.html) |
| static [JP2](../../groupdocs.redaction/filetype/jp2) { get; } | JPEG 2000 कोर इमेज फ़ाइल (.jp2) |
| static [JPEG](../../groupdocs.redaction/filetype/jpeg) { get; } | JPEG इमेज (.jpeg) |
| static [JPG](../../groupdocs.redaction/filetype/jpg) { get; } | JPEG इमेज (.jpg) |
| static [LOG](../../groupdocs.redaction/filetype/log) { get; } | लॉग फ़ाइल (.log) |
| static [MD](../../groupdocs.redaction/filetype/md) { get; } | मार्कडाउन डॉक्यूमेंटेशन फ़ाइल (.md) |
| static [NUMBERS](../../groupdocs.redaction/filetype/numbers) { get; } | Apple Numbers स्प्रेडशीट (.numbers) |
| static [ODP](../../groupdocs.redaction/filetype/odp) { get; } | OpenDocument प्रेज़ेंटेशन (.odp) |
| static [ODS](../../groupdocs.redaction/filetype/ods) { get; } | OpenDocument स्प्रेडशीट (.ods) |
| static [ODT](../../groupdocs.redaction/filetype/odt) { get; } | OpenDocument टेक्स्ट दस्तावेज़ (.odt) |
| static [OTP](../../groupdocs.redaction/filetype/otp) { get; } | OpenDocument प्रेज़ेंटेशन टेम्पलेट (.otp) |
| static [OTS](../../groupdocs.redaction/filetype/ots) { get; } | OpenDocument स्प्रेडशीट टेम्पलेट (.ots) |
| static [OTT](../../groupdocs.redaction/filetype/ott) { get; } | OpenDocument दस्तावेज़ टेम्पलेट (.ott) |
| static [PDF](../../groupdocs.redaction/filetype/pdf) { get; } | पोर्टेबल डॉक्यूमेंट फ़ॉर्मेट फ़ाइल (.pdf) |
| static [PNG](../../groupdocs.redaction/filetype/png) { get; } | पोर्टेबल नेटवर्क ग्राफ़िक (.png) |
| static [POTM](../../groupdocs.redaction/filetype/potm) { get; } | PowerPoint Open XML मैक्रो-सक्षम प्रस्तुति टेम्पलेट (.potm) |
| static [POTX](../../groupdocs.redaction/filetype/potx) { get; } | PowerPoint Open XML प्रस्तुति टेम्पलेट (.potx) |
| static [PPS](../../groupdocs.redaction/filetype/pps) { get; } | PowerPoint स्लाइड शो (.pps) |
| static [PPSM](../../groupdocs.redaction/filetype/ppsm) { get; } | PowerPoint Open XML मैक्रो-सक्षम स्लाइड (.ppsm) |
| static [PPSX](../../groupdocs.redaction/filetype/ppsx) { get; } | PowerPoint Open XML स्लाइड शो (.ppsx) |
| static [PPT](../../groupdocs.redaction/filetype/ppt) { get; } | PowerPoint प्रस्तुति (.ppt) |
| static [PPTM](../../groupdocs.redaction/filetype/pptm) { get; } | PowerPoint Open XML मैक्रो-सक्षम प्रस्तुति |
| static [PPTX](../../groupdocs.redaction/filetype/pptx) { get; } | PowerPoint Open XML प्रस्तुति (.pptx) |
| static [RTF](../../groupdocs.redaction/filetype/rtf) { get; } | रिच टेक्स्ट फॉर्मेट फ़ाइल (.rtf) |
| static [TAB](../../groupdocs.redaction/filetype/tab) { get; } | टैब सेपरेटेड वैल्यू फ़ाइल (.tab) |
| static [TIF](../../groupdocs.redaction/filetype/tif) { get; } | टैग्ड इमेज फ़ाइल (.tif) |
| static [TIFF](../../groupdocs.redaction/filetype/tiff) { get; } | टैग्ड इमेज फ़ाइल फ़ॉर्मेट (.tiff) |
| static [TSV](../../groupdocs.redaction/filetype/tsv) { get; } | टैब सेपरेटेड वैल्यू फ़ाइल (.tsv) |
| static [TXT](../../groupdocs.redaction/filetype/txt) { get; } | सादा टेक्स्ट फ़ाइल (.txt) |
| static [Unknown](../../groupdocs.redaction/filetype/unknown) { get; } | अज्ञात फ़ाइल प्रकार को दर्शाता है। |
| static [WEBP](../../groupdocs.redaction/filetype/webp) { get; } | WebP छवि (.webp) |
| static [XLS](../../groupdocs.redaction/filetype/xls) { get; } | Excel स्प्रेडशीट (.xls) |
| static [XLSB](../../groupdocs.redaction/filetype/xlsb) { get; } | Excel बाइनरी स्प्रेडशीट (.xlsb) |
| static [XLSM](../../groupdocs.redaction/filetype/xlsm) { get; } | Excel Open XML मैक्रो-सक्षम स्प्रेडशीट (.xlsm) |
| static [XLSX](../../groupdocs.redaction/filetype/xlsx) { get; } | Microsoft Excel Open XML स्प्रेडशीट (.xlsx) |
| static [XLT](../../groupdocs.redaction/filetype/xlt) { get; } | Excel टेम्पलेट (.xlt) |
| static [XLTM](../../groupdocs.redaction/filetype/xltm) { get; } | Excel Open XML मैक्रो-सक्षम स्प्रेडशीट टेम्पलेट (.xltm) |
| static [XLTX](../../groupdocs.redaction/filetype/xltx) { get; } | Excel Open XML स्प्रेडशीट टेम्पलेट (.xltx) |
| [Extension](../../groupdocs.redaction/filetype/extension) { get; } | फ़ाइलनाम प्रत्यय प्राप्त करता है (बिंदु "." सहित), उदाहरण के लिए ".doc"। |
| [FileFormat](../../groupdocs.redaction/filetype/fileformat) { get; } | फ़ाइल प्रकार का नाम प्राप्त करता है, उदाहरण के लिए "Microsoft Word Document"। |

## विधियाँ

| नाम | विवरण |
| --- | --- |
| static [FromExtension](../../groupdocs.redaction/filetype/fromextension)(string) | फ़ाइल एक्सटेंशन को फ़ाइल प्रकार से मैप करता है। |
| [Equals](../../groupdocs.redaction/filetype/equals#equals)(FileType) | निर्धारित करता है कि वर्तमान [`FileType`](../filetype) निर्दिष्ट [`FileType`](../filetype) ऑब्जेक्ट के समान है या नहीं। |
| override [Equals](../../groupdocs.redaction/filetype/equals#equals_1)(object) | निर्धारित करता है कि वर्तमान [`FileType`](../filetype) निर्दिष्ट ऑब्जेक्ट के समान है या नहीं। |
| override [GetHashCode](../../groupdocs.redaction/filetype/gethashcode)() | वर्तमान [`FileType`](../filetype) ऑब्जेक्ट के लिए हैश कोड लौटाता है। |
| override [ToString](../../groupdocs.redaction/filetype/tostring)() | वर्तमान ऑब्जेक्ट का प्रतिनिधित्व करने वाली स्ट्रिंग लौटाता है। |
| static [GetSupportedFileTypes](../../groupdocs.redaction/filetype/getsupportedfiletypes)() | समर्थित फ़ाइल प्रकारों को प्राप्त करता है |
| [operator ==](../../groupdocs.redaction/filetype/op_equality) | निर्धारित करता है कि दो [`FileType`](../filetype) ऑब्जेक्ट समान हैं या नहीं। |
| [operator !=](../../groupdocs.redaction/filetype/op_inequality) | निर्धारित करता है कि दो [`FileType`](../filetype) ऑब्जेक्ट समान नहीं हैं या नहीं। |

### टिप्पणियाँ

**Learn more**

* [Supported Document Formats](https://docs.groupdocs.com/redaction/net/supported-document-formats/)
* [Get supported file formats](https://docs.groupdocs.com/redaction/net/get-supported-file-formats/)
* [Get file info](https://docs.groupdocs.com/redaction/net/get-file-info/)

### साथ ही देखें

* namespace [GroupDocs.Redaction](../../groupdocs.redaction)
* assembly [GroupDocs.Redaction](../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Redaction.dll -->
