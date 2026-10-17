---
title: "파일 정보 가져오기"
linkTitle: "Get file info"
second_title: "GroupDocs.Redaction for Python via .NET API 참조"
description: "이 문서는 GroupDocs.Redaction API가 파일 유형, 페이지 수 및 파일 크기를 포함한 일반 문서 정보를 가져오는 기능을 설명합니다."
type: docs
url: /ko/python-net/guides/get-file-info/
is_root: false
weight: 120
---


GroupDocs.Redaction은 다음과 같은 일반 문서 정보를 제공합니다:

*   FileType
*   PageCount
*   FileSize

다음 코드 예제는 문서 정보를 가져오는 방법을 보여줍니다.

## Get file info for a file from local disk

```python
from groupdocs.redaction import Redactor

def get_local_file_info():
    # 로컬 디스크에서 문서 로드
    with Redactor("./sample.docx") as redactor:
        # 일반 문서 정보 검색
        info = redactor.get_document_info()

        print(f"File type: {info.file_type}")
        print(f"Number of pages: {info.page_count}")
        print(f"Document size: {info.size} bytes")

if __name__ == "__main__":
    get_local_file_info()
```

`sample.docx`는 이 예제에서 사용되는 샘플 파일입니다. 다운로드하려면 [here](https://docs.groupdocs.com/redaction/python-net/_sample_files/developer-guide/basic-usage/get-file-info/sample.docx)를 클릭하십시오.

  
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
    # 문서를 바이너리 스트림으로 열기
    with open("./sample.docx", "rb") as stream:
        # 스트림에서 문서 로드
        with Redactor(stream) as redactor:
            # 일반 문서 정보 검색
            info = redactor.get_document_info()

            print(f"File type: {info.file_type}")
            print(f"Number of pages: {info.page_count}")
            print(f"Document size: {info.size} bytes")

if __name__ == "__main__":
    get_file_info_from_stream()
```

`sample.docx`는 이 예제에서 사용되는 샘플 파일입니다. 다운로드하려면 [here](https://docs.groupdocs.com/redaction/python-net/_sample_files/developer-guide/basic-usage/get-file-info/sample.docx)를 클릭하십시오.

  
```text
File type: Microsoft Word Open XML Document (.docx)
Number of pages: 1
Document size: 19370 bytes
```
[Download full output](https://docs.groupdocs.com/redaction/python-net/_output_files/developer-guide/basic-usage/get-file-info/get_file_info_from_stream/get-file-info-from-stream.txt)
