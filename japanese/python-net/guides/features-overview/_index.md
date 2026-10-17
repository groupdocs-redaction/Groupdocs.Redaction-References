---
title: "機能概要"
linkTitle: "Features overview"
second_title: "GroupDocs.Redaction for Python via .NET API リファレンス"
description: "GroupDocs.Redaction for Python via .NET は、単一のフォーマット非依存 API を通じて、テキスト、メタデータ、画像領域、アノテーション、ページ全体など、ドキュメントから機密情報を削除し、結果を元の形式またはサニタイズされた PDF として保存します。"
type: docs
url: /ja/python-net/guides/features-overview/
is_root: false
weight: 30
---


GroupDocs.Redaction for Python via .NET は、幅広い [サポートされているドキュメント形式]() にわたって機密情報を削除または永久に隠蔽します。すべての編集は同じワークフローに従います：[`Redactor`](/redaction/python-net/groupdocs.redaction/redactor/) でドキュメントを開き、`apply()` で1つ以上の編集を適用し、`save()` でクリーンアップされた結果を元の形式またはサニタイズされた PDF として保存します。以下の機能は単一のパスで自由に組み合わせて使用できます。

## Text redaction

正確なフレーズまたは正規表現でテキストを検索して置換し、単語全体やメールアドレス、電話番号、国民ID番号などの複雑なパターンもカバーします。マッチしたテキストは置換テキストに置き換えるか、カラーのボックスで覆って元の内容が復元できないようにします。スプレッドシートでは検索範囲を単一のワークシートまたは列に絞ることができます。[Text Redactions]() を参照してください。

## Metadata redaction

文書のメタデータ（作者、タイトル、会社、コメント、画像のEXIFデータ）を消去または書き換えて、機密情報が文書プロパティから漏れないようにします。すべてのメタデータをクリアしたり、特定のフィールドだけを対象にしたり、新しい値に置き換えることができます。[Metadata Redactions]() を参照してください。

## Image-area redaction

埋め込み画像やスキャンページの矩形領域を塗りつぶしボックスで黒く塗りつぶすことで、署名、写真、ヘッダー、フッターなど機密データが表示される可能性のある部分を隠すことができます。[Image Redactions]() を参照してください。

## Annotation redaction

注釈、コメント、ノートを書き換えまたは削除します。すべての注釈を削除するか、正規表現を使用して機密テキストを含むものだけをマッチさせることができます。[Annotation Redactions]() を参照してください。

## Page removal

PDF文書のページ、プレゼンテーションのスライド、スプレッドシートのワークシートを丸ごと削除します。開始ページと削除するページ数、開始点に対する方向を指定します。[Remove Page Redactions]() を参照してください。

## Rasterization to PDF

クリーンアップした文書をページがラスタ画像としてレンダリングされたPDFとして保存します。結果のファイルには検索可能なテキストも元のメタデータも含まれず、削除されたコンテンツは復元できません。第三者に文書を渡す必要がある場合や、PDFを要求する規制に準拠する必要がある場合はラスタライズが適切です。特定のページを選択したり、詳細なラスタライズオプションを通じてPDF/A準拠を要求したりできます。[Save in Rasterized PDF]() と [Advanced Rasterization Options]() を参照してください。

## Redaction policies

複数の赤字処理を再利用可能なポリシーにまとめ、同じルールセットを多数の文書に一貫して適用します。公開前に標準フィールドセットを一括で除去するような繰り返しタスクに最適です。[Use Redaction Policies]() を参照してください。

## Loading and saving

ローカルパスまたはストリームから文書を読み込み、パスワード保護されたファイルにも対応し、必要に応じて赤字処理前に文書を事前にラスタライズできます。保存時には、さらに編集できるように元の形式を保持したり、元ファイルを上書きしたり、PDFにラスタライズしたり、ストリームに書き出したりできます。[Loading Documents]() と [Saving Documents]() を参照してください。

## On-premise

GroupDocs.Redaction for Python via .NET は完全に自社インフラ上で実行され、文書が環境から外部に出ることはありません。パッケージはすべての必要物をバンドルした自己完結型の wheel で、Microsoft Office、OpenOffice、Adobe Acrobat、または別個のランタイムをインストールする必要はありません。[System Requirements]() でサポートされているプラットフォームとネイティブ依存関係を確認してください。
