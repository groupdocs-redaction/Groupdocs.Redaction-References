---
title: "RasterizationOptions クラス"
second_title: "GroupDocs.Redaction for Python via .NET API リファレンス"
description: "ファイルを PDF に変換するためのオプションを提供します。"
type: docs
url: /ja/python-net/groupdocs.redaction.options/rasterizationoptions/
is_root: false
weight: 80
---


## RasterizationOptions class

ファイルを PDF に変換するためのオプションを提供します。

- More details about saving document as a rasterized PDF: https://docs.groupdocs.com/redaction/net/save-in-rasterized-pdf/
- More details about rasterization options: https://docs.groupdocs.com/redaction/net/select-specific-pages-for-rasterized-pdf/

RasterizationOptions 型は次のメンバーを公開します：

### コンストラクター
| コンストラクター | 説明 |
| :- | :- |
| [__init__](/redaction/python-net/groupdocs.redaction.options/rasterizationoptions/__init__/) | 新しいインスタンスを初期化します。 |

### メソッド
| メソッド | 説明 |
| :- | :- |
| [add_advanced_option](/redaction/python-net/groupdocs.redaction.options/rasterizationoptions/add_advanced_option/#option_type) | 適用する高度なラスター化オプションを登録します。 |
| [add_advanced_option](/redaction/python-net/groupdocs.redaction.options/rasterizationoptions/add_advanced_option/#option_type-parameters) | 適用する高度なラスター化オプションを登録します。 |
| [add_advanced_option_advanced_rasterization_options](/redaction/python-net/groupdocs.redaction.options/rasterizationoptions/add_advanced_option_advanced_rasterization_options/) |  |

### プロパティ
| プロパティ | 説明 |
| :- | :- |
| [compliance](/redaction/python-net/groupdocs.redaction.options/rasterizationoptions/compliance/) | The PDF の準拠レベルです。 |
| [enabled](/redaction/python-net/groupdocs.redaction.options/rasterizationoptions/enabled/) | 有効フラグは、ドキュメント内のすべてのページが画像に変換され、単一の PDF ファイルに配置されるかどうかを示します。デフォルトは True です。ラスタライズを回避するには False に設定してください。 |
| [has_advanced_options](/redaction/python-net/groupdocs.redaction.options/rasterizationoptions/has_advanced_options/) | 高度なラスタライズオプションが設定されている場合、インジケータは True です。 |
| [page_count](/redaction/python-net/groupdocs.redaction.options/rasterizationoptions/page_count/) | PDF に変換されるページ数です。 |
| [page_index](/redaction/python-net/groupdocs.redaction.options/rasterizationoptions/page_index/) | PDF に変換する最初のページのインデックス（0 ベース）です。 |

### 例

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.options import RasterizationOptions, PdfComplianceLevel

with Redactor("SomePresentation.pptx") as redactor:
    ro = RasterizationOptions()
    ro.page_index = 0          # first slide
    ro.page_count = 1
    ro.compliance = PdfComplianceLevel.PdfA1a
    redactor.save("PresentationFirstSlide.pdf", ro)
```

### 関連項目
* module [`groupdocs.redaction.options`](/redaction/python-net/groupdocs.redaction.options/)
