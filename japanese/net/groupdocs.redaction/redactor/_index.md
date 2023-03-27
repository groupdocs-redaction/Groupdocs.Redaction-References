---
title: Redactor
second_title: GroupDocs.Redaction for .NET API リファレンス
description: ドキュメントの編集プロセスを制御するメイン クラスを表しドキュメントを開く編集する保存することができます
type: docs
weight: 660
url: /ja/net/groupdocs.redaction/redactor/
---
## Redactor class

ドキュメントの編集プロセスを制御するメイン クラスを表し、ドキュメントを開く、編集する、保存することができます。

```csharp
public sealed class Redactor : IDisposable, IPreviewable
```

## コンストラクター

| 名前 | 説明 |
| --- | --- |
| [Redactor](redactor#constructor)(Stream) | の新しいインスタンスを初期化します[`Redactor`](../redactor) stream. を使用したクラス |
| [Redactor](redactor#constructor_3)(string) | の新しいインスタンスを初期化します[`Redactor`](../redactor)ファイルパスを使用するクラス. |
| [Redactor](redactor#constructor_1)(Stream, LoadOptions) | の新しいインスタンスを初期化します[`Redactor`](../redactor) stream. を使用したパスワードで保護されたドキュメントのクラス |
| [Redactor](redactor#constructor_4)(string, LoadOptions) | の新しいインスタンスを初期化します[`Redactor`](../redactor) path. を使用した、パスワードで保護されたドキュメントのクラス |
| [Redactor](redactor#constructor_2)(Stream, LoadOptions, RedactorSettings) | の新しいインスタンスを初期化します[`Redactor`](../redactor)stream と settings. を使用した、パスワードで保護されたドキュメントのクラス |
| [Redactor](redactor#constructor_5)(string, LoadOptions, RedactorSettings) | の新しいインスタンスを初期化します[`Redactor`](../redactor)パスと設定を使用して、パスワードで保護されたドキュメントのクラス. |

## メソッド

| 名前 | 説明 |
| --- | --- |
| [Apply](../../groupdocs.redaction/redactor/apply#apply)(Redaction) | ドキュメントに編集を適用します。 |
| [Apply](../../groupdocs.redaction/redactor/apply#apply_1)(RedactionPolicy) | ドキュメントに編集ポリシーを適用します。 |
| [Apply](../../groupdocs.redaction/redactor/apply#apply_2)(Redaction[]) | 一連の編集をドキュメントに適用します。 |
| [Dispose](../../groupdocs.redaction/redactor/dispose)() | リソースを解放します。 |
| [GeneratePreview](../../groupdocs.redaction/redactor/generatepreview)(PreviewOptions) | 指定された画像形式で特定のページのプレビュー画像を生成します. |
| [GetDocumentInfo](../../groupdocs.redaction/redactor/getdocumentinfo)() | ドキュメントに関する一般的な情報を取得します - サイズ、ページ数など. |
| [Save](../../groupdocs.redaction/redactor/save#save)() | 次のオプションでドキュメントをファイルに保存します: AddSuffix = true、RasterizeToPDF = true. |
| [Save](../../groupdocs.redaction/redactor/save#save_1)(SaveOptions) | ドキュメントをファイルに保存します。 |
| [Save](../../groupdocs.redaction/redactor/save#save_2)(Stream, RasterizationOptions) | カスタムの場所を含め、ドキュメントをストリームに保存します。 |

### 備考

**もっと詳しく知る**

* リダクションの適用に関する詳細: [リダクションの基本](https://docs.groupdocs.com/redaction/net/redaction-basics/)
* より高度な編集トピック: [高度な使い方](https://docs.groupdocs.com/redaction/net/advanced-usage/)

### 例

次の例は、ドキュメントに単一のリダクションを適用する方法を示しています。

次の例は、リダクションのリストをドキュメントに適用する方法を示しています。

次の例は、特定のインバウンド フォルダー内のすべてのファイルにリダクション ポリシーを適用し、正常に更新されたファイルと失敗したファイルのいずれかのアウトバウンド フォルダーに保存する方法を示しています。

次の例は、LoadOptions を使用してパスワードで保護されたドキュメントを開く方法を示しています。

次の例は、SaveOptions を使用してドキュメントを保存する方法を示しています。

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

```csharp
using (Redactor redactor = new Redactor(@"D:\\test.docx"))
{
   var redactionList = new Redaction[] 
   {
      new ExactPhraseRedaction(LookupStrings.ClientName, new ReplacementOptions("[client]")),
      new ExactPhraseRedaction(LookupStrings.ClientAddress, new ReplacementOptions(System.Drawing.Color.Red)),
      new RegexRedaction(LookupStrings.SSNRegexPattern, new ReplacementOptions("[ssn]")),
      new RegexRedaction(LookupStrings.BankCardRegexPattern, new ReplacementOptions(System.Drawing.Color.Blue)),
      // ... その他のリダクション
      new DeleteAnnotationRedaction("(?im:(use|show|describe))"),
      new EraseMetadataRedaction(MetadataFilter.Author),
      new MetadataSearchRedaction(LookupStrings.CompanyName, "--company--") 
   }; 
   RedactorChangeLog result = redactor.Apply(redactionList);
   // false、少なくとも 1 つのリダクションが失敗した場合
   if (result.Status != RedactionStatus.Failed)
   {
      redactor.Save();
   };
}
```

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

```csharp
LoadOptions loadOptions = new LoadOptions("mypassword");
using (Redactor redactor = new Redactor(@"C:\sample.pdf", loadOptions))
{
    // ここで、ドキュメント インスタンスを使用してリダクションを実行できます
}
```

```csharp
    using (Redactor redactor = new Redactor(@"C:\sample.pdf"))
    {
       // ドキュメントのリダクションがここに入る
       // ...
    
       // ドキュメントをデフォルトのオプションで保存します (ページを画像に変換し、PDF として保存します)
       redactor.Save();
    
       // ドキュメントを元の形式で保存し、元のファイルを上書きします
       redactor.Save(new SaveOptions() { AddSuffix = false, RasterizeToPDF = false });
    
       // ドキュメントを「*_Redacted.*」ファイルに元の形式で保存します
       redactor.Save(new SaveOptions() { AddSuffix = true, RasterizeToPDF = false });
    
       // ドキュメントをラスタライズせずに、そのファイル名で "*_AnyText.*" (たとえば、"AnyText" ではなくタイムスタンプ) に保存します。
       redactor.Save(new SaveOptions(false, "AnyText"));
    }    
```

### 関連項目

* interface [IPreviewable](../../groupdocs.redaction.integration/ipreviewable)
* 名前空間 [GroupDocs.Redaction](../../groupdocs.redaction)
* 組み立て [GroupDocs.Redaction](../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Redaction.dll -->
