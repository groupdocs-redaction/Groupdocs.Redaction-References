---
title: "Installera GroupDocs.Redaction för Python via .NET"
linkTitle: "Installation"
second_title: "GroupDocs.Redaction för Python via .NET API-referenser"
description: "Installera GroupDocs.Redaction för Python via .NET på Windows, Linux eller macOS — från PyPI eller från ett förnedladdat wheel, inklusive Intel- och Apple Silicon‑byggversioner."
type: docs
url: /sv/python-net/guides/installation/
is_root: false
weight: 10
---


GroupDocs.Redaction för Python via .NET distribueras som ett förbyggt wheel på [PyPI](https://pypi.org/project/groupdocs-redaction-net/). PyPI-indexet innehåller ett separat wheel för varje stödd plattform, och `pip` väljer automatiskt rätt. Varje wheel är självständigt: det samlar den inbäddade runtime och alla hanterade beroenden, så ingen Microsoft Office, OpenOffice, Adobe Acrobat eller separat runtime‑installation krävs.

Innan installationen, bekräfta att din miljö matchar de stödda plattformarna och Python‑versionerna som listas i ämnet [Systemkrav]().

## Install Package from PyPI

Öppna en terminal och kör installationskommandot för din plattform:

```ps
py -m pip install groupdocs-redaction-net
```

```bash
python3 -m pip install groupdocs-redaction-net
```

```bash
python3 -m pip install groupdocs-redaction-net
```

Efter att ha kört kommandot bör du se en utskrift liknande:

```bash
Collecting groupdocs-redaction-net
  Downloading groupdocs_redaction_net-26.6.0-py3-none-win_amd64.whl.metadata (3.0 kB)
  Downloading groupdocs_redaction_net-26.6.0-py3-none-win_amd64.whl (40.0 MB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 40.0/40.0 MB 2.8 MB/s eta 0:00:00
Installing collected packages: groupdocs-redaction-net
Successfully installed groupdocs-redaction-net-26.6.0
```

Wheel‑filnamnet kommer att innehålla ett plattformsuffix som matchar ditt operativsystem — till exempel `manylinux1_x86_64` på Ubuntu/Debian, `macosx_11_0_arm64` på Apple Silicon eller `win_amd64` på 64‑bit Windows.

## Add the Package to `requirements.txt`

För reproducerbara miljöer, lås paketversionen i din `requirements.txt`:

```txt
groupdocs-redaction-net==26.6.0
```

Installera sedan alla beroenden i ett steg:

```bash
pip install -r requirements.txt
```

## Install from a Pre-Downloaded Wheel

Om din byggmiljö inte kan nå PyPI, ladda ner lämpligt wheel från [GroupDocs Releases-webbplatsen](https://releases.groupdocs.com/redaction/python-net/) och installera det lokalt. Wheels publiceras för följande fyra plattformar:

- **Windows 64-bit**: file name ends with `win_amd64.whl`
- **Linux x64 (glibc)**: file name ends with `manylinux1_x86_64.whl`
- **macOS Intel**: file name ends with `macosx_10_14_x86_64.whl`
- **macOS Apple Silicon**: file name ends with `macosx_11_0_arm64.whl`

Placera det nedladdade wheelet i din projektmapp och installera det sedan:

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

Förväntad utskrift:

```bash
Processing ./groupdocs_redaction_net-26.6.0-py3-none-*.whl
Installing collected packages: groupdocs-redaction-net
Successfully installed groupdocs-redaction-net-26.6.0
```

## Platform Prerequisites

På Windows krävs inga extra steg. På Linux och macOS, installera de inhemska biblioteken som renderingsmotorn är beroende av:

```bash
apt install libgdiplus libfontconfig1 libicu-dev ttf-mscorefonts-installer
```

```bash
brew install mono-libgdiplus
```

I version 26.6.0 kör **rasterisering till PDF och bildområde-redigering endast på Windows** — på Linux/macOS kastas `System.PlatformNotSupportedException`, och de inhemska paketen ovan lyfter inte den begränsningen. Text, metadata, annotationer och sidredigering samt sparande i originalformat fungerar på alla plattformar. Se [System Requirements]() för den fullständiga funktionsstödmatrixen.

## Verify the Installation

Bekräfta att paketet importerades korrekt och kontrollera den installerade versionen:

```bash
python -c "import groupdocs.redaction; print('GroupDocs.Redaction is ready')"
```

Du kan också lista det installerade paketet med `pip show groupdocs-redaction-net` för att bekräfta versionen och platsen.

## Next Steps

- Follow the [Hello, World!]() guide to run your first redaction.
- Read the [Features Overview]() to see everything you can redact.
- Clone the [examples repository](https://github.com/groupdocs-redaction/GroupDocs.Redaction-for-Python-via-.NET) and read [How to Run Examples]() to try every documented scenario locally.
