---
title: "LoadOptions 클래스"
second_title: "GroupDocs.Redaction for Python via .NET API 참조"
description: "파일을 열 때 사용할 옵션을 제공합니다."
type: docs
url: /ko/python-net/groupdocs.redaction.options/loadoptions/
is_root: false
weight: 40
---


## LoadOptions class

파일을 열 때 사용할 옵션을 제공합니다.

자세히 알아보기
- [Loading documents](https://docs.groupdocs.com/redaction/net/loading-documents/)
- [Load from local disk](https://docs.groupdocs.com/redaction/net/load-from-local-disc/)
- [Load from stream](https://docs.groupdocs.com/redaction/net/load-from-stream/)
- [Load password-protected document](https://docs.groupdocs.com/redaction/net/load-password-protected-file/)

LoadOptions 유형은 다음 멤버를 노출합니다:

### 생성자
| 생성자 | 설명 |
| :- | :- |
| [__init__](/redaction/python-net/groupdocs.redaction.options/loadoptions/__init__/) | LoadOptions 클래스의 새 인스턴스를 초기화합니다. |
| [__init__](/redaction/python-net/groupdocs.redaction.options/loadoptions/__init__/#password) | 지정된 비밀번호로 LoadOptions의 새 인스턴스를 초기화합니다. |
| [__init__](/redaction/python-net/groupdocs.redaction.options/loadoptions/__init__/#pre_rasterize) | 지정된 pre‑rasterization 플래그로 새로운 LoadOptions 인스턴스를 초기화합니다. |
| [__init__](/redaction/python-net/groupdocs.redaction.options/loadoptions/__init__/#password-pre_rasterize) | 지정된 비밀번호로 새로운 LoadOptions 인스턴스를 초기화합니다. |

### 속성
| 속성 | 설명 |
| :- | :- |
| [password](/redaction/python-net/groupdocs.redaction.options/loadoptions/password/) | 암호로 보호된 문서의 비밀번호. |
| [pre_rasterize](/redaction/python-net/groupdocs.redaction.options/loadoptions/pre_rasterize/) | 파일을 사전 래스터화할지 여부를 나타내는 pre_rasterize 플래그입니다. |

### 예제

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.options import LoadOptions, SaveOptions
from groupdocs.redaction.redactions import ExactPhraseRedaction, ReplacementOptions

# 문서 비밀번호로 로드 옵션을 지정합니다
load_opt = LoadOptions("mypassword")

# 레다션을 정의합니다
repl_opt = ReplacementOptions("[personal]")
ex_red = ExactPhraseRedaction("John Doe", repl_opt)

# 비밀번호로 보호된 문서를 엽니다
with Redactor("./protected.docx", load_opt) as redactor:
    redactor.apply(ex_red)

    # 레다션된 문서를 저장합니다
    save_opt = SaveOptions()
    save_opt.add_suffix = True
    result_path = redactor.save(save_opt)
    print(f"Document redacted successfully. Check output in {result_path}.")
```

### 또 보기
* module [`groupdocs.redaction.options`](/redaction/python-net/groupdocs.redaction.options/)
