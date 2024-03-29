---
title: AnnotationRedaction
second_title: GroupDocs.Redaction for .NET API リファレンス
description: 指定された正規表現に一致する注釈テキスト コメントなど を置き換えるリダクションを表します
type: docs
weight: 440
url: /ja/net/groupdocs.redaction.redactions/annotationredaction/
---
## AnnotationRedaction class

指定された正規表現に一致する注釈テキスト (コメントなど) を置き換えるリダクションを表します。

```csharp
public class AnnotationRedaction : Redaction
```

## コンストラクター

| 名前 | 説明 |
| --- | --- |
| [AnnotationRedaction](annotationredaction#constructor_1)(Regex, string) | AnnotationRedaction クラスの新しいインスタンスを初期化します。 |
| [AnnotationRedaction](annotationredaction#constructor)(string, string) | AnnotationRedaction クラスの新しいインスタンスを初期化します。 |

## プロパティ

| 名前 | 説明 |
| --- | --- |
| override [Description](../../groupdocs.redaction.redactions/annotationredaction/description) { get; } | リダクションとそのパラメーターを説明する文字列を返します。 |
| [Expression](../../groupdocs.redaction.redactions/annotationredaction/expression) { get; } | 一致する正規表現を取得します。 |
| [Replacement](../../groupdocs.redaction.redactions/annotationredaction/replacement) { get; } | 一致したテキストのテキスト置換を取得します。 |

## メソッド

| 名前 | 説明 |
| --- | --- |
| override [ApplyTo](../../groupdocs.redaction.redactions/annotationredaction/applyto)(DocumentFormatInstance) | 特定のフォーマット インスタンスにリダクションを適用します。 |

### 備考

**もっと詳しく知る**

* リダクションの適用に関する詳細: [リダクションの基本](https://docs.groupdocs.com/redaction/net/redaction-basics/)
* ドキュメントの注釈編集に関する詳細: [注釈編集](https://docs.groupdocs.com/redaction/net/annotation-redactions/)

### 例

次の例は、すべての注釈で「John」という名前を「[redacted]」に置き換える方法を示しています。

```csharp
using (Redactor redactor = new Redactor(@"C:\test.pdf"))
{
   redactor.Apply(new AnnotationRedaction("(?im:john)", "[redacted]"));
   redactor.Save()
}
```

### 関連項目

* class [Redaction](../../groupdocs.redaction/redaction)
* 名前空間 [GroupDocs.Redaction.Redactions](../../groupdocs.redaction.redactions)
* 組み立て [GroupDocs.Redaction](../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Redaction.dll -->
