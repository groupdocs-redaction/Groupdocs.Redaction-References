---
title: RedactionPolicy
second_title: GroupDocs.Redaction for .NET API リファレンス
description: 適用する特定のリダクションのセットを含むサニタイズ ポリシーを表します.
type: docs
weight: 410
url: /ja/net/groupdocs.redaction/redactionpolicy/
---
## RedactionPolicy class

適用する特定のリダクションのセットを含むサニタイズ ポリシーを表します.

```csharp
public class RedactionPolicy
```

## コンストラクター

| 名前 | 説明 |
| --- | --- |
| [RedactionPolicy](redactionpolicy#constructor)() | Redaction ポリシーの新しいインスタンスを作成します。 |
| [RedactionPolicy](redactionpolicy#constructor_1)(Redaction[]) | リダクションの特定のリストを使用して、リダクション ポリシーの新しいインスタンスを作成します。 |

## プロパティ

| 名前 | 説明 |
| --- | --- |
| [Redactions](../../groupdocs.redaction/redactionpolicy/redactions) { get; } | 完全に構成された配列を取得します[`Redaction`](../redaction)-派生クラス. |

## メソッド

| 名前 | 説明 |
| --- | --- |
| static [Load](../../groupdocs.redaction/redactionpolicy/load#load)(Stream) | のインスタンスをロードします[`RedactionPolicy`](../redactionpolicy)ストリームから. |
| static [Load](../../groupdocs.redaction/redactionpolicy/load#load_1)(string) | のインスタンスをロードします[`RedactionPolicy`](../redactionpolicy)ファイルパスから. |
| [Save](../../groupdocs.redaction/redactionpolicy/save#save)(Stream) | リダクション ポリシーをストリームに保存します。 |
| [Save](../../groupdocs.redaction/redactionpolicy/save#save_1)(string) | リダクション ポリシーをファイルに保存します。 |

### 備考

**もっと詳しく知る**

* ポリシーの詳細: [リダクション ポリシーの使用](https://docs.groupdocs.com/redaction/net/use-redaction-policies/)
* リダクションの適用に関する詳細: [リダクションの基本](https://docs.groupdocs.com/redaction/net/redaction-basics/)

### 例

次の例は、特定のインバウンド フォルダー内のすべてのファイルにリダクション ポリシーを適用し、正常に更新されたファイルと失敗したファイルのいずれかのアウトバウンド フォルダーに保存する方法を示しています。

次の例には、すべてのタイプのリダクションのサンプル設定を含むサンプル XML ポリシー ファイルが含まれています。

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
<?xml version="1.0" encoding="utf-8"?>  
<redactionPolicy xmlns = "http://www.groupdocs.com/redaction" >
  <regexRedaction regularExpression="(dolor)" actionType="ReplaceString" replacement="foobar" />  
  <exactPhraseRedaction searchPhrase = "dolor" caseSensitive="true" actionType="DrawBox" color="Red" />   
  
  <cellColumnRedaction regularExpression = "(foo)bar1" replacement="[red1]" columnIndex="1" worksheetIndex="2" /> 
  <cellColumnRedaction regularExpression = "(foo)bar2" replacement="[red2]" wokrsheetName="Sample" /> 
  
  <eraseMetadataRedaction filter = "All" />
  <metadataSearchRedaction filter="Title, Author" replacement="foobar" valueExpression="(metasearch)" keyExpression="" />  
  
 <annotationRedaction regularExpression = "(anno1)" replacement="foobar" />  
 <deleteAnnotationRedaction regularExpression = "(anno2)" />

 <imageAreaRedaction pointX="15" pointY="17" width="200" height="10" color="#AA50FC"  />  
 <imageAreaRedaction pointX = "110" pointY="120" width="60" height="20" color="Magenta"  />  
</redactionPolicy>
```

### 関連項目

* 名前空間 [GroupDocs.Redaction](../../groupdocs.redaction)
* 組み立て [GroupDocs.Redaction](../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Redaction.dll -->