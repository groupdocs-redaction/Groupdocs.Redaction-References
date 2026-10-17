---
title: "__init__ コンストラクタ"
second_title: "GroupDocs.Redaction for Python via .NET API リファレンス"
description: "LoadOptions クラスの新しいインスタンスを初期化します。"
type: docs
url: /ja/python-net/groupdocs.redaction.options/loadoptions/__init__/
is_root: false
weight: 10
---


## __init__

LoadOptions クラスの新しいインスタンスを初期化します。

```python
def __init__(self):
    ...
```

## __init__ {#password}

指定されたパスワードで LoadOptions の新しいインスタンスを初期化します。

```python
def __init__(self, password):
    ...
```

| パラメーター | タイプ | 説明 |
| :- | :- | :- |
| password | `str` | 保護されたファイルのパスワードです。 |

### 例

```python
    from groupdocs.redaction.options import LoadOptions

    # パスワードで保護されたドキュメントを読み込む
    load_opt = LoadOptions("mypassword")
    ```

## __init__ {#pre_rasterize}

指定された pre‑rasterization フラグで新しい LoadOptions インスタンスを初期化します。

```python
def __init__(self, pre_rasterize):
    ...
```

| パラメーター | タイプ | 説明 |
| :- | :- | :- |
| pre_rasterize | `bool` | True の場合、読み込み時にラスタライズを強制します。 |

## __init__ {#password-pre_rasterize}

指定されたパスワードで新しい LoadOptions インスタンスを初期化します。

`pre_rasterize` が True の場合、ドキュメントが読み込まれるときにラスタライズが強制されます。

```python
def __init__(self, password, pre_rasterize):
    ...
```

| パラメーター | タイプ | 説明 |
| :- | :- | :- |
| password | `str` | 保護されたファイルのパスワードです。 |
| pre_rasterize | `bool` | True の場合、読み込み時にラスタライズを強制します。 |

### 例

```python
from groupdocs.redaction.options import LoadOptions

# パスワードで保護されたドキュメントを読み込む
load_opt = LoadOptions("mypassword")
```

### 関連項目
* class [`LoadOptions`](/redaction/python-net/groupdocs.redaction.options/loadoptions/)
