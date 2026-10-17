---
title: "지원되는 파일 형식 가져오기"
linkTitle: "Get supported file formats"
second_title: "GroupDocs.Redaction for Python via .NET API 참조"
description: "이 문서는 Python을 사용하여 GroupDocs.Redaction의 모든 지원 파일 형식 목록을 가져오는 방법을 보여줍니다."
type: docs
url: /ko/python-net/guides/get-supported-file-formats/
is_root: false
weight: 130
---


GroupDocs.Redaction은 다음 단계에 따라 모든 지원 파일 형식 목록을 가져올 수 있습니다:

*   Call [GetSupportedFileTypes](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction/filetype/get_supported_file_types/) of [FileType](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction/filetype/) class;
*   Enumerate through the collection of [FileType](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction/filetype/) objects*.*

다음 예제는 지원 파일 형식 목록을 가져오는 방법을 보여줍니다.

```python
from groupdocs.redaction import FileType

def list_supported_formats():
    # 지원 파일 유형 컬렉션 가져오기
    supported_file_types = FileType.get_supported_file_types()

    # 확장자별로 정렬된 파일 유형 열거
    for file_type in sorted(supported_file_types, key=lambda x: x.extension):
        print(file_type)

if __name__ == "__main__":
    list_supported_formats()
```

  
```text
Bitmap Image File (.bmp)
Comma Separated Values File (.csv)
Microsoft Word Document (.doc)
Word Open XML Macro-Enabled Document (.docm)
Microsoft Word Open XML Document (.docx)
Word Document Template (.dot)
Word Open XML Macro-Enabled Document Template (.dotm)
Word Open XML Document Template (.dotx)
Graphical Interchange Format File (.gif)
Hypertext Markup Language File (.htm)
[TRUNCATED]
```
[Download full output](https://docs.groupdocs.com/redaction/python-net/_output_files/developer-guide/basic-usage/get-supported-file-formats/list_supported_formats/list-supported-formats.txt)
