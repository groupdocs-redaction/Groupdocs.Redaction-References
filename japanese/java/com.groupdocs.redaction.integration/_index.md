---
title: "com.groupdocs.redaction.integration"
second_title: "GroupDocs.Redaction for Java API Reference"
description: "このパッケージは、さまざまな形式のドキュメントを GroupDocs.Redactions と統合するために使用されるインターフェイスとクラスを提供します。"
type: docs
weight: 13
url: /ja/java/com.groupdocs.redaction.integration/
---

このパッケージは、さまざまな形式のドキュメントを GroupDocs.Redactions と統合するために使用されるインターフェイスとクラスを提供します。



## クラス

| クラス | 説明 |
| --- | --- |
| [DocumentFormatInstance](../com.groupdocs.redaction.integration/documentformatinstance) | ドキュメントの特定の形式を表します。 |
| [MetadataCollection](../com.groupdocs.redaction.integration/metadatacollection) | MetadataItem の辞書を、タイトルをキーとして表します。 |
| [MetadataItem](../com.groupdocs.redaction.integration/metadataitem) | すべてのサポート対象フォーマットで共通のメタデータ項目を表し、メタデータの編集に使用されます。 |
| [RecognizedImage](../com.groupdocs.redaction.integration/recognizedimage) | 画像から認識プロセスの結果として抽出されたテキストを表します。 |
| [RedactableImage](../com.groupdocs.redaction.integration/redactableimage) | すべてのラスター画像編集操作へのファサードを提供します。 |
| [TextFragment](../com.groupdocs.redaction.integration/textfragment) | OCR エンジンによって抽出された、認識されたテキスト（単語、記号など）の一部を表します。 |
| [TextLine](../com.groupdocs.redaction.integration/textline) | OCR エンジンが画像から抽出したテキストの行を表します。 |

## インターフェイス

| インターフェイス | 説明 |
| --- | --- |
| [IAnnotatedDocument](../com.groupdocs.redaction.integration/iannotateddocument) | コメントなどのアノテーションへのアクセスに必要なメソッドを定義します。 |
| [ICellularFormatInstance](../com.groupdocs.redaction.integration/icellularformatinstance) | 1 つまたは複数のワークシートを持つスプレッドシート形式へのアクセスに必要なメソッドを定義します。 |
| [IFixedFormatDocument](../com.groupdocs.redaction.integration/ifixedformatdocument) | PDF やプレゼンテーションなど、固定構造の形式へのアクセスに必要なメソッドを定義します。 |
| [IImageFormatInstance](../com.groupdocs.redaction.integration/iimageformatinstance) | ラスター画像形式の編集に必要なメソッドを定義します。 |
| [IMetadataAccess](../com.groupdocs.redaction.integration/imetadataaccess) | 形式がサポートしている場合、ドキュメントのメタデータへのアクセスに必要なメソッドを定義します。 |
| [IMultipleAreaRedactable](../com.groupdocs.redaction.integration/imultiplearearedactable) | 同じ色で複数の画像領域を一度に編集するために必要なメソッドを定義します。 |
| [IOcrConnector](../com.groupdocs.redaction.integration/iocrconnector) | 画像ドキュメントおよび埋め込み画像にテキスト編集を適用するために必要なメソッドを定義します。 |
| [IPaginatedDocument](../com.groupdocs.redaction.integration/ipaginateddocument) | ドキュメントのページを操作するために必要なメソッドを定義します。 |
| [IPreviewable](../com.groupdocs.redaction.integration/ipreviewable) | ドキュメントのプレビューを作成するメソッドを定義します。 |
| [IRasterizableDocument](../com.groupdocs.redaction.integration/irasterizabledocument) | 任意のバイナリ形式でドキュメントを保存するために必要なメソッドを定義します。 |
| [ITextualFormatInstance](../com.groupdocs.redaction.integration/itextualformatinstance) | テキストを含む任意のドキュメントのテキストデータを編集するために必要なメソッドを定義します。 |
