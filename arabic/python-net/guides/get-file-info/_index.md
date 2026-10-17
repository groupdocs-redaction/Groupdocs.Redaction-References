---
title: "احصل على معلومات الملف"
linkTitle: "Get file info"
second_title: "مراجع API لـ GroupDocs.Redaction للبايثون عبر .NET"
description: "توضح هذه المقالة قدرة واجهة برمجة تطبيقات GroupDocs.Redaction على الحصول على معلومات الوثيقة العامة، والتي تشمل نوع الملف، عدد الصفحات وحجم الملف."
type: docs
url: /ar/python-net/guides/get-file-info/
is_root: false
weight: 120
---


GroupDocs.Redaction يوفر معلومات الوثيقة العامة، والتي تشمل:

*   FileType
*   PageCount
*   FileSize

توضح الأمثلة البرمجية التالية كيفية الحصول على معلومات الوثيقة.

## Get file info for a file from local disk

```python
from groupdocs.redaction import Redactor

def get_local_file_info():
    # حمّل الوثيقة من القرص المحلي
    with Redactor("./sample.docx") as redactor:
        # استرجع معلومات الوثيقة العامة
        info = redactor.get_document_info()

        print(f"File type: {info.file_type}")
        print(f"Number of pages: {info.page_count}")
        print(f"Document size: {info.size} bytes")

if __name__ == "__main__":
    get_local_file_info()
```

`sample.docx` هو ملف العينة المستخدم في هذا المثال. انقر [هنا](https://docs.groupdocs.com/redaction/python-net/_sample_files/developer-guide/basic-usage/get-file-info/sample.docx) لتنزيله.

  
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
    # افتح الوثيقة كتيار ثنائي
    with open("./sample.docx", "rb") as stream:
        # حمّل الوثيقة من التيار
        with Redactor(stream) as redactor:
            # استرجع معلومات الوثيقة العامة
            info = redactor.get_document_info()

            print(f"File type: {info.file_type}")
            print(f"Number of pages: {info.page_count}")
            print(f"Document size: {info.size} bytes")

if __name__ == "__main__":
    get_file_info_from_stream()
```

`sample.docx` هو ملف العينة المستخدم في هذا المثال. انقر [هنا](https://docs.groupdocs.com/redaction/python-net/_sample_files/developer-guide/basic-usage/get-file-info/sample.docx) لتنزيله.

  
```text
File type: Microsoft Word Open XML Document (.docx)
Number of pages: 1
Document size: 19370 bytes
```
[Download full output](https://docs.groupdocs.com/redaction/python-net/_output_files/developer-guide/basic-usage/get-file-info/get_file_info_from_stream/get-file-info-from-stream.txt)
