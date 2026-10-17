---
title: "LoadOptions 类"
second_title: "GroupDocs.Redaction 用于 Python，通过 .NET API 参考"
description: "提供用于打开文件的选项。"
type: docs
url: /zh/python-net/groupdocs.redaction.options/loadoptions/
is_root: false
weight: 40
---


## LoadOptions class

提供用于打开文件的选项。

了解更多
- [Loading documents](https://docs.groupdocs.com/redaction/net/loading-documents/)
- [Load from local disk](https://docs.groupdocs.com/redaction/net/load-from-local-disc/)
- [Load from stream](https://docs.groupdocs.com/redaction/net/load-from-stream/)
- [Load password-protected document](https://docs.groupdocs.com/redaction/net/load-password-protected-file/)

LoadOptions 类型公开以下成员：

### 构造函数
| 构造函数 | 描述 |
| :- | :- |
| [__init__](/redaction/python-net/groupdocs.redaction.options/loadoptions/__init__/) | 初始化 LoadOptions 类的新实例。 |
| [__init__](/redaction/python-net/groupdocs.redaction.options/loadoptions/__init__/#password) | 使用指定的密码初始化 LoadOptions 的新实例。 |
| [__init__](/redaction/python-net/groupdocs.redaction.options/loadoptions/__init__/#pre_rasterize) | 使用指定的预光栅化标志初始化新的 LoadOptions 实例。 |
| [__init__](/redaction/python-net/groupdocs.redaction.options/loadoptions/__init__/#password-pre_rasterize) | 使用指定的密码初始化新的 LoadOptions 实例。 |

### 属性
| 属性 | 描述 |
| :- | :- |
| [password](/redaction/python-net/groupdocs.redaction.options/loadoptions/password/) | 受密码保护的文档的密码。 |
| [pre_rasterize](/redaction/python-net/groupdocs.redaction.options/loadoptions/pre_rasterize/) | pre_rasterize 标志指示文件是否应预光栅化。 |

### 示例

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.options import LoadOptions, SaveOptions
from groupdocs.redaction.redactions import ExactPhraseRedaction, ReplacementOptions

# 使用文档密码指定加载选项
load_opt = LoadOptions("mypassword")

# 定义遮蔽
repl_opt = ReplacementOptions("[personal]")
ex_red = ExactPhraseRedaction("John Doe", repl_opt)

# 打开受密码保护的文档
with Redactor("./protected.docx", load_opt) as redactor:
    redactor.apply(ex_red)

    # 保存已遮蔽的文档
    save_opt = SaveOptions()
    save_opt.add_suffix = True
    result_path = redactor.save(save_opt)
    print(f"Document redacted successfully. Check output in {result_path}.")
```

### 另请参阅
* module [`groupdocs.redaction.options`](/redaction/python-net/groupdocs.redaction.options/)
