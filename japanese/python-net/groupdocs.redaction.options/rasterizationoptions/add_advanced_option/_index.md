---
title: "add_advanced_option メソッド"
second_title: "GroupDocs.Redaction for Python via .NET API リファレンス"
description: "適用する高度なラスター化オプションを登録します。"
type: docs
url: /ja/python-net/groupdocs.redaction.options/rasterizationoptions/add_advanced_option/
is_root: false
weight: 1010
---


## add_advanced_option {#option_type}

適用する高度なラスター化オプションを登録します。

```python
def add_advanced_option(self, option_type):
    ...
```

| パラメーター | タイプ | 説明 |
| :- | :- | :- |
| option_type | `AdvancedRasterizationOptions` | 選択されたエフェクトタイプ（グレースケール、ボーダーなど）に関する情報を提供します。 |

### 例

```python
from groupdocs.redaction.options import SaveOptions, AdvancedRasterizationOptions

so = SaveOptions()
so.rasterization.enabled = True
so.rasterization.add_advanced_option(AdvancedRasterizationOptions.NOISE)
so.rasterization.add_advanced_option(AdvancedRasterizationOptions.GRAYSCALE)
```

## add_advanced_option {#option_type-parameters}

適用する高度なラスター化オプションを登録します。

```python
def add_advanced_option(self, option_type, parameters):
    ...
```

| パラメーター | タイプ | 説明 |
| :- | :- | :- |
| option_type | `AdvancedRasterizationOptions` | 選択されたエフェクトタイプ（グレースケール、ボーダーなど）に関する情報を提供します。 |
| parameters | `dict[str, str]` | 回転角度など、指定されたエフェクトのパラメータです。 |

### 例

```python
from groupdocs.redaction.options import RasterizationOptions, AdvancedRasterizationOptions

ro = RasterizationOptions()
ro.enabled = True
# 組み込みエフェクトを適用する
ro.add_advanced_option(AdvancedRasterizationOptions.NOISE)
ro.add_advanced_option(AdvancedRasterizationOptions.GRAYSCALE)

# カスタム設定でエフェクトを適用します。例：幅 10 ユニットのボーダー
ro.add_advanced_option(
    AdvancedRasterizationOptions.BORDER,
    {"border": "10"}
)
```

### 関連項目
* class [`RasterizationOptions`](/redaction/python-net/groupdocs.redaction.options/rasterizationoptions/)
