---
title: "ファイル情報を取得"
linkTitle: "Get file info"
second_title: "GroupDocs.Redaction for Python via .NET API リファレンス"
description: "この記事では、GroupDocs.Redaction API が一般的な文書情報（FileType、PageCount、FileSize を含む）を取得する機能について説明します。"
type: docs
url: /ja/python-net/guides/get-file-info/
is_root: false
weight: 120
---


GroupDocs.Redaction は以下を含む一般的な文書情報を提供します:

*   FileType
*   PageCount
*   FileSize

以下のコード例は、文書情報を取得する方法を示しています。

## Get file info for a file from local disk

```python
from groupdocs.redaction import Redactor

def get_local_file_info():
    # ローカルディスクから文書を読み込む
    with Redactor("./sample.docx") as redactor:
        # 一般的な文書情報を取得する
        info = redactor.get_document_info()

        print(f"File type: {info.file_type}")
        print(f"Number of pages: {info.page_count}")
        print(f"Document size: {info.size} bytes")

if __name__ == "__main__":
    get_local_file_info()
```

`sample.docx` はこの例で使用されるサンプルファイルです。[here](https://docs.groupdocs.com/redaction/python-net/_sample_files/developer-guide/basic-usage/get-file-info/sample.docx) をクリックしてダウンロードしてください。

  
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
    # バイナリストリームとして文書を開く
    with open("./sample.docx", "rb") as stream:
        # ストリームから文書を読み込む
        with Redactor(stream) as redactor:
            # 一般的な文書情報を取得する
            info = redactor.get_document_info()

            print(f"File type: {info.file_type}")
            print(f"Number of pages: {info.page_count}")
            print(f"Document size: {info.size} bytes")

if __name__ == "__main__":
    get_file_info_from_stream()
```

`sample.docx` はこの例で使用されるサンプルファイルです。[here](https://docs.groupdocs.com/redaction/python-net/_sample_files/developer-guide/basic-usage/get-file-info/sample.docx) をクリックしてダウンロードしてください。

  
```text
File type: Microsoft Word Open XML Document (.docx)
Number of pages: 1
Document size: 19370 bytes
```
[Download full output](https://docs.groupdocs.com/redaction/python-net/_output_files/developer-guide/basic-usage/get-file-info/get_file_info_from_stream/get-file-info-from-stream.txt)
