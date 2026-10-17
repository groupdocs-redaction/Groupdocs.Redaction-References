---
title: "Metered クラス"
second_title: "GroupDocs.Redaction for Python via .NET API リファレンス"
description: "従量課金（使用量に応じた支払い）ライセンスを管理します。"
type: docs
url: /ja/python-net/groupdocs.redaction/metered/
is_root: false
weight: 80
---


## Metered class

従量課金（使用量に応じた支払い）ライセンスを管理します。

Metered ライセンスは実際の使用量（通常はページまたは
処理されたドキュメント）に基づいて課金されます。公開/非公開キー ペアは一度だけ設定してください
アプリケーションの起動時に設定します。ラッパーは使用状況を GroupDocs に報告します
バックグラウンドでライセンスサーバーへ送信します。

Metered 型は次のメンバーを公開します：

### メソッド
| メソッド | 説明 |
| :- | :- |
| [get_consumption_credit](/redaction/python-net/groupdocs.redaction/metered/get_consumption_credit/) | 現在のキーの残りのメータークレジットを返します。 |
| [get_consumption_quantity](/redaction/python-net/groupdocs.redaction/metered/get_consumption_quantity/) | これまでに消費された合計メーター量を返します。 |
| [set_metered_key](/redaction/python-net/groupdocs.redaction/metered/set_metered_key/#public_key-private_key) | 指定された公開/秘密キーのペアでメーター課金を有効にします。 |

### 関連項目
* module [`groupdocs.redaction`](/redaction/python-net/groupdocs.redaction/)
