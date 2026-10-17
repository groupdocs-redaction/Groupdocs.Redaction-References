---
title: "मेटाडेटा रिडैक्शन"
linkTitle: "Metadata redactions"
second_title: "GroupDocs.Redaction for Python via .NET API संदर्भ"
description: "यह लेख दर्शाता है कि Python रिडैक्शन API कैसे फ़िल्टर या रेगुलर एक्सप्रेशन द्वारा खोज का उपयोग करके मेटाडेटा को बदलने या हटाने की अनुमति देता है।"
type: docs
url: /hi/python-net/guides/metadata-redactions/
is_root: false
weight: 70
---


GroupDocs.Redaction API के साथ आप PDF, DOC, DOCX, PPT, PPTX, XLS, XLSX और अन्य विभिन्न फ़ॉर्मेट के दस्तावेज़ों पर मेटाडेटा रिडैक्शन लागू कर सकते हैं। पूर्ण सूची के लिए देखें [supported document formats]() लेख।

GroupDocs.Redactions एक लचीला API प्रदान करता है जो फ़िल्टर या रेगुलर एक्सप्रेशन द्वारा खोज का उपयोग करके मेटाडेटा को बदलने या हटाने की अनुमति देता है।

## Filter metadata

सभी रिडैक्शन के लिए बेस कार्यक्षमता, जो [MetadataRedaction](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction.redactions/metadataredaction/) बेस क्लास से व्युत्पन्न है, *metadata filtering* है और यह मेटाडेटा रिडैक्शन के लिए अनिवार्य है। यह फ़्लैग्ड एन्क्यूमरेशन [MetadataFilters](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction.redactions/metadatafilters/) का उपयोग करता है, जिसमें सबसे सामान्य मेटाडेटा प्रविष्टियों के आइटम होते हैं। आप फ़िल्टर को *All* पर सेट कर सकते हैं, या मेटाडेटा के किसी भी संयोजन पर। उदाहरण के लिए, नीचे दिया गया उदाहरण फ़िल्टर को *Author*, *Manager* और *NameOfApplication* पर सेट करता है - टेक्स्टुअल रिडैक्शन या उन्हें साफ़ करने के लिए:

```python
# MetadataRedaction से व्युत्पन्न रिडैक्शन
redaction.filter = MetadataFilters.AUTHOR | MetadataFilters.MANAGER | MetadataFilters.NAME_OF_APPLICATION
```

नीचे [MetadataFilters](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction.redactions/metadatafilters/) आइटमों की पूर्ण सूची वाली तालिका है:

| फ़िल्टर | संख्यात्मक मान | विवरण |
| --- | --- | --- |
| *None* | 0 | खाली फ़िल्टर सेटिंग, कोई मेटाडेटा आइटम नहीं मिलते |
| *Author* | 1 | दस्तावेज़ का लेखक |
| *श्रेणी* | 2 | दस्तावेज़ की श्रेणी |
| *टिप्पणियाँ* | 4 | दस्तावेज़ टिप्पणी |
| *कंपनी* | 8 | लेखक की कंपनी |
| *सामग्रीस्थिति* | 16 | सामग्री स्थिति |
| *निर्माणसमय* | 32 | निर्माण समय |
| *हाइपरलिंकबेस* | 64 | हाइपरलिंक बेस |
| *अंतिमप्रिंटेड* | 128 | अंतिम प्रिंट तिथि और समय |
| *अंतिमसहेजनेवाला* | 256 | उपयोगकर्ता द्वारा अंतिम सहेजा गया |
| *LastSavedTime* | 1024 | अंतिम सहेजी गई तिथि और समय |
| *NameOfApplication* | 2048 | ऐप्लिकेशन का नाम जहाँ दस्तावेज़ बनाया गया था |
| *Manager* | 4096 | लेखक के प्रबंधक का नाम |
| *RevisionNumber* | 8192 | संशोधन संख्या |
| *Subject* | 16384 | दस्तावेज़ का विषय |
| *Template* | 32768 | दस्तावेज़ टेम्पलेट का नाम |
| *Title* | 65536 | दस्तावेज़ शीर्षक |
| *TotalEditingTime* | 131072 | कुल संपादन समय |
| *Version* | 262144 | दस्तावेज़ का संस्करण |
| *Description* | 524288 | दस्तावेज़ का विवरण |
| *Keywords* | 1048576 | दस्तावेज़ के कीवर्ड |
| *ContentType* | 2097152 | सामग्री प्रकार |
| *All* | 2147483647 | मेटाडाटा आइटम के सभी प्रकार |

## Clean metadata

आप दस्तावेज़ में सभी या विशिष्ट मेटाडाटा को खाली (खाली या न्यूनतम) मानों से बदल सकते हैं, इसके लिए [EraseMetadataRedaction](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction.redactions/erasemetadataredaction/) क्लास का उपयोग करें। नीचे दिया गया उदाहरण दस्तावेज़ की सभी प्रॉपर्टीज़ को खाली कर देता है:

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.options import SaveOptions
from groupdocs.redaction.redactions import EraseMetadataRedaction, MetadataFilters

def clean_all_metadata():
    # सभी मेटाडाटा को मिटाने के लिए रेडैक्शन विकल्प निर्दिष्ट करें
    met_red = EraseMetadataRedaction(MetadataFilters.ALL)

    # रेडैक्ट किए जाने वाले दस्तावेज़ को लोड करें
    with Redactor("./sample.docx") as redactor:
        # रेडैक्शन लागू करें
        result = redactor.apply(met_red)

        # रिडैक्टेड दस्तावेज़ को स्रोत फ़ाइल के बगल में सहेजें
        so = SaveOptions()
        so.add_suffix = True
        so.rasterize_to_pdf = False
        so.redacted_file_suffix = "redacted"
        redactor.save(so)

if __name__ == "__main__":
    clean_all_metadata()
```

`sample.docx` इस उदाहरण में उपयोग की गई नमूना फ़ाइल है। इसे डाउनलोड करने के लिए [here](https://docs.groupdocs.com/redaction/python-net/_sample_files/developer-guide/basic-usage/metadata-redactions/sample.docx) पर क्लिक करें।

  
```text
Binary file (DOCX, 16 KB)
```
[Download full output](https://docs.groupdocs.com/redaction/python-net/_output_files/developer-guide/basic-usage/metadata-redactions/clean_all_metadata/sample_redacted.docx)

आप [MetadataFilter.All](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction.redactions/metadatafilters/) निर्दिष्ट कर सकते हैं या डिफ़ॉल्ट कन्स्ट्रक्टर का उपयोग करके दिए गए दस्तावेज़ में सभी मेटाडाटा को खाली कर सकते हैं, Custom - सभी कस्टम मेटाडाटा एंट्रीज़ को साफ़ करने के लिए।

## Redact metadata

आप [MetadataSearchRedaction](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction.redactions/metadatasearchredaction/) का उपयोग करके नियमित अभिव्यक्तियों के माध्यम से दस्तावेज़ के मेटाडाटा से संवेदनशील डेटा हटा सकते हैं। उदाहरण के लिए, हम "Company Ltd." का कोई भी उल्लेख हटा सकते हैं:

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.options import SaveOptions
from groupdocs.redaction.redactions import MetadataSearchRedaction

def redact_metadata():
    # रेडैक्शन विकल्प निर्दिष्ट करें: खोज पैटर्न और प्रतिस्थापन स्ट्रिंग
    met_red = MetadataSearchRedaction("Company Ltd.", "--company--")

    # रेडैक्ट किए जाने वाले दस्तावेज़ को लोड करें
    with Redactor("./sample.docx") as redactor:
        # रेडैक्शन लागू करें
        result = redactor.apply(met_red)

        # रिडैक्टेड दस्तावेज़ को स्रोत फ़ाइल के बगल में सहेजें
        so = SaveOptions()
        so.add_suffix = True
        so.rasterize_to_pdf = False
        so.redacted_file_suffix = "redacted"
        redactor.save(so)

if __name__ == "__main__":
    redact_metadata()
```

`sample.docx` इस उदाहरण में उपयोग की गई नमूना फ़ाइल है। इसे डाउनलोड करने के लिए [here](https://docs.groupdocs.com/redaction/python-net/_sample_files/developer-guide/basic-usage/metadata-redactions/sample.docx) पर क्लिक करें।

  
```text
Binary file (DOCX, 16 KB)
```
[Download full output](https://docs.groupdocs.com/redaction/python-net/_output_files/developer-guide/basic-usage/metadata-redactions/redact_metadata/sample_redacted.docx)

पहला तर्क नियमित अभिव्यक्ति है, दूसरा प्रतिस्थापन स्ट्रिंग। आप फ़िल्टर सेट करके रेडैक्शन का दायरा भी निर्धारित कर सकते हैं, उदाहरण के लिए [MetadataFilter.Company](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction.redactions/metadatafilters/). - यह सभी मेटाडाटा आइटम में नियमित अभिव्यक्ति के मिलान को अनडन छोड़ देगा, सिवाय "Company" प्रॉपर्टी के:

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.options import SaveOptions
from groupdocs.redaction.redactions import MetadataSearchRedaction, MetadataFilters

def redact_metadata_with_filter():
    # रेडैक्शन विकल्प निर्दिष्ट करें: खोज पैटर्न और प्रतिस्थापन स्ट्रिंग
    met_red = MetadataSearchRedaction("Company Ltd.", "--company--")

    # रेडैक्शन दायरे को केवल Company मेटाडाटा आइटम तक सीमित करें
    met_red.filter = MetadataFilters.COMPANY

    # रेडैक्ट किए जाने वाले दस्तावेज़ को लोड करें
    with Redactor("./sample.docx") as redactor:
        # रेडैक्शन लागू करें
        result = redactor.apply(met_red)

        # रिडैक्टेड दस्तावेज़ को स्रोत फ़ाइल के बगल में सहेजें
        so = SaveOptions()
        so.add_suffix = True
        so.rasterize_to_pdf = False
        so.redacted_file_suffix = "redacted"
        redactor.save(so)

if __name__ == "__main__":
    redact_metadata_with_filter()
```

`sample.docx` इस उदाहरण में उपयोग की गई नमूना फ़ाइल है। इसे डाउनलोड करने के लिए [here](https://docs.groupdocs.com/redaction/python-net/_sample_files/developer-guide/basic-usage/metadata-redactions/sample.docx) पर क्लिक करें।

  
```text
Binary file (DOCX, 16 KB)
```
[Download full output](https://docs.groupdocs.com/redaction/python-net/_output_files/developer-guide/basic-usage/metadata-redactions/redact_metadata_with_filter/sample_redacted.docx)

## Metadata redaction status

सभी मेटाडाटा रेडैक्शन प्रत्येक मेटाडाटा आइटम पर अलग-अलग लागू होते हैं, और यदि किसी मेटाडाटा आइटम का रेडैक्शन विफल हो भी जाता है, तो बाकी मेटाडाटा आइटम अपडेट हो जाएंगे। आप विफल, स्किप (अस्वीकृत) मेटाडाटा आइटमों की सूची और उनके कारणों को [ErrorMessage](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction/redactionresult/error_message/) प्रॉपर्टी में [RedactorLogEntry.Result](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction/redactorlogentry/result/) के तहत पा सकते हैं।
