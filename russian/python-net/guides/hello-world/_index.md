---
title: "Привет, мир!"
linkTitle: "Hello, World!"
second_title: "GroupDocs.Redaction для Python через .NET справочник API"
description: "Быстро начните работу с GroupDocs.Redaction for Python via .NET, создав и запустив простой пример."
type: docs
url: /ru/python-net/guides/hello-world/
is_root: false
weight: 20
---


## Introduction
Пример "Hello, World!" часто является первым шагом при изучении GroupDocs.Redaction for Python via .NET. Он служит простым тестом, подтверждающим, что ваша среда разработки правильно настроена и библиотека работает как ожидается.

## Overview
GroupDocs.Redaction for Python via .NET позволяет выполнять поиск, редактирование и удаление конфиденциальной информации из различных форматов документов. Широкий набор [supported formats](https://docs.groupdocs.com/redaction/python-net/getting-started/supported-document-formats/) делает его универсальным для разных вариантов использования.

## How to redact a document
Следующие шаги демонстрируют, как редактировать конфиденциальную информацию в документе с помощью GroupDocs.Redaction for Python via .NET:

1. Импортируйте необходимые классы `groupdocs.redaction`.
2. Опишите редактирование (здесь — точную фразу, которую нужно заменить цветным прямоугольником).
3. Создайте экземпляр [`Redactor`](/redaction/python-net/groupdocs.redaction/redactor/) с путём к образцу документа.
4. Примените редактирование.
5. Сохраните результат.

## Complete example
Пример ниже заменяет каждое вхождение фразы "John Doe" полупрозрачным красным прямоугольником и сохраняет отредактированный документ:

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.options import SaveOptions
from groupdocs.redaction.redactions import ExactPhraseRedaction, ReplacementOptions
from groupdocs.pydrawing import Color

def hello_world():
    # Нарисуйте полупрозрачный красный прямоугольник над каждым вхождением "John Doe"
    options = ReplacementOptions(Color.from_argb(128, 255, 0, 0))
    redaction = ExactPhraseRedaction("John Doe", options)

    # Загрузите документ, примените редактирование и сохраните результат
    with Redactor("./sample.docx") as redactor:
        redactor.apply(redaction)
        save_options = SaveOptions()
        save_options.add_suffix = True
        save_options.rasterize_to_pdf = True
        save_options.redacted_file_suffix = "redacted"
        result_path = redactor.save(save_options)

    print(f"Document redacted successfully. Output saved to {result_path}.")

if __name__ == "__main__":
    hello_world()
```

`sample.docx` — пример файла, используемый в этом примере. Нажмите [here](https://docs.groupdocs.com/redaction/python-net/_sample_files/getting-started/hello-world/sample.docx), чтобы скачать его.

  
```text
Binary file (PDF, 1.0 MB)
```
[Download full output](https://docs.groupdocs.com/redaction/python-net/_output_files/getting-started/hello-world/hello_world/sample_redacted.pdf)

В этом примере результат растеризуется в PDF с именем `sample_redacted.pdf`, поэтому отредактированное содержимое нельзя восстановить (`save()` по умолчанию растеризует в PDF; параметр `redacted_file_suffix` лишь задаёт имя выходного файла). Чтобы сохранить исходный формат, установите `rasterize_to_pdf = False`.

## Additional resources
Эта демонстрация ссылается на GroupDocs.Redaction for Python via .NET [code samples](https://github.com/groupdocs-redaction/GroupDocs.Redaction-for-Python-via-.NET/).
