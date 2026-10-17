---
title: "Установите GroupDocs.Redaction для Python через .NET"
linkTitle: "Installation"
second_title: "GroupDocs.Redaction для Python через .NET справочник API"
description: "Установите GroupDocs.Redaction для Python через .NET на Windows, Linux или macOS — из PyPI или из предварительно загруженного wheel, включая сборки для Intel и Apple Silicon."
type: docs
url: /ru/python-net/guides/installation/
is_root: false
weight: 10
---


GroupDocs.Redaction для Python через .NET распространяется в виде готового wheel на [PyPI](https://pypi.org/project/groupdocs-redaction-net/). Индекс PyPI содержит отдельный wheel для каждой поддерживаемой платформы, и `pip` автоматически выбирает нужный. Каждый wheel самодостаточен: он включает встроенную среду выполнения и все управляемые зависимости, поэтому установка Microsoft Office, OpenOffice, Adobe Acrobat или отдельной среды выполнения не требуется.

Перед установкой убедитесь, что ваша среда соответствует поддерживаемым платформам и версиям Python, перечисленным в разделе [System Requirements]().

## Install Package from PyPI

Откройте терминал и выполните команду установки для вашей платформы:

```ps
py -m pip install groupdocs-redaction-net
```

```bash
python3 -m pip install groupdocs-redaction-net
```

```bash
python3 -m pip install groupdocs-redaction-net
```

После выполнения команды вы должны увидеть вывод, похожий на:

```bash
Collecting groupdocs-redaction-net
  Downloading groupdocs_redaction_net-26.6.0-py3-none-win_amd64.whl.metadata (3.0 kB)
  Downloading groupdocs_redaction_net-26.6.0-py3-none-win_amd64.whl (40.0 MB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 40.0/40.0 MB 2.8 MB/s eta 0:00:00
Installing collected packages: groupdocs-redaction-net
Successfully installed groupdocs-redaction-net-26.6.0
```

Имя файла wheel будет содержать суффикс платформы, соответствующий вашей операционной системе — например `manylinux1_x86_64` на Ubuntu/Debian, `macosx_11_0_arm64` на Apple Silicon или `win_amd64` на 64‑разрядном Windows.

## Add the Package to `requirements.txt`

Для воспроизводимых сред зафиксируйте версию пакета в файле `requirements.txt`:

```txt
groupdocs-redaction-net==26.6.0
```

Затем установите все зависимости одним шагом:

```bash
pip install -r requirements.txt
```

## Install from a Pre-Downloaded Wheel

Если ваша среда сборки не может получить доступ к PyPI, скачайте соответствующий wheel с сайта [GroupDocs Releases website](https://releases.groupdocs.com/redaction/python-net/) и установите его локально. Wheels публикуются для следующих четырёх платформ:

- **Windows 64-bit**: file name ends with `win_amd64.whl`
- **Linux x64 (glibc)**: file name ends with `manylinux1_x86_64.whl`
- **macOS Intel**: file name ends with `macosx_10_14_x86_64.whl`
- **macOS Apple Silicon**: file name ends with `macosx_11_0_arm64.whl`

Поместите загруженный wheel в папку проекта, затем установите его:

```ps
py -m pip install ./groupdocs_redaction_net-26.6.0-py3-none-win_amd64.whl
```

```bash
python3 -m pip install ./groupdocs_redaction_net-26.6.0-py3-none-manylinux1_x86_64.whl
```

```bash
python3 -m pip install ./groupdocs_redaction_net-26.6.0-py3-none-macosx_10_14_x86_64.whl
```

```bash
python3 -m pip install ./groupdocs_redaction_net-26.6.0-py3-none-macosx_11_0_arm64.whl
```

Ожидаемый вывод:

```bash
Processing ./groupdocs_redaction_net-26.6.0-py3-none-*.whl
Installing collected packages: groupdocs-redaction-net
Successfully installed groupdocs-redaction-net-26.6.0
```

## Platform Prerequisites

В Windows дополнительные шаги не требуются. В Linux и macOS установите нативные библиотеки, от которых зависит движок рендеринга:

```bash
apt install libgdiplus libfontconfig1 libicu-dev ttf-mscorefonts-installer
```

```bash
brew install mono-libgdiplus
```

В версии 26.6.0, **rasterization to PDF and image-area redaction run only on Windows** — в Linux/macOS они вызывают `System.PlatformNotSupportedException`, и перечисленные выше нативные пакеты не снимают это ограничение. Текстовая, метаданные, аннотации, редактирование страниц и сохранение в оригинальном формате работают на любой платформе. См. [System Requirements]() для полной матрицы поддержки функций.

## Verify the Installation

Убедитесь, что пакет импортирован корректно, и проверьте установленную версию:

```bash
python -c "import groupdocs.redaction; print('GroupDocs.Redaction is ready')"
```

Вы также можете вывести список установленного пакета с помощью `pip show groupdocs-redaction-net`, чтобы подтвердить версию и расположение.

## Next Steps

- Follow the [Hello, World!]() guide to run your first redaction.
- Read the [Features Overview]() to see everything you can redact.
- Clone the [examples repository](https://github.com/groupdocs-redaction/GroupDocs.Redaction-for-Python-via-.NET) and read [How to Run Examples]() to try every documented scenario locally.
