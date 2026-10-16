---
title: "Redactor"
second_title: "GroupDocs.Redaction（.NET 用）API リファレンス"
description: "ドキュメントの赤字処理プロセスを制御し、開く、赤字化、保存を可能にするメインクラスを表します。"
type: docs
weight: 820
url: /ja/net/groupdocs.redaction/redactor/
---
## Redactor class

ドキュメントの赤字プロセスを制御し、開く、赤字化、保存を可能にするメインクラスを表します。

```csharp
public sealed class Redactor : IDisposable, IPreviewable
```

## コンストラクタ

| 名前 | 説明 |
| --- | --- |
| [Redactor](redactor#constructor)(Stream) | [`Redactor`](../redactor) クラスをストリームで使用する新しいインスタンスを初期化します。 |
| [Redactor](redactor#constructor_3)(string) | [`Redactor`](../redactor) クラスをファイルパスで使用する新しいインスタンスを初期化します。 |
| [Redactor](redactor#constructor_1)(Stream, LoadOptions) | パスワード保護されたドキュメント用にストリームを使用して、[`Redactor`](../redactor) クラスの新しいインスタンスを初期化します。 |
| [Redactor](redactor#constructor_4)(string, LoadOptions) | パスワードで保護されたドキュメントのパスを使用して、[`Redactor`](../redactor) クラスの新しいインスタンスを初期化します。 |
| [Redactor](redactor#constructor_2)(Stream, LoadOptions, RedactorSettings) | ストリームと設定を使用して、パスワードで保護されたドキュメントの [`Redactor`](../redactor) クラスの新しいインスタンスを初期化します。 |
| [Redactor](redactor#constructor_5)(string, LoadOptions, RedactorSettings) | パスと設定を使用して、パスワードで保護されたドキュメントの [`Redactor`](../redactor) クラスの新しいインスタンスを初期化します。 |

## メソッド

| 名前 | 説明 |
| --- | --- |
| [Apply](../../groupdocs.redaction/redactor/apply#apply)(Redaction) | ドキュメントにレダクションを適用します。 |
| [Apply](../../groupdocs.redaction/redactor/apply#apply_1)(RedactionPolicy) | ドキュメントにレダクションポリシーを適用します。 |
| [Apply](../../groupdocs.redaction/redactor/apply#apply_2)(Redaction[]) | ドキュメントにレダクションのセットを適用します。 |
| [Dispose](../../groupdocs.redaction/redactor/dispose)() | リソースを解放します。 |
| [GeneratePreview](../../groupdocs.redaction/redactor/generatepreview)(PreviewOptions) | 指定された画像形式で特定のページのプレビュー画像を生成します。 |
| [GetDocumentInfo](../../groupdocs.redaction/redactor/getdocumentinfo)() | ドキュメントの一般情報（サイズ、ページ数など）を取得します。 |
| [Save](../../groupdocs.redaction/redactor/save#save)() | 次のオプションでドキュメントをファイルに保存します: AddSuffix = true, RasterizeToPDF = true。 |
| [Save](../../groupdocs.redaction/redactor/save#save_1)(SaveOptions) | ドキュメントをファイルに保存します。 |
| [Save](../../groupdocs.redaction/redactor/save#save_3)(Stream, SaveOptions) | ドキュメントを指定されたストリームに保存します。 |

### 備考

**Learn more**

* More details about applying redactions: [Redaction basics](https://docs.groupdocs.com/redaction/net/redaction-basics/)
* More advanced redaction topics: [Advanced usage](https://docs.groupdocs.com/redaction/net/advanced-usage/)

### 例

次の例は、ドキュメントに単一のレダクションを適用する方法を示しています。

```csharp
using (Redactor redactor = new Redactor(@"D:\\test.docx"))
{
   RedactorChangeLog result = redactor.Apply(new RegexRedaction(LookupStrings.SSNRegexPattern, new ReplacementOptions("[ssn]")));
   if (result.Status != RedactionStatus.Failed)
   {
      redactor.Save();
   };
}
```

次の例は、ドキュメントにレダクションのリストを適用する方法を示しています。

```csharp
using (Redactor redactor = new Redactor(@"D:\\test.docx"))
{
var redactionList = new Redaction[]
{
new ExactPhraseRedaction(LookupStrings.ClientName, new ReplacementOptions("[client]")),
new ExactPhraseRedaction(LookupStrings.ClientAddress, new ReplacementOptions(GroupDocs.Redaction.Options.Drawing.Color.Red)),
new RegexRedaction(LookupStrings.SSNRegexPattern, new ReplacementOptions("[ssn]")),
new RegexRedaction(LookupStrings.BankCardRegexPattern, new ReplacementOptions(GroupDocs.Redaction.Options.Drawing.Color.Blue)),
// ... その他のレダクション
new DeleteAnnotationRedaction("(?im:(use|show|describe))"),
new EraseMetadataRedaction(MetadataFilter.Author),
new MetadataSearchRedaction(LookupStrings.CompanyName, "--company--")
};
RedactorChangeLog result = redactor.Apply(redactionList);
// false、少なくとも1つのレダクションが失敗した場合
if (result.Status != RedactionStatus.Failed)
{
redactor.Save();
};
}
```

次の例は、指定された受信フォルダー内のすべてのファイルにリダクション ポリシーを適用し、正常に更新されたファイルと失敗したファイル用に、送信フォルダーのいずれかに保存する方法を示しています。

```csharp
RedactionPolicy policy = RedactionPolicy.Load("RedactionPolicy.xml");
foreach (var fileEntry in Directory.GetFileNames("C:\\Inbound")) 
{
     using (Redactor redactor = new Redactor(Path.Combine("C:\\Inbound\\", fileEntry)))
     {
    	     RedactorChangeLog result = redactor.Apply(policy);
    	     String resultFolder = result.Status != RedactionStatus.Failed ? "C:\\Outbound\\Done\\" : "C:\\Outbound\\Failed\\";
    	     using (Stream fileStream = File.Open(Path.Combine(resultFolder, fileEntry), FileMode.Open, FileAccess.ReadWrite))
   	     {
               redactor.Save(fileStream, new RasterizationOptions() { Enabled = false });
   	     }        
     }
}   
```

次の例は、LoadOptions を使用してパスワードで保護されたドキュメントを開く方法を示しています。

```csharp
LoadOptions loadOptions = new LoadOptions("mypassword");
using (Redactor redactor = new Redactor(@"C:\sample.pdf", loadOptions))
{
    // ここでは、ドキュメントインスタンスを使用してレダクションを実行できます。
}
```

次の例は SaveOptions を使用してドキュメントを保存する方法を示しています。

```csharp
    using (Redactor redactor = new Redactor(@"C:\sample.pdf"))
    {
       // ここにドキュメントの編集が入ります
       // ...
    
       // デフォルトオプションでドキュメントを保存します（ページを画像に変換し、PDF として保存）
       redactor.Save();
    
       // 元の形式でドキュメントを保存し、元のファイルを上書きします
       redactor.Save(new SaveOptions() { AddSuffix = false, RasterizeToPDF = false });
    
       // 元の形式でドキュメントを "*_Redacted.*" ファイルに保存します
       redactor.Save(new SaveOptions() { AddSuffix = true, RasterizeToPDF = false });
    
       // ラスター化せずに、ファイル名に "*_AnyText.*"（例："AnyText" の代わりにタイムスタンプ）を付けてドキュメントを保存します
       redactor.Save(new SaveOptions(false, "AnyText"));
    }    
```

### 参照

* interface [IPreviewable](../../groupdocs.redaction.integration/ipreviewable)
* namespace [GroupDocs.Redaction](../../groupdocs.redaction)
* assembly [GroupDocs.Redaction](../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Redaction.dll -->
