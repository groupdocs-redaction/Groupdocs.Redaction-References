---
title: "फ़ाइल जानकारी प्राप्त करें"
linkTitle: "Get file info"
second_title: "GroupDocs.Redaction for Python via .NET API संदर्भ"
description: "यह लेख GroupDocs.Redaction API की सामान्य दस्तावेज़ जानकारी प्राप्त करने की क्षमता को समझाता है, जिसमें FileType, PageCount और FileSize शामिल हैं।"
type: docs
url: /hi/python-net/guides/get-file-info/
is_root: false
weight: 120
---


GroupDocs.Redaction सामान्य दस्तावेज़ जानकारी प्रदान करता है, जिसमें शामिल हैं:

*   FileType
*   PageCount
*   FileSize

निम्नलिखित कोड उदाहरण दर्शाते हैं कि दस्तावेज़ जानकारी कैसे प्राप्त करें।

## Get file info for a file from local disk

```python
from groupdocs.redaction import Redactor

def get_local_file_info():
    # दस्तावेज़ को स्थानीय डिस्क से लोड करें
    with Redactor("./sample.docx") as redactor:
        # सामान्य दस्तावेज़ जानकारी प्राप्त करें
        info = redactor.get_document_info()

        print(f"File type: {info.file_type}")
        print(f"Number of pages: {info.page_count}")
        print(f"Document size: {info.size} bytes")

if __name__ == "__main__":
    get_local_file_info()
```

`sample.docx` इस उदाहरण में उपयोग की गई नमूना फ़ाइल है। इसे डाउनलोड करने के लिए [यहाँ](https://docs.groupdocs.com/redaction/python-net/_sample_files/developer-guide/basic-usage/get-file-info/sample.docx) पर क्लिक करें।

  
```text
File type: Microsoft Word Open XML Document (.docx)
Number of pages: 1
Document size: 19370 bytes
```
[Download full output](https://docs.groupdocs.com/redaction/python-net/_output_files/developer-guide/basic-usage/get-file-info/get_local_file_info/get-local-file-info.txt)

## Get file info for a file from Stream

```python
from groupdocs.redaction import Redactor

def get_file_info_from_stream():
    # दस्तावेज़ को बाइनरी स्ट्रीम के रूप में खोलें
    with open("./sample.docx", "rb") as stream:
        # स्ट्रीम से दस्तावेज़ लोड करें
        with Redactor(stream) as redactor:
            # सामान्य दस्तावेज़ जानकारी प्राप्त करें
            info = redactor.get_document_info()

            print(f"File type: {info.file_type}")
            print(f"Number of pages: {info.page_count}")
            print(f"Document size: {info.size} bytes")

if __name__ == "__main__":
    get_file_info_from_stream()
```

`sample.docx` इस उदाहरण में उपयोग की गई नमूना फ़ाइल है। इसे डाउनलोड करने के लिए [यहाँ](https://docs.groupdocs.com/redaction/python-net/_sample_files/developer-guide/basic-usage/get-file-info/sample.docx) पर क्लिक करें।

  
```text
File type: Microsoft Word Open XML Document (.docx)
Number of pages: 1
Document size: 19370 bytes
```
[Download full output](https://docs.groupdocs.com/redaction/python-net/_output_files/developer-guide/basic-usage/get-file-info/get_file_info_from_stream/get-file-info-from-stream.txt)
