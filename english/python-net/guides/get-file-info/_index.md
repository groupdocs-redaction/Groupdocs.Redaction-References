---
title: Get file info
linkTitle: "Get file info"
second_title: GroupDocs.Redaction for Python via .NET API References
description: "This article explains the ability of the GroupDocs.Redaction API to get the general document information, which includes FileType, PageCount and FileSize."
type: docs
url: /python-net/guides/get-file-info/
is_root: false
weight: 120
---


GroupDocs.Redaction provides general document information, which includes:

*   FileType
*   PageCount
*   FileSize

The following code examples demonstrate how to get document information.

## Get file info for a file from local disk

```python
from groupdocs.redaction import Redactor

def get_local_file_info():
    # Load the document from local disk
    with Redactor("./sample.docx") as redactor:
        # Retrieve general document information
        info = redactor.get_document_info()

        print(f"File type: {info.file_type}")
        print(f"Number of pages: {info.page_count}")
        print(f"Document size: {info.size} bytes")

if __name__ == "__main__":
    get_local_file_info()
```

`sample.docx` is the sample file used in this example. Click [here](https://docs.groupdocs.com/redaction/python-net/_sample_files/developer-guide/basic-usage/get-file-info/sample.docx) to download it.

  
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
    # Open the document as a binary stream
    with open("./sample.docx", "rb") as stream:
        # Load the document from the stream
        with Redactor(stream) as redactor:
            # Retrieve general document information
            info = redactor.get_document_info()

            print(f"File type: {info.file_type}")
            print(f"Number of pages: {info.page_count}")
            print(f"Document size: {info.size} bytes")

if __name__ == "__main__":
    get_file_info_from_stream()
```

`sample.docx` is the sample file used in this example. Click [here](https://docs.groupdocs.com/redaction/python-net/_sample_files/developer-guide/basic-usage/get-file-info/sample.docx) to download it.

  
```text
File type: Microsoft Word Open XML Document (.docx)
Number of pages: 1
Document size: 19370 bytes
```
[Download full output](https://docs.groupdocs.com/redaction/python-net/_output_files/developer-guide/basic-usage/get-file-info/get_file_info_from_stream/get-file-info-from-stream.txt)
