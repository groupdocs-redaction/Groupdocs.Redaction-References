---
title: "赤字ポリシーを使用する"
linkTitle: "Use redaction policies"
second_title: "GroupDocs.Redaction for Python via .NET API リファレンス"
description: "対処方法を学びましょう。企業の機密データ除去ポリシーが赤字ルールのリストとしてある場合、コード内で指定する必要はありません。事前に設定された赤字のリストを含む XML ドキュメントを指定できます。"
type: docs
url: /ja/python-net/guides/use-redaction-policies/
is_root: false
weight: 110
---


企業の機密データ除去ポリシーが赤字ルールのリストとしてある場合、コード内で指定する必要はありません。事前に設定された赤字のリストを含む XML ドキュメントを指定できます。

以下は赤字ポリシー XML ファイルの例です（コードプロパティのマッピングは明らかです）：

**RedactionPolicy.xml**

```xml
<?xml version="1.0" encoding="utf-8"?>  
<redactionPolicy xmlns="http://www.groupdocs.com/redaction">  
  <regexRedaction regularExpression="(dolor)" actionType="ReplaceString" replacement="foobar" />  
  <exactPhraseRedaction searchPhrase="dolor" caseSensitive="true" actionType="DrawBox" color="Red" />   
  
  <eraseMetadataRedaction filter="All" />  
  <metadataSearchRedaction filter="Title, Author" replacement="foobar" valueExpression="(metasearch)" keyExpression="" />  
  
  <annotationRedaction regularExpression="(anno1)" replacement="foobar" />  
  <deleteAnnotationRedaction regularExpression="(anno2)" />  
  
  <imageAreaRedaction pointX="15" pointY="17" width="200" height="10" color="#AA50FC"  />  
  <imageAreaRedaction pointX="110" pointY="120" width="60" height="20" color="Magenta"  />  
</redactionPolicy> 
```
この構造の XML ドキュメントを作成するには、RedactionPolicy.save() メソッドを使用して、実行時に赤字を設定できます。

次の例は、[RedactionPolicy](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction/redactionpolicy/) を XML ファイルに保存する方法を示しています。
 

```python
from groupdocs.redaction import RedactionPolicy
from groupdocs.redaction.redactions import (
    ExactPhraseRedaction,
    ReplacementOptions,
    RegexRedaction,
    DeleteAnnotationRedaction,
    EraseMetadataRedaction,
    MetadataFilters,
)
from groupdocs.pydrawing import Color

def create_redaction_policy():
    # 赤字の色を定義する
    color = Color.from_argb(255, 220, 20, 60)

    # 赤字を設定する
    redactions = [
        ExactPhraseRedaction("Redaction", ReplacementOptions("[Product]")),
        RegexRedaction("\\d{2}\\s*\\d{2}[^\\d]*\\d{6}", ReplacementOptions(color)),
        DeleteAnnotationRedaction(),
        EraseMetadataRedaction(MetadataFilters.ALL),
    ]

    # ポリシーを作成する
    policy = RedactionPolicy(redactions)

    # 赤字ポリシーを XML ファイルに保存する
    policy.save("./sample_policy.xml")
    print("Redactions policy saved to ./sample_policy.xml")

if __name__ == "__main__":
    create_redaction_policy()
```

  
```text
<?xml version="1.0"?>
<redactionPolicy>
  <exactPhraseRedaction actionType="ReplaceString" replacement="[Product]" searchPhrase="Redaction" />
  <regexRedaction actionType="DrawBox" color="#DC143C" regularExpression="\d{2}\s*\d{2}[^\d]*\d{6}" />
  <deleteAnnotationRedaction regularExpression="[.]*" />
  <eraseMetadataRedaction filter="All" />
</redactionPolicy>
```
[Download full output](https://docs.groupdocs.com/redaction/python-net/_output_files/developer-guide/advanced-usage/use-redaction-policies/create_redaction_policy/sample_policy.xml)

必要なだけ多くのポリシーを作成でき、ドキュメントを赤字するためにそれらをロードします。

以下の例は XML ファイルから赤字ポリシーをロードし、含まれるすべてのルールを単一の `apply` 呼び出しでドキュメントに適用します：

```python
from groupdocs.redaction import Redactor, RedactionPolicy
from groupdocs.redaction.options import SaveOptions

def use_redaction_policy():
    # XML ファイルから赤字ポリシーをロードする
    policy = RedactionPolicy.load("./redaction_policy.xml")

    # ドキュメントをロードし、1 回の呼び出しでポリシー全体を適用する
    with Redactor("./sample.docx") as redactor:
        redactor.apply(policy)

        # 元の形式を保持し、出力名にサフィックスを付加する
        save_options = SaveOptions()
        save_options.add_suffix = True
        save_options.rasterize_to_pdf = False
        save_options.redacted_file_suffix = "redacted"
        result_path = redactor.save(save_options)

    print(f"Redaction policy applied. Output saved to {result_path}.")

if __name__ == "__main__":
    use_redaction_policy()
```

`redaction_policy.xml` はこの例で使用されるポリシーファイルです。[here](https://docs.groupdocs.com/redaction/python-net/_sample_files/developer-guide/advanced-usage/use-redaction-policies/redaction_policy.xml) をクリックしてダウンロードしてください。

`sample.docx` はこの例で編集されたドキュメントです。ダウンロードするには[here](https://docs.groupdocs.com/redaction/python-net/_sample_files/developer-guide/advanced-usage/use-redaction-policies/sample.docx)をクリックしてください。

  
```text
Binary file (DOCX, 16 KB)
```
[Download full output](https://docs.groupdocs.com/redaction/python-net/_output_files/developer-guide/advanced-usage/use-redaction-policies/use_redaction_policy/sample_redacted.docx)
