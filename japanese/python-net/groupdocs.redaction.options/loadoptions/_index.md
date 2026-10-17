---
title: "LoadOptions クラス"
second_title: "GroupDocs.Redaction for Python via .NET API リファレンス"
description: "ファイルを開く際に使用されるオプションを提供します。"
type: docs
url: /ja/python-net/groupdocs.redaction.options/loadoptions/
is_root: false
weight: 40
---


## LoadOptions class

ファイルを開く際に使用されるオプションを提供します。

詳細を見る
- [Loading documents](https://docs.groupdocs.com/redaction/net/loading-documents/)
- [Load from local disk](https://docs.groupdocs.com/redaction/net/load-from-local-disc/)
- [Load from stream](https://docs.groupdocs.com/redaction/net/load-from-stream/)
- [Load password-protected document](https://docs.groupdocs.com/redaction/net/load-password-protected-file/)

LoadOptions 型は次のメンバーを公開します:

### コンストラクター
| コンストラクター | 説明 |
| :- | :- |
| [__init__](/redaction/python-net/groupdocs.redaction.options/loadoptions/__init__/) | LoadOptions クラスの新しいインスタンスを初期化します。 |
| [__init__](/redaction/python-net/groupdocs.redaction.options/loadoptions/__init__/#password) | 指定されたパスワードで LoadOptions の新しいインスタンスを初期化します。 |
| [__init__](/redaction/python-net/groupdocs.redaction.options/loadoptions/__init__/#pre_rasterize) | 指定された pre‑rasterization フラグで新しい LoadOptions インスタンスを初期化します。 |
| [__init__](/redaction/python-net/groupdocs.redaction.options/loadoptions/__init__/#password-pre_rasterize) | 指定されたパスワードで新しい LoadOptions インスタンスを初期化します。 |

### プロパティ
| プロパティ | 説明 |
| :- | :- |
| [password](/redaction/python-net/groupdocs.redaction.options/loadoptions/password/) | パスワードで保護されたドキュメントのパスワードです。 |
| [pre_rasterize](/redaction/python-net/groupdocs.redaction.options/loadoptions/pre_rasterize/) | ファイルを事前にラスタライズすべきかを示す pre_rasterize フラグです。 |

### 例

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.options import LoadOptions, SaveOptions
from groupdocs.redaction.redactions import ExactPhraseRedaction, ReplacementOptions

# ドキュメントのパスワードでロードオプションを指定します
load_opt = LoadOptions("mypassword")

# 編集（レダクション）を定義します
repl_opt = ReplacementOptions("[personal]")
ex_red = ExactPhraseRedaction("John Doe", repl_opt)

# パスワードで保護されたドキュメントを開きます
with Redactor("./protected.docx", load_opt) as redactor:
    redactor.apply(ex_red)

    # 編集されたドキュメントを保存します
    save_opt = SaveOptions()
    save_opt.add_suffix = True
    result_path = redactor.save(save_opt)
    print(f"Document redacted successfully. Check output in {result_path}.")
```

### 関連項目
* module [`groupdocs.redaction.options`](/redaction/python-net/groupdocs.redaction.options/)
