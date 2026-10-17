---
title: "rasterize 메서드"
second_title: "GroupDocs.Redaction for Python via .NET API 참조"
description: "문서를 PDF 형식으로 스트림에 저장합니다."
type: docs
url: /ko/python-net/groupdocs.redaction.integration/irasterizabledocument/rasterize/
is_root: false
weight: 1010
---


## rasterize {#output}

문서를 PDF 형식으로 스트림에 저장합니다.

```python
def rasterize(self, output):
    ...
```

| 매개변수 | 유형 | 설명 |
| :- | :- | :- |
| output | `io.RawIOBase` | 대상 스트림. |

## rasterize {#output-options}

문서를 페이지 범위 및 규격 옵션과 함께 PDF 형식으로 스트림에 저장합니다.

```python
def rasterize(self, output, options):
    ...
```

| 매개변수 | 유형 | 설명 |
| :- | :- | :- |
| output | `io.RawIOBase` | 대상 스트림. |
| options | `RasterizationOptions` | PDF 변환 옵션. |

### 또 보기
* class [`IRasterizableDocument`](/redaction/python-net/groupdocs.redaction.integration/irasterizabledocument/)
