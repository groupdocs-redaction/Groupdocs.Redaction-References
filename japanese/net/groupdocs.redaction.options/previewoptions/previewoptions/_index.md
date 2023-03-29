---
title: PreviewOptions
second_title: GroupDocs.Redaction for .NET API リファレンス
description: PreviewOptions クラスの新しいインスタンスを初期化し出力ストリームを閉じます
type: docs
weight: 10
url: /ja/net/groupdocs.redaction.options/previewoptions/previewoptions/
---
## PreviewOptions(CreatePageStream) {#constructor}

PreviewOptions クラスの新しいインスタンスを初期化し、出力ストリームを閉じます。

```csharp
public PreviewOptions(CreatePageStream createPageStream)
```

| パラメータ | タイプ | 説明 |
| --- | --- | --- |
| createPageStream | CreatePageStream | 特定のページ プレビュー用のストリームを作成します |

### 関連項目

* delegate [CreatePageStream](../../createpagestream)
* class [PreviewOptions](../../previewoptions)
* 名前空間 [GroupDocs.Redaction.Options](../../previewoptions)
* 組み立て [GroupDocs.Redaction](../../../)

---

## PreviewOptions(CreatePageStream, ReleasePageStream) {#constructor_1}

PreviewOptions クラスの新しいインスタンスを初期化し、出力ストリームをクライアントに返してさらに使用できるようにします。

```csharp
public PreviewOptions(CreatePageStream createPageStream, ReleasePageStream releasePageStream)
```

| パラメータ | タイプ | 説明 |
| --- | --- | --- |
| createPageStream | CreatePageStream | 特定のページ プレビュー用のストリームを作成します |
| releasePageStream | ReleasePageStream | ページ プレビューの生成が完了したことを通知し、出力ストリームを取得します |

### 関連項目

* delegate [CreatePageStream](../../createpagestream)
* delegate [ReleasePageStream](../../releasepagestream)
* class [PreviewOptions](../../previewoptions)
* 名前空間 [GroupDocs.Redaction.Options](../../previewoptions)
* 組み立て [GroupDocs.Redaction](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Redaction.dll -->