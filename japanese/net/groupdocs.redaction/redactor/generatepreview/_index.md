---
title: GeneratePreview
second_title: GroupDocs.Redaction for .NET API リファレンス
description: 指定された画像形式で特定のページのプレビュー画像を生成します.
type: docs
weight: 40
url: /ja/net/groupdocs.redaction/redactor/generatepreview/
---
## Redactor.GeneratePreview method

指定された画像形式で特定のページのプレビュー画像を生成します.

```csharp
public void GeneratePreview(PreviewOptions previewOptions)
```

| パラメータ | タイプ | 説明 |
| --- | --- | --- |
| previewOptions | PreviewOptions | 画像のプロパティとページ範囲の設定 |

### 例

次の例は、ドキュメントのプレビューを取得する方法を示しています[`PreviewOptions`](../../../groupdocs.redaction.options/previewoptions)と両方の代表。

```csharp
    CreatePageStream createDelegate = delegate (int pageNumber)
    {
        var pagePath = System.IO.Path.Combine(@"C:\Temp", string.Format("page_{0}.png", pageNumber));
        return System.IO.File.Create(pagePath);
    };
    ReleasePageStream releaseDelegate = delegate (int pageNumber, System.IO.Stream pageStream)
    {
        // ページのプレビューを含め、Stream を使って何でもします
        pageStream.Close();
    };
    var previewOptions = new PreviewOptions(createDelegate, releaseDelegate);
    previewOptions.PreviewFormat = PreviewOptions.PreviewFormats.PNG;
    previewOptions.Height = 640;
    previewOptions.Width = 480;
    previewOptions.PageNumbers = new int[] { 1 };
    using (var redactor = new Redactor("C:\Temp\SourceFile.pdf"))
    {
        redactor.GeneratePreview(previewOptions);
    }
```

### 関連項目

* class [PreviewOptions](../../../groupdocs.redaction.options/previewoptions)
* class [Redactor](../../redactor)
* 名前空間 [GroupDocs.Redaction](../../redactor)
* 組み立て [GroupDocs.Redaction](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Redaction.dll -->