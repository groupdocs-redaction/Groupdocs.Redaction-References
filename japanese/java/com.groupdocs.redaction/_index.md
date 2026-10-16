---
title: "com.groupdocs.redaction"
second_title: "GroupDocs.Redaction for Java API Reference"
description: "このパッケージは、PDF ラスター画像および Office ドキュメント形式のドキュメントから機密情報を編集するためのクラスを提供します。"
type: docs
weight: 10
url: /ja/java/com.groupdocs.redaction/
---

このパッケージは、PDF、ラスタ画像、オフィス文書形式のドキュメントから機密情報を編集（赤字）するためのクラスを提供します。

このパッケージの主なクラスは次のとおりです：

<br />

* [Redactor](../../com.groupdocs.redaction/redactor) is the entry point for redaction process.
* [Redaction](../../com.groupdocs.redaction/redaction) is abstract base class for all types of document redactions.
* [RedactionPolicy](../../com.groupdocs.redaction/redactionpolicy) is pre-configured in XML set of redaction rules.
* [RedactorChangeLog](../../com.groupdocs.redaction/redactorchangelog) provides information about redaction process results.

<br />




## クラス

| クラス | 説明 |
| --- | --- |
| [DocumentInfo](../com.groupdocs.redaction/documentinfo) | ドキュメントに関する情報を表します。 |
| [FileType](../com.groupdocs.redaction/filetype) | ファイルタイプを表します。 |
| [PageInfo](../com.groupdocs.redaction/pageinfo) | 簡潔なページ情報を表します。 |
| [Redaction](../com.groupdocs.redaction/redaction) | すべての編集タイプの基底抽象クラスを表します。 |
| [RedactionPolicy](../com.groupdocs.redaction/redactionpolicy) | 適用する特定の編集のセットを含むサニタイズポリシーを表します。 |
| [RedactionResult](../com.groupdocs.redaction/redactionresult) | 編集操作の結果を表します。 |
| [Redactor](../com.groupdocs.redaction/redactor) | ドキュメントの編集プロセスを制御し、開く、編集する、保存することを可能にするメインクラスを表します。 |
| [RedactorChangeLog](../com.groupdocs.redaction/redactorchangelog) | Redactor クラスの Apply() メソッドに渡される編集リストの結果を表します。 |
| [RedactorLogEntry](../com.groupdocs.redaction/redactorlogentry) | 編集適用の結果を表します。 |

## インターフェイス

| インターフェイス | 説明 |
| --- | --- |
| [IDocumentInfo](../com.groupdocs.redaction/idocumentinfo) | 基本的なドキュメント情報を取得するために必要なメソッドを定義します。 |

## 列挙型

| 列挙型 | 説明 |
| --- | --- |
| [RedactionStatus](../com.groupdocs.redaction/redactionstatus) | 編集完了ステータスを表します。 |
