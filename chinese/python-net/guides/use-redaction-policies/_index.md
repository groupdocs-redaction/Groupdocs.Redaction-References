---
title: "使用遮蔽策略"
linkTitle: "Use redaction policies"
second_title: "GroupDocs.Redaction 用于 Python，通过 .NET API 参考"
description: "了解如何处理。如果你有企业敏感数据删除策略，以遮蔽规则列表的形式存在，则无需在代码中指定它们。你可以提供包含预配置遮蔽列表的 XML 文档。"
type: docs
url: /zh/python-net/guides/use-redaction-policies/
is_root: false
weight: 110
---


如果你有企业敏感数据删除策略，以遮蔽规则列表的形式存在，则无需在代码中指定它们。你可以提供包含预配置遮蔽列表的 XML 文档。

下面是一个遮蔽策略 XML 文件的示例（代码属性映射显而易见）：

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
你可以使用 RedactionPolicy.save() 方法创建此结构的 XML 文档，在运行时配置遮蔽。

以下示例演示如何将 [RedactionPolicy](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction/redactionpolicy/) 保存为 XML 文件。
 

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
    # 定义遮蔽的颜色
    color = Color.from_argb(255, 220, 20, 60)

    # 配置遮蔽
    redactions = [
        ExactPhraseRedaction("Redaction", ReplacementOptions("[Product]")),
        RegexRedaction("\\d{2}\\s*\\d{2}[^\\d]*\\d{6}", ReplacementOptions(color)),
        DeleteAnnotationRedaction(),
        EraseMetadataRedaction(MetadataFilters.ALL),
    ]

    # 创建策略
    policy = RedactionPolicy(redactions)

    # 将遮蔽策略保存为 XML 文件
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

你可以根据需要创建任意数量的策略，并加载它们来遮蔽文档。

下面的示例从 XML 文件加载遮蔽策略，并在一次 `apply` 调用中将其包含的所有规则应用到文档上：

```python
from groupdocs.redaction import Redactor, RedactionPolicy
from groupdocs.redaction.options import SaveOptions

def use_redaction_policy():
    # 从 XML 文件加载遮蔽策略
    policy = RedactionPolicy.load("./redaction_policy.xml")

    # 加载文档并一次性应用完整策略
    with Redactor("./sample.docx") as redactor:
        redactor.apply(policy)

        # 保持原始格式并在输出名称后追加后缀
        save_options = SaveOptions()
        save_options.add_suffix = True
        save_options.rasterize_to_pdf = False
        save_options.redacted_file_suffix = "redacted"
        result_path = redactor.save(save_options)

    print(f"Redaction policy applied. Output saved to {result_path}.")

if __name__ == "__main__":
    use_redaction_policy()
```

`redaction_policy.xml` 是本示例使用的策略文件。点击 [here](https://docs.groupdocs.com/redaction/python-net/_sample_files/developer-guide/advanced-usage/use-redaction-policies/redaction_policy.xml) 下载。

`sample.docx` 是本示例中被编辑的文档。点击 [此处](https://docs.groupdocs.com/redaction/python-net/_sample_files/developer-guide/advanced-usage/use-redaction-policies/sample.docx) 下载它。

  
```text
Binary file (DOCX, 16 KB)
```
[Download full output](https://docs.groupdocs.com/redaction/python-net/_output_files/developer-guide/advanced-usage/use-redaction-policies/use_redaction_policy/sample_redacted.docx)
