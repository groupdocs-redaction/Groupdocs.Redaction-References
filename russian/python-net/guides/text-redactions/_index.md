---
title: "Редактирование текста"
linkTitle: "Text redaction"
second_title: "GroupDocs.Redaction для Python через .NET справочник API"
description: "В этой статье объясняется, как API редактирования Python позволяет легко скрывать конфиденциальные или личные данные в ваших документах. Вы можете применять редактирование текста, используя точную фразу или регулярное выражение, для документов разных форматов, таких как PDF, DOC, DOCX, PPT, PPTX, XLS, XLSX и другие."
type: docs
url: /ru/python-net/guides/text-redactions/
is_root: false
weight: 50
---


GroupDocs.Redaction позволяет легко скрывать конфиденциальные или личные данные в ваших документах. Наиболее распространённый случай редактирования — удаление текста из документа.

С помощью GroupDocs.Redaction API вы можете применять редактирование текста, используя точную фразу или [регулярное выражение](https://docs.microsoft.com/en-us/dotnet/standard/base-types/regular-expressions) для документов разных форматов, таких как PDF, DOC, DOCX, PPT, PPTX, XLS, XLSX и другие. Полный список см. в статье [поддерживаемые форматы документов]().

## Use exact phrase redaction

В приведённом ниже примере мы применяем текстовое редактирование, заменяя точную личную фразу "John Doe" на "\[personal\]" (или любой код исключения):

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.options import SaveOptions
from groupdocs.redaction.redactions import ExactPhraseRedaction, ReplacementOptions

def redact_exact_phrase():
    # Укажите параметры редактирования
    repl_opt = ReplacementOptions("[personal]")
    ex_red = ExactPhraseRedaction("John Doe", repl_opt)

    # Загрузите документ для редактирования
    with Redactor("./sample.docx") as redactor:
        # Применить редактирование
        result = redactor.apply(ex_red)

        # Сохраните отредактированный документ рядом с исходным файлом
        so = SaveOptions()
        so.add_suffix = True
        so.rasterize_to_pdf = False
        so.redacted_file_suffix = "redacted"
        redactor.save(so)

if __name__ == "__main__":
    redact_exact_phrase()
```

`sample.docx` — это пример файла, используемый в этом примере. Нажмите [здесь](https://docs.groupdocs.com/redaction/python-net/_sample_files/developer-guide/basic-usage/text-redactions/sample.docx) для его загрузки.

  
```text
Binary file (DOCX, 16 KB)
```
[Download full output](https://docs.groupdocs.com/redaction/python-net/_output_files/developer-guide/basic-usage/text-redactions/redact_exact_phrase/sample_redacted.docx)

По умолчанию поиск точной фразы регистронезависим. Для регистрозависимого редактирования существует параметр конструктора и соответствующее публичное свойство:

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.options import SaveOptions
from groupdocs.redaction.redactions import ExactPhraseRedaction, ReplacementOptions

def redact_case_sensitive_phrase():
    # Включить регистрозависимое сопоставление
    case_sensitive = True

    # Укажите параметры редактирования
    repl_opt = ReplacementOptions("[personal]")
    ex_red = ExactPhraseRedaction("John Doe", case_sensitive, repl_opt)

    # Загрузите документ для редактирования
    with Redactor("./sample.docx") as redactor:
        # Применить редактирование
        result = redactor.apply(ex_red)

        # Сохраните отредактированный документ рядом с исходным файлом
        so = SaveOptions()
        so.add_suffix = True
        so.rasterize_to_pdf = False
        so.redacted_file_suffix = "redacted"
        redactor.save(so)

if __name__ == "__main__":
    redact_case_sensitive_phrase()
```

`sample.docx` — это пример файла, используемый в этом примере. Нажмите [здесь](https://docs.groupdocs.com/redaction/python-net/_sample_files/developer-guide/basic-usage/text-redactions/sample.docx) для его загрузки.

  
```text
Binary file (DOCX, 16 KB)
```
[Download full output](https://docs.groupdocs.com/redaction/python-net/_output_files/developer-guide/basic-usage/text-redactions/redact_case_sensitive_phrase/sample_redacted.docx)

Если вам нужен цветной блок над отредактированным текстом, вы можете использовать параметр color вместо строки замены. Редактирование удалит найденный текст и поместит прямоугольник указанного цвета вместо отредактированного текста:

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.options import SaveOptions
from groupdocs.redaction.redactions import ExactPhraseRedaction, ReplacementOptions
from groupdocs.pydrawing import Color

def redact_with_color_box():
    # Определите цвет блока редактирования
    color = Color.from_argb(255, 220, 20, 60)

    # Укажите параметры редактирования
    repl_opt = ReplacementOptions(color)
    ex_red = ExactPhraseRedaction("John Doe", repl_opt)

    # Загрузите документ для редактирования
    with Redactor("./sample.docx") as redactor:
        # Применить редактирование
        result = redactor.apply(ex_red)

        # Сохраните отредактированный документ рядом с исходным файлом
        so = SaveOptions()
        so.add_suffix = True
        so.rasterize_to_pdf = False
        so.redacted_file_suffix = "redacted"
        redactor.save(so)

if __name__ == "__main__":
    redact_with_color_box()
```

`sample.docx` — это пример файла, используемый в этом примере. Нажмите [здесь](https://docs.groupdocs.com/redaction/python-net/_sample_files/developer-guide/basic-usage/text-redactions/sample.docx) для его загрузки.

  
```text
Binary file (DOCX, 17 KB)
```
[Download full output](https://docs.groupdocs.com/redaction/python-net/_output_files/developer-guide/basic-usage/text-redactions/redact_with_color_box/sample_redacted.docx)

Возможно, вам потребуется применить редактирование к документу с направлением справа налево, например, на арабском или иврите. Следующий пример демонстрирует, как применить ExactPhraseRedaction к PDF‑документу на арабском языке:

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.options import SaveOptions
from groupdocs.redaction.redactions import ExactPhraseRedaction, ReplacementOptions

def redact_right_to_left_text():
    # Укажите параметры редактирования с помощью арабской фразы
    repl_opt = ReplacementOptions("[test]")
    ex_red = ExactPhraseRedaction("انتقد", repl_opt)

    # Загрузите документ для редактирования
    with Redactor("./arabic.pdf") as redactor:
        # Применить редактирование
        result = redactor.apply(ex_red)

        # Сохраните отредактированный документ рядом с исходным файлом
        so = SaveOptions()
        so.add_suffix = True
        so.rasterize_to_pdf = False
        so.redacted_file_suffix = "redacted"
        redactor.save(so)

if __name__ == "__main__":
    redact_right_to_left_text()
```

`arabic.pdf` — это пример файла, используемый в этом примере. Нажмите [здесь](https://docs.groupdocs.com/redaction/python-net/_sample_files/developer-guide/basic-usage/text-redactions/arabic.pdf), чтобы скачать его.

  
```text
Binary file (PDF, 23 KB)
```
[Download full output](https://docs.groupdocs.com/redaction/python-net/_output_files/developer-guide/basic-usage/text-redactions/redact_right_to_left_text/arabic_redacted.pdf)

## Use regular expression

Внутри процесс редактирования «exact phrase» работает через регулярные выражения, которые являются базовым подходом к редактированию. В приведённом ниже примере мы удаляем любой текст, соответствующий шаблону "2 цифры, пробел или ничего, 2 цифры, снова пробел и 6 цифр", с помощью синего цветного блока:

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.options import SaveOptions
from groupdocs.redaction.redactions import RegexRedaction, ReplacementOptions
from groupdocs.pydrawing import Color

def redact_with_regex():
    # Определите цвет блока редактирования
    color = Color.from_argb(255, 220, 20, 60)

    # Укажите параметры редактирования
    repl_opt = ReplacementOptions(color)
    reg_red = RegexRedaction("\\d{2}\\s*\\d{2}[^\\d]*\\d{6}", repl_opt)

    # Загрузите документ для редактирования
    with Redactor("./sample.docx") as redactor:
        # Применить редактирование
        result = redactor.apply(reg_red)

        # Сохраните отредактированный документ рядом с исходным файлом
        so = SaveOptions()
        so.add_suffix = True
        so.rasterize_to_pdf = False
        so.redacted_file_suffix = "redacted"
        redactor.save(so)

if __name__ == "__main__":
    redact_with_regex()
```

`sample.docx` — это пример файла, используемый в этом примере. Нажмите [здесь](https://docs.groupdocs.com/redaction/python-net/_sample_files/developer-guide/basic-usage/text-redactions/sample.docx) для его загрузки.

  
```text
Binary file (DOCX, 16 KB)
```
[Download full output](https://docs.groupdocs.com/redaction/python-net/_output_files/developer-guide/basic-usage/text-redactions/redact_with_regex/sample_redacted.docx)

Если вам нужно применить редактирование к целому абзацу, возможно, вам также понадобится использовать RegexRedaction. Следующий пример демонстрирует, как отредактировать весь абзац в PDF‑документе:

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.options import SaveOptions
from groupdocs.redaction.redactions import RegexRedaction, ReplacementOptions
from groupdocs.pydrawing import Color

def redact_whole_paragraph():
    # Определите цвет блока редактирования
    color = Color.from_argb(255, 220, 20, 60)

    # Укажите параметры редактирования, соответствующие целому абзацу
    repl_opt = ReplacementOptions(color)
    reg_red = RegexRedaction("(Lorem(\n|.)+?urna)", repl_opt)

    # Загрузите документ для редактирования
    with Redactor("./sample.pdf") as redactor:
        # Применить редактирование
        result = redactor.apply(reg_red)

        # Сохраните отредактированный документ рядом с исходным файлом
        so = SaveOptions()
        so.add_suffix = True
        so.rasterize_to_pdf = False
        so.redacted_file_suffix = "redacted"
        redactor.save(so)

if __name__ == "__main__":
    redact_whole_paragraph()
```

`sample.pdf` — это пример файла, используемый в этом примере. Нажмите [здесь](https://docs.groupdocs.com/redaction/python-net/_sample_files/developer-guide/basic-usage/text-redactions/sample.pdf), чтобы скачать его.

  
```text
Binary file (PDF, 68 KB)
```
[Download full output](https://docs.groupdocs.com/redaction/python-net/_output_files/developer-guide/basic-usage/text-redactions/redact_whole_paragraph/sample_redacted.pdf)
