---
title: "Installeer GroupDocs.Redaction voor Python via .NET"
linkTitle: "Installation"
second_title: "GroupDocs.Redaction voor Python via .NET API-referenties"
description: "Installeer GroupDocs.Redaction voor Python via .NET op Windows, Linux of macOS — vanaf PyPI of vanaf een vooraf gedownloade wheel, inclusief builds voor Intel en Apple Silicon."
type: docs
url: /nl/python-net/guides/installation/
is_root: false
weight: 10
---


GroupDocs.Redaction voor Python via .NET wordt gedistribueerd als een vooraf gebouwde wheel op [PyPI](https://pypi.org/project/groupdocs-redaction-net/). De PyPI-index host een aparte wheel voor elk ondersteund platform, en `pip` kiest automatisch de juiste. Elke wheel is zelfvoorzienend: hij bundelt de ingebedde runtime en elke beheerde afhankelijkheid, zodat geen Microsoft Office, OpenOffice, Adobe Acrobat, of aparte runtime‑installatie nodig is.

Controleer vóór het installeren of uw omgeving overeenkomt met de ondersteunde platforms en Python‑versies die vermeld staan in het onderwerp [System Requirements]().

## Install Package from PyPI

Open een terminal en voer het installatie‑commando voor uw platform uit:

```ps
py -m pip install groupdocs-redaction-net
```

```bash
python3 -m pip install groupdocs-redaction-net
```

```bash
python3 -m pip install groupdocs-redaction-net
```

Na het uitvoeren van het commando zou u output moeten zien die lijkt op:

```bash
Collecting groupdocs-redaction-net
  Downloading groupdocs_redaction_net-26.6.0-py3-none-win_amd64.whl.metadata (3.0 kB)
  Downloading groupdocs_redaction_net-26.6.0-py3-none-win_amd64.whl (40.0 MB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 40.0/40.0 MB 2.8 MB/s eta 0:00:00
Installing collected packages: groupdocs-redaction-net
Successfully installed groupdocs-redaction-net-26.6.0
```

De bestandsnaam van de wheel bevat een platformsuffix die overeenkomt met uw besturingssysteem — bijvoorbeeld `manylinux1_x86_64` op Ubuntu/Debian, `macosx_11_0_arm64` op Apple Silicon, of `win_amd64` op 64‑bit Windows.

## Add the Package to `requirements.txt`

Voor reproduceerbare omgevingen, pin de pakketversie in uw `requirements.txt`:

```txt
groupdocs-redaction-net==26.6.0
```

Installeer vervolgens alle afhankelijkheden in één stap:

```bash
pip install -r requirements.txt
```

## Install from a Pre-Downloaded Wheel

Als uw build‑omgeving geen toegang heeft tot PyPI, download dan de juiste wheel van de [GroupDocs Releases website](https://releases.groupdocs.com/redaction/python-net/) en installeer deze lokaal. Wheels worden gepubliceerd voor de volgende vier platforms:

- **Windows 64-bit**: file name ends with `win_amd64.whl`
- **Linux x64 (glibc)**: file name ends with `manylinux1_x86_64.whl`
- **macOS Intel**: file name ends with `macosx_10_14_x86_64.whl`
- **macOS Apple Silicon**: file name ends with `macosx_11_0_arm64.whl`

Plaats de gedownloade wheel in uw projectmap en installeer deze vervolgens:

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

Verwachte output:

```bash
Processing ./groupdocs_redaction_net-26.6.0-py3-none-*.whl
Installing collected packages: groupdocs-redaction-net
Successfully installed groupdocs-redaction-net-26.6.0
```

## Platform Prerequisites

Op Windows zijn geen extra stappen vereist. Op Linux en macOS installeert u de native bibliotheken waar de rendering‑engine van afhankelijk is:

```bash
apt install libgdiplus libfontconfig1 libicu-dev ttf-mscorefonts-installer
```

```bash
brew install mono-libgdiplus
```

In versie 26.6.0, **rasterization to PDF and image-area redaction run only on Windows** — op Linux/macOS veroorzaken ze een `System.PlatformNotSupportedException`, en de bovenstaande native pakketten heffen die beperking niet op. Tekst, metadata, annotatie en paginaredactie en opslaan in oorspronkelijke indeling werken op elk platform. Zie [System Requirements]() voor de volledige functie‑ondersteuningsmatrix.

## Verify the Installation

Bevestig dat het pakket correct is geïmporteerd en controleer de geïnstalleerde versie:

```bash
python -c "import groupdocs.redaction; print('GroupDocs.Redaction is ready')"
```

U kunt ook het geïnstalleerde pakket weergeven met `pip show groupdocs-redaction-net` om de versie en locatie te bevestigen.

## Next Steps

- Follow the [Hello, World!]() guide to run your first redaction.
- Read the [Features Overview]() to see everything you can redact.
- Clone the [examples repository](https://github.com/groupdocs-redaction/GroupDocs.Redaction-for-Python-via-.NET) and read [How to Run Examples]() to try every documented scenario locally.
