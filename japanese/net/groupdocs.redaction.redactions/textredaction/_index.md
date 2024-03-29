---
title: TextRedaction
second_title: GroupDocs.Redaction for .NET API リファレンス
description: ドキュメント テキスト編集の基本抽象クラスを表します
type: docs
weight: 640
url: /ja/net/groupdocs.redaction.redactions/textredaction/
---
## TextRedaction class

ドキュメント テキスト編集の基本抽象クラスを表します。

```csharp
public abstract class TextRedaction : Redaction
```

## プロパティ

| 名前 | 説明 |
| --- | --- |
| [ActionOptions](../../groupdocs.redaction.redactions/textredaction/actionoptions) { get; } | を取得します[`ReplacementOptions`](../replacementoptions)インスタンス、テキスト置換のタイプを指定します. |
| virtual [Description](../../groupdocs.redaction/redaction/description) { get; } | リダクションとそのパラメーターを説明する文字列を返します。 |
| [OcrConnector](../../groupdocs.redaction.redactions/textredaction/ocrconnector) { get; set; } | を取得または設定します[`IOcrConnector`](../../groupdocs.redaction.integration.ocr/iocrconnector)グラフィックコンテンツからテキストを抽出するために必要な実装. |

## メソッド

| 名前 | 説明 |
| --- | --- |
| abstract [ApplyTo](../../groupdocs.redaction/redaction/applyto)(DocumentFormatInstance) | 特定のフォーマット インスタンスにリダクションを適用します。 |

### 備考

**もっと詳しく知る**

* リダクションの適用に関する詳細: [リダクションの基本](https://docs.groupdocs.com/redaction/net/redaction-basics/)
* ドキュメント テキストの編集に関する詳細: [テキスト編集](https://docs.groupdocs.com/redaction/net/text-redactions/)

### 関連項目

* class [Redaction](../../groupdocs.redaction/redaction)
* 名前空間 [GroupDocs.Redaction.Redactions](../../groupdocs.redaction.redactions)
* 組み立て [GroupDocs.Redaction](../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Redaction.dll -->
