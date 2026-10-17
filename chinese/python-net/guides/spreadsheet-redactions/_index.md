---
title: "电子表格脱敏"
linkTitle: "Spreadsheet redactions"
second_title: "GroupDocs.Redaction 用于 Python，通过 .NET API 参考"
description: "本文展示了 Python 脱敏 API 如何从您的 XLS、XLSX、ODS 电子表格文档格式及其他格式中脱敏敏感或私人数据。"
type: docs
url: /zh/python-net/guides/spreadsheet-redactions/
is_root: false
weight: 90
---


GroupDocs.Redaction 能够从您的 XLS、XLSX、ODS 电子表格文档格式及其他格式中脱敏敏感或私人数据。请参阅[supported document formats]() 文章中的完整列表。

## Redact spreadsheet content

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.options import SaveOptions
from groupdocs.redaction.redactions import ExactPhraseRedaction, ReplacementOptions

def redact_spreadsheet_content():
    # 指定脱敏选项
    repl_opt = ReplacementOptions("-redacted-")
    ex_red = ExactPhraseRedaction("John Doe", repl_opt)

    # 加载待脱敏的电子表格
    with Redactor("./sample.xlsx") as redactor:
        # 应用编辑
        result = redactor.apply(ex_red)

        # 将脱敏后的文档保存到源文件旁边
        so = SaveOptions()
        so.add_suffix = True
        so.rasterize_to_pdf = False
        so.redacted_file_suffix = "redacted"
        redactor.save(so)

if __name__ == "__main__":
    redact_spreadsheet_content()
```

`sample.xlsx` 是本示例中使用的示例文件。点击 [here](https://docs.groupdocs.com/redaction/python-net/_sample_files/developer-guide/basic-usage/spreadsheet-redactions/sample.xlsx) 下载。

  
```text
Binary file (XLSX, 15 KB)
```
[Download full output](https://docs.groupdocs.com/redaction/python-net/_output_files/developer-guide/basic-usage/spreadsheet-redactions/redact_spreadsheet_content/sample_redacted.xlsx)
