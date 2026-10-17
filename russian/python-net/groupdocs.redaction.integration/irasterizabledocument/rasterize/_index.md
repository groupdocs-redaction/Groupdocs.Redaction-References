---
title: "метод rasterize"
second_title: "GroupDocs.Redaction для Python через .NET справочник API"
description: "Сохраняет документ в поток в формате PDF."
type: docs
url: /ru/python-net/groupdocs.redaction.integration/irasterizabledocument/rasterize/
is_root: false
weight: 1010
---


## rasterize {#output}

Сохраняет документ в поток в формате PDF.

```python
def rasterize(self, output):
    ...
```

| Параметр | Тип | Описание |
| :- | :- | :- |
| output | `io.RawIOBase` | Целевой поток. |

## rasterize {#output-options}

Сохраняет документ в поток в формате PDF с диапазоном страниц и параметрами соответствия.

```python
def rasterize(self, output, options):
    ...
```

| Параметр | Тип | Описание |
| :- | :- | :- |
| output | `io.RawIOBase` | Целевой поток. |
| options | `RasterizationOptions` | Параметры конвертации PDF. |

### См. также
* class [`IRasterizableDocument`](/redaction/python-net/groupdocs.redaction.integration/irasterizabledocument/)
