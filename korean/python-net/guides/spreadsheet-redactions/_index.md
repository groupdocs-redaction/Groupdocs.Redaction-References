---
title: "스프레드시트 편집"
linkTitle: "Spreadsheet redactions"
second_title: "GroupDocs.Redaction for Python via .NET API 참조"
description: "이 문서는 Python 편집 API가 XLS, XLSX, ODS 스프레드시트 문서 형식 및 기타 형식에서 민감하거나 개인적인 데이터를 편집하는 방법을 보여줍니다."
type: docs
url: /ko/python-net/guides/spreadsheet-redactions/
is_root: false
weight: 90
---


GroupDocs.Redaction은 XLS, XLSX, ODS 스프레드시트 문서 형식 및 기타 형식에서 민감하거나 개인적인 데이터를 편집할 수 있습니다. 전체 목록은 [supported document formats]() 문서를 참조하십시오.

## Redact spreadsheet content

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.options import SaveOptions
from groupdocs.redaction.redactions import ExactPhraseRedaction, ReplacementOptions

def redact_spreadsheet_content():
    # 편집 옵션을 지정합니다
    repl_opt = ReplacementOptions("-redacted-")
    ex_red = ExactPhraseRedaction("John Doe", repl_opt)

    # 편집할 스프레드시트를 로드합니다
    with Redactor("./sample.xlsx") as redactor:
        # 가리기를 적용합니다
        result = redactor.apply(ex_red)

        # 편집된 문서를 원본 파일 옆에 저장합니다
        so = SaveOptions()
        so.add_suffix = True
        so.rasterize_to_pdf = False
        so.redacted_file_suffix = "redacted"
        redactor.save(so)

if __name__ == "__main__":
    redact_spreadsheet_content()
```

`sample.xlsx`는 이 예제에서 사용된 샘플 파일입니다. 다운로드하려면 [here](https://docs.groupdocs.com/redaction/python-net/_sample_files/developer-guide/basic-usage/spreadsheet-redactions/sample.xlsx)를 클릭하십시오.

  
```text
Binary file (XLSX, 15 KB)
```
[Download full output](https://docs.groupdocs.com/redaction/python-net/_output_files/developer-guide/basic-usage/spreadsheet-redactions/redact_spreadsheet_content/sample_redacted.xlsx)
