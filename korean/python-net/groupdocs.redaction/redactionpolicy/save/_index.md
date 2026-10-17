---
title: "save 메서드"
second_title: "GroupDocs.Redaction for Python via .NET API 참조"
description: "삭제 정책을 파일에 저장합니다."
type: docs
url: /ko/python-net/groupdocs.redaction/redactionpolicy/save/
is_root: false
weight: 1060
---


## save {#file_path}

삭제 정책을 파일에 저장합니다.

```python
def save(self, file_path):
    ...
```

| 매개변수 | 유형 | 설명 |
| :- | :- | :- |
| file_path | `str` | 파일 경로. |

### 예제

```python
    policy = RedactionPolicy([
        ExactPhraseRedaction("ACME", ReplacementOptions("[CO]")),
        RegexRedaction(r"\d{2,}", ReplacementOptions("[NUM]")),
    ])
    policy.save("./sample_policy.xml")
    ```

## save {#output}

삭제 정책을 스트림에 저장합니다.

```python
def save(self, output):
    ...
```

| 매개변수 | 유형 | 설명 |
| :- | :- | :- |
| output | `io.RawIOBase` | 정책을 저장할 대상 스트림. |

**Returns:** None.

### 또 보기
* class [`RedactionPolicy`](/redaction/python-net/groupdocs.redaction/redactionpolicy/)
