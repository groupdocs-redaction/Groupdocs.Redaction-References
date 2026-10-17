---
title: "텍스트 레드액션"
linkTitle: "Text redaction"
second_title: "GroupDocs.Redaction for Python via .NET API 참조"
description: "이 문서는 Python 레드액션 API를 사용하여 문서에서 민감하거나 개인적인 데이터를 쉽게 레드액션하는 방법을 설명합니다. PDF, DOC, DOCX, PPT, PPTX, XLS, XLSX 등 다양한 형식의 문서에 대해 정확한 구문이나 정규식을 사용하여 텍스트 레드액션을 적용할 수 있습니다."
type: docs
url: /ko/python-net/guides/text-redactions/
is_root: false
weight: 50
---


GroupDocs.Redaction을 사용하면 문서에서 민감하거나 개인적인 데이터를 쉽게 레드액션할 수 있습니다. 가장 일반적인 레드액션 사례는 문서에서 텍스트를 제거하는 것입니다.

GroupDocs.Redaction API를 사용하면 PDF, DOC, DOCX, PPT, PPTX, XLS, XLSX 등 다양한 형식의 문서에 대해 정확한 구문이나 [정규식](https://docs.microsoft.com/en-us/dotnet/standard/base-types/regular-expressions)을 사용하여 텍스트 레드액션을 적용할 수 있습니다. 전체 목록은 [지원되는 문서 형식]() 기사에서 확인하십시오.

## Use exact phrase redaction

아래 예제에서는 텍스트 레드액션을 적용하여 개인 정확 구문 "John Doe"를 "\\[personal\\]"(또는 다른 면제 코드)로 교체합니다:

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.options import SaveOptions
from groupdocs.redaction.redactions import ExactPhraseRedaction, ReplacementOptions

def redact_exact_phrase():
    # 편집 옵션을 지정합니다
    repl_opt = ReplacementOptions("[personal]")
    ex_red = ExactPhraseRedaction("John Doe", repl_opt)

    # 레드랙션할 문서를 로드합니다
    with Redactor("./sample.docx") as redactor:
        # 가리기를 적용합니다
        result = redactor.apply(ex_red)

        # 편집된 문서를 원본 파일 옆에 저장합니다
        so = SaveOptions()
        so.add_suffix = True
        so.rasterize_to_pdf = False
        so.redacted_file_suffix = "redacted"
        redactor.save(so)

if __name__ == "__main__":
    redact_exact_phrase()
```

`sample.docx`는 이 예제에 사용된 샘플 파일입니다. 다운로드하려면 [여기](https://docs.groupdocs.com/redaction/python-net/_sample_files/developer-guide/basic-usage/text-redactions/sample.docx)를 클릭하십시오.

  
```text
Binary file (DOCX, 16 KB)
```
[Download full output](https://docs.groupdocs.com/redaction/python-net/_output_files/developer-guide/basic-usage/text-redactions/redact_exact_phrase/sample_redacted.docx)

기본적으로 정확한 구문 검색은 대소문자를 구분하지 않습니다. 대소문자를 구분하는 레드액션을 위해서는 생성자 매개변수와 해당 공개 속성이 있습니다:

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.options import SaveOptions
from groupdocs.redaction.redactions import ExactPhraseRedaction, ReplacementOptions

def redact_case_sensitive_phrase():
    # 대소문자 구분 매칭 활성화
    case_sensitive = True

    # 편집 옵션을 지정합니다
    repl_opt = ReplacementOptions("[personal]")
    ex_red = ExactPhraseRedaction("John Doe", case_sensitive, repl_opt)

    # 레드랙션할 문서를 로드합니다
    with Redactor("./sample.docx") as redactor:
        # 가리기를 적용합니다
        result = redactor.apply(ex_red)

        # 편집된 문서를 원본 파일 옆에 저장합니다
        so = SaveOptions()
        so.add_suffix = True
        so.rasterize_to_pdf = False
        so.redacted_file_suffix = "redacted"
        redactor.save(so)

if __name__ == "__main__":
    redact_case_sensitive_phrase()
```

`sample.docx`는 이 예제에 사용된 샘플 파일입니다. 다운로드하려면 [여기](https://docs.groupdocs.com/redaction/python-net/_sample_files/developer-guide/basic-usage/text-redactions/sample.docx)를 클릭하십시오.

  
```text
Binary file (DOCX, 16 KB)
```
[Download full output](https://docs.groupdocs.com/redaction/python-net/_output_files/developer-guide/basic-usage/text-redactions/redact_case_sensitive_phrase/sample_redacted.docx)

레드액션된 텍스트 위에 색상 상자를 표시해야 하는 경우, 교체 문자열 대신 색상을 사용할 수 있습니다. 레드액션은 일치하는 텍스트를 삭제하고 지정된 색상의 사각형을 레드액션된 텍스트 위치에 삽입합니다:

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.options import SaveOptions
from groupdocs.redaction.redactions import ExactPhraseRedaction, ReplacementOptions
from groupdocs.pydrawing import Color

def redact_with_color_box():
    # 레드액션 상자의 색상 정의
    color = Color.from_argb(255, 220, 20, 60)

    # 편집 옵션을 지정합니다
    repl_opt = ReplacementOptions(color)
    ex_red = ExactPhraseRedaction("John Doe", repl_opt)

    # 레드랙션할 문서를 로드합니다
    with Redactor("./sample.docx") as redactor:
        # 가리기를 적용합니다
        result = redactor.apply(ex_red)

        # 편집된 문서를 원본 파일 옆에 저장합니다
        so = SaveOptions()
        so.add_suffix = True
        so.rasterize_to_pdf = False
        so.redacted_file_suffix = "redacted"
        redactor.save(so)

if __name__ == "__main__":
    redact_with_color_box()
```

`sample.docx`는 이 예제에 사용된 샘플 파일입니다. 다운로드하려면 [여기](https://docs.groupdocs.com/redaction/python-net/_sample_files/developer-guide/basic-usage/text-redactions/sample.docx)를 클릭하십시오.

  
```text
Binary file (DOCX, 17 KB)
```
[Download full output](https://docs.groupdocs.com/redaction/python-net/_output_files/developer-guide/basic-usage/text-redactions/redact_with_color_box/sample_redacted.docx)

아랍어 또는 히브리어와 같이 오른쪽에서 왼쪽으로 쓰는 문서에 레드액션을 적용해야 할 수도 있습니다. 다음 예제는 Arabic PDF 문서에 ExactPhraseRedaction을 적용하는 방법을 보여줍니다:

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.options import SaveOptions
from groupdocs.redaction.redactions import ExactPhraseRedaction, ReplacementOptions

def redact_right_to_left_text():
    # 아랍어 구문으로 레드액션 옵션 지정
    repl_opt = ReplacementOptions("[test]")
    ex_red = ExactPhraseRedaction("انتقد", repl_opt)

    # 레드랙션할 문서를 로드합니다
    with Redactor("./arabic.pdf") as redactor:
        # 가리기를 적용합니다
        result = redactor.apply(ex_red)

        # 편집된 문서를 원본 파일 옆에 저장합니다
        so = SaveOptions()
        so.add_suffix = True
        so.rasterize_to_pdf = False
        so.redacted_file_suffix = "redacted"
        redactor.save(so)

if __name__ == "__main__":
    redact_right_to_left_text()
```

`arabic.pdf`는 이 예제에서 사용된 샘플 파일입니다. 다운로드하려면 [here](https://docs.groupdocs.com/redaction/python-net/_sample_files/developer-guide/basic-usage/text-redactions/arabic.pdf) 를 클릭하십시오.

  
```text
Binary file (PDF, 23 KB)
```
[Download full output](https://docs.groupdocs.com/redaction/python-net/_output_files/developer-guide/basic-usage/text-redactions/redact_right_to_left_text/arabic_redacted.pdf)

## Use regular expression

내부적으로 "exact phrase" 레드액션은 정규식을 통해 작동하며, 이는 레드액션의 기본 접근 방식입니다. 아래 예제에서는 "2 digits, space or nothing, 2 digits, again space and 6 digits"와 일치하는 모든 텍스트를 파란색 상자로 레드액션합니다:

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.options import SaveOptions
from groupdocs.redaction.redactions import RegexRedaction, ReplacementOptions
from groupdocs.pydrawing import Color

def redact_with_regex():
    # 레드액션 상자의 색상 정의
    color = Color.from_argb(255, 220, 20, 60)

    # 편집 옵션을 지정합니다
    repl_opt = ReplacementOptions(color)
    reg_red = RegexRedaction("\\d{2}\\s*\\d{2}[^\\d]*\\d{6}", repl_opt)

    # 레드랙션할 문서를 로드합니다
    with Redactor("./sample.docx") as redactor:
        # 가리기를 적용합니다
        result = redactor.apply(reg_red)

        # 편집된 문서를 원본 파일 옆에 저장합니다
        so = SaveOptions()
        so.add_suffix = True
        so.rasterize_to_pdf = False
        so.redacted_file_suffix = "redacted"
        redactor.save(so)

if __name__ == "__main__":
    redact_with_regex()
```

`sample.docx`는 이 예제에 사용된 샘플 파일입니다. 다운로드하려면 [여기](https://docs.groupdocs.com/redaction/python-net/_sample_files/developer-guide/basic-usage/text-redactions/sample.docx)를 클릭하십시오.

  
```text
Binary file (DOCX, 16 KB)
```
[Download full output](https://docs.groupdocs.com/redaction/python-net/_output_files/developer-guide/basic-usage/text-redactions/redact_with_regex/sample_redacted.docx)

전체 단락을 레드액션해야 하는 경우, RegexRedaction을 사용해야 할 수도 있습니다. 다음 예제는 PDF 문서에서 전체 단락을 레드액션하는 방법을 보여줍니다:

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.options import SaveOptions
from groupdocs.redaction.redactions import RegexRedaction, ReplacementOptions
from groupdocs.pydrawing import Color

def redact_whole_paragraph():
    # 레드액션 상자의 색상 정의
    color = Color.from_argb(255, 220, 20, 60)

    # 전체 단락과 일치하는 레드액션 옵션 지정
    repl_opt = ReplacementOptions(color)
    reg_red = RegexRedaction("(Lorem(\n|.)+?urna)", repl_opt)

    # 레드랙션할 문서를 로드합니다
    with Redactor("./sample.pdf") as redactor:
        # 가리기를 적용합니다
        result = redactor.apply(reg_red)

        # 편집된 문서를 원본 파일 옆에 저장합니다
        so = SaveOptions()
        so.add_suffix = True
        so.rasterize_to_pdf = False
        so.redacted_file_suffix = "redacted"
        redactor.save(so)

if __name__ == "__main__":
    redact_whole_paragraph()
```

`sample.pdf`는 이 예제에서 사용된 샘플 파일입니다. 다운로드하려면 [here](https://docs.groupdocs.com/redaction/python-net/_sample_files/developer-guide/basic-usage/text-redactions/sample.pdf) 를 클릭하십시오.

  
```text
Binary file (PDF, 68 KB)
```
[Download full output](https://docs.groupdocs.com/redaction/python-net/_output_files/developer-guide/basic-usage/text-redactions/redact_whole_paragraph/sample_redacted.pdf)
