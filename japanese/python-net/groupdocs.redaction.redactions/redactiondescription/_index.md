---
title: "RedactionDescription クラス"
second_title: "GroupDocs.Redaction for Python via .NET API リファレンス"
description: "赤字処理中に実行された単一の変更アクション情報を表します。"
type: docs
url: /ja/python-net/groupdocs.redaction.redactions/redactiondescription/
is_root: false
weight: 200
---


## RedactionDescription class

赤字処理中に実行された単一の変更アクション情報を表します。

詳細を見る

- More details about [`RedactionDescription`](/redaction/python-net/groupdocs.redaction.redactions/redactiondescription/) class and [`IRedactionCallback`](/redaction/python-net/groupdocs.redaction.redactions/iredactioncallback/) interface: Use redaction callback https://docs.groupdocs.com/redaction/net/use-redaction-callback/

RedactionDescription 型は次のメンバーを公開します：

### コンストラクター
| コンストラクター | 説明 |
| :- | :- |
| [__init__](/redaction/python-net/groupdocs.redaction.redactions/redactiondescription/__init__/#redaction_type-action_type-original_text) | 置換情報なしで RedactionDescription クラスの新しいインスタンスを初期化します。 |
| [__init__](/redaction/python-net/groupdocs.redaction.redactions/redactiondescription/__init__/#redaction_type-action_type-original_text-replacement) | 置換情報付きで RedactionDescription クラスの新しいインスタンスを初期化します。 |
| [__init__](/redaction/python-net/groupdocs.redaction.redactions/redactiondescription/__init__/#redaction_type-action_type-image_area_replacement-image_details) | 画像領域の置換情報を使用して新しい RedactionDescription を初期化します。 |

### プロパティ
| プロパティ | 説明 |
| :- | :- |
| [action_type](/redaction/python-net/groupdocs.redaction.redactions/redactiondescription/action_type/) | 赤字処理の操作：置換、クリーンアップ、または削除。 |
| [details](/redaction/python-net/groupdocs.redaction.redactions/redactiondescription/details/) | 赤字対象項目のオプションの詳細情報です。 |
| [image_area_replacement](/redaction/python-net/groupdocs.redaction.redactions/redactiondescription/image_area_replacement/) | 画像領域の赤字処理の置換情報、テキストの赤字処理の場合は None です。 |
| [original_text](/redaction/python-net/groupdocs.redaction.redactions/redactiondescription/original_text/) | 式が提供されている場合の一致したテキストです。 |
| [redaction_type](/redaction/python-net/groupdocs.redaction.redactions/redactiondescription/redaction_type/) | ドキュメントデータのタイプ – テキスト、メタデータ、または注釈です。 |
| [replacement](/redaction/python-net/groupdocs.redaction.redactions/redactiondescription/replacement/) | 置換情報です。None の場合があります。 |

### 関連項目
* module [`groupdocs.redaction.redactions`](/redaction/python-net/groupdocs.redaction.redactions/)
