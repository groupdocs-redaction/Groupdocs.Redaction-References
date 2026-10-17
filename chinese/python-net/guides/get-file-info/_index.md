---
title: "获取文件信息"
linkTitle: "Get file info"
second_title: "GroupDocs.Redaction 用于 Python，通过 .NET API 参考"
description: "本文说明了 GroupDocs.Redaction API 获取通用文档信息的功能，信息包括 FileType、PageCount 和 FileSize。"
type: docs
url: /zh/python-net/guides/get-file-info/
is_root: false
weight: 120
---


GroupDocs.Redaction 提供通用文档信息，内容包括：

*   FileType
*   PageCount
*   FileSize

以下代码示例演示如何获取文档信息。

## Get file info for a file from local disk

```python
from groupdocs.redaction import Redactor

def get_local_file_info():
    # 从本地磁盘加载文档
    with Redactor("./sample.docx") as redactor:
        # 检索通用文档信息
        info = redactor.get_document_info()

        print(f"File type: {info.file_type}")
        print(f"Number of pages: {info.page_count}")
        print(f"Document size: {info.size} bytes")

if __name__ == "__main__":
    get_local_file_info()
```

`sample.docx` 是本示例使用的示例文件。点击 [here](https://docs.groupdocs.com/redaction/python-net/_sample_files/developer-guide/basic-usage/get-file-info/sample.docx) 下载。

  
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
    # 以二进制流打开文档
    with open("./sample.docx", "rb") as stream:
        # 从流加载文档
        with Redactor(stream) as redactor:
            # 检索通用文档信息
            info = redactor.get_document_info()

            print(f"File type: {info.file_type}")
            print(f"Number of pages: {info.page_count}")
            print(f"Document size: {info.size} bytes")

if __name__ == "__main__":
    get_file_info_from_stream()
```

`sample.docx` 是本示例使用的示例文件。点击 [here](https://docs.groupdocs.com/redaction/python-net/_sample_files/developer-guide/basic-usage/get-file-info/sample.docx) 下载。

  
```text
File type: Microsoft Word Open XML Document (.docx)
Number of pages: 1
Document size: 19370 bytes
```
[Download full output](https://docs.groupdocs.com/redaction/python-net/_output_files/developer-guide/basic-usage/get-file-info/get_file_info_from_stream/get-file-info-from-stream.txt)
