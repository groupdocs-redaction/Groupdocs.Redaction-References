---
title: "Редактирование электронных таблиц"
linkTitle: "Spreadsheet redactions"
second_title: "GroupDocs.Redaction для Python через .NET справочник API"
description: "В этой статье показано, как API редактирования Python позволяет удалять данные чувствительного или частного характера из ваших электронных таблиц форматов XLS, XLSX, ODS и других."
type: docs
url: /ru/python-net/guides/spreadsheet-redactions/
is_root: false
weight: 90
---


GroupDocs.Redaction позволяет удалять данные чувствительного или частного характера из ваших электронных таблиц форматов XLS, XLSX, ODS и других. Смотрите полный список в статье [supported document formats]().

## Redact spreadsheet content

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.options import SaveOptions
from groupdocs.redaction.redactions import ExactPhraseRedaction, ReplacementOptions

def redact_spreadsheet_content():
    # Укажите параметры редактирования
    repl_opt = ReplacementOptions("-redacted-")
    ex_red = ExactPhraseRedaction("John Doe", repl_opt)

    # Загрузите электронную таблицу для редактирования
    with Redactor("./sample.xlsx") as redactor:
        # Применить редактирование
        result = redactor.apply(ex_red)

        # Сохраните отредактированный документ рядом с исходным файлом
        so = SaveOptions()
        so.add_suffix = True
        so.rasterize_to_pdf = False
        so.redacted_file_suffix = "redacted"
        redactor.save(so)

if __name__ == "__main__":
    redact_spreadsheet_content()
```

`sample.xlsx` — пример файла, используемый в этом примере. Нажмите [here](https://docs.groupdocs.com/redaction/python-net/_sample_files/developer-guide/basic-usage/spreadsheet-redactions/sample.xlsx), чтобы скачать его.

  
```text
Binary file (XLSX, 15 KB)
```
[Download full output](https://docs.groupdocs.com/redaction/python-net/_output_files/developer-guide/basic-usage/spreadsheet-redactions/redact_spreadsheet_content/sample_redacted.xlsx)
