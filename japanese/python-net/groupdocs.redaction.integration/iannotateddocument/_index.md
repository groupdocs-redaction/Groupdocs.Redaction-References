---
title: "IAnnotatedDocument クラス"
second_title: "GroupDocs.Redaction for Python via .NET API リファレンス"
description: "コメントなどの注釈にアクセスするために必要なメソッドを定義し、注釈の削除を実行するために DocumentFormatInstance 派生クラスで実装する必要があります。"
type: docs
url: /ja/python-net/groupdocs.redaction.integration/iannotateddocument/
is_root: false
weight: 20
---


## IAnnotatedDocument class

コメントなどのアノテーションにアクセスするために必要なメソッドを定義し、アノテーションの編集を実行するために [`DocumentFormatInstance`](/redaction/python-net/groupdocs.redaction.integration/documentformatinstance/)-派生クラスで実装する必要があります。

詳しく読む：
- More details about applying redactions: https://docs.groupdocs.com/redaction/net/redaction-basics/
- More details about document annotation redactions: https://docs.groupdocs.com/redaction/net/annotation-redactions/
- More details about implementing custom formats: https://docs.groupdocs.com/redaction/net/create-custom-format-handler/

IAnnotatedDocument 型は次のメンバーを公開します:

### メソッド
| メソッド | 説明 |
| :- | :- |
| [delete_annotations](/redaction/python-net/groupdocs.redaction.integration/iannotateddocument/delete_annotations/#regular_expression) | ドキュメント内で正規表現に一致するすべての注釈を削除します。 |
| [delete_annotations_regex](/redaction/python-net/groupdocs.redaction.integration/iannotateddocument/delete_annotations_regex/) |  |
| [redact_annotation](/redaction/python-net/groupdocs.redaction.integration/iannotateddocument/redact_annotation/#regular_expression-replacement) | ドキュメント内のすべての注釈で一致するテキストを置換します。 |
| [redact_annotation_file](/redaction/python-net/groupdocs.redaction.integration/iannotateddocument/redact_annotation_file/) |  |
| [redact_annotation_regex](/redaction/python-net/groupdocs.redaction.integration/iannotateddocument/redact_annotation_regex/) |  |
| [redact_annotation_string](/redaction/python-net/groupdocs.redaction.integration/iannotateddocument/redact_annotation_string/) |  |

### 関連項目
* module [`groupdocs.redaction.integration`](/redaction/python-net/groupdocs.redaction.integration/)
