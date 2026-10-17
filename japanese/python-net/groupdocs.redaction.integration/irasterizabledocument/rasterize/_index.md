---
title: "rasterize メソッド"
second_title: "GroupDocs.Redaction for Python via .NET API リファレンス"
description: "ドキュメントを PDF としてストリームに保存します。"
type: docs
url: /ja/python-net/groupdocs.redaction.integration/irasterizabledocument/rasterize/
is_root: false
weight: 1010
---


## rasterize {#output}

ドキュメントを PDF としてストリームに保存します。

```python
def rasterize(self, output):
    ...
```

| パラメーター | タイプ | 説明 |
| :- | :- | :- |
| output | `io.RawIOBase` | 対象ストリーム。 |

## rasterize {#output-options}

ページ範囲と準拠オプションを指定して、ドキュメントを PDF としてストリームに保存します。

```python
def rasterize(self, output, options):
    ...
```

| パラメーター | タイプ | 説明 |
| :- | :- | :- |
| output | `io.RawIOBase` | 対象ストリーム。 |
| options | `RasterizationOptions` | PDF 変換オプション。 |

### 関連項目
* class [`IRasterizableDocument`](/redaction/python-net/groupdocs.redaction.integration/irasterizabledocument/)
