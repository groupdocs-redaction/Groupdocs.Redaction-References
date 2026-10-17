---
title: "recognize yöntemi"
second_title: "GroupDocs.Redaction for Python via .NET API Referansları"
description: "Akış olarak sağlanan bir görüntünün OCR işleme işlemini gerçekleştirir."
type: docs
url: /tr/python-net/groupdocs.redaction.integration.ocr/iocrconnector/recognize/
is_root: false
weight: 1010
---


## recognize {#image_stream}

Akış olarak sağlanan bir görüntünün OCR işleme işlemini gerçekleştirir.

```python
def recognize(self, image_stream):
    ...
```

| Parametre | [ExactPhraseRedaction](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction.redactions/exactphraseredaction/), [RegexRedaction](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction.redactions/regexredaction/) | Açıklama |
| :- | :- | :- |
| image_stream | `io.RawIOBase` | İşlenecek bir görüntüyü içeren akış. |

**Returns:** Structured recognized text, containing lines, words and their bounding rectangles.

### Ayrıca Bakınız
* class [`IOcrConnector`](/redaction/python-net/groupdocs.redaction.integration.ocr/iocrconnector/)
