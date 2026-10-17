---
title: "Installa GroupDocs.Redaction per Python via .NET"
linkTitle: "Installation"
second_title: "Riferimenti API di GroupDocs.Redaction per Python tramite .NET"
description: "Installa GroupDocs.Redaction per Python via .NET su Windows, Linux o macOS — da PyPI o da una wheel pre‑scaricata, includendo build per Intel e Apple Silicon."
type: docs
url: /it/python-net/guides/installation/
is_root: false
weight: 10
---


GroupDocs.Redaction per Python via .NET è distribuito come una wheel pre-costruita su [PyPI](https://pypi.org/project/groupdocs-redaction-net/). L'indice PyPI ospita una wheel separata per ogni piattaforma supportata, e `pip` seleziona automaticamente quella corretta. Ogni wheel è autonomo: include il runtime incorporato e tutte le dipendenze gestite, quindi non è necessario installare Microsoft Office, OpenOffice, Adobe Acrobat o un runtime separato.

Prima dell'installazione, verifica che il tuo ambiente corrisponda alle piattaforme supportate e alle versioni Python elencate nella sezione [System Requirements]().

## Install Package from PyPI

Apri un terminale ed esegui il comando di installazione per la tua piattaforma:

```ps
py -m pip install groupdocs-redaction-net
```

```bash
python3 -m pip install groupdocs-redaction-net
```

```bash
python3 -m pip install groupdocs-redaction-net
```

Dopo aver eseguito il comando dovresti vedere un output simile a:

```bash
Collecting groupdocs-redaction-net
  Downloading groupdocs_redaction_net-26.6.0-py3-none-win_amd64.whl.metadata (3.0 kB)
  Downloading groupdocs_redaction_net-26.6.0-py3-none-win_amd64.whl (40.0 MB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 40.0/40.0 MB 2.8 MB/s eta 0:00:00
Installing collected packages: groupdocs-redaction-net
Successfully installed groupdocs-redaction-net-26.6.0
```

Il nome del file wheel includerà un suffisso di piattaforma che corrisponde al tuo sistema operativo — ad esempio `manylinux1_x86_64` su Ubuntu/Debian, `macosx_11_0_arm64` su Apple Silicon, o `win_amd64` su Windows a 64 bit.

## Add the Package to `requirements.txt`

Per ambienti riproducibili, fissa la versione del pacchetto nel tuo `requirements.txt`:

```txt
groupdocs-redaction-net==26.6.0
```

Quindi installa tutte le dipendenze in un unico passaggio:

```bash
pip install -r requirements.txt
```

## Install from a Pre-Downloaded Wheel

Se il tuo ambiente di compilazione non può raggiungere PyPI, scarica la wheel appropriata dal [GroupDocs Releases website](https://releases.groupdocs.com/redaction/python-net/) e installala localmente. Le wheel sono pubblicate per le seguenti quattro piattaforme:

- **Windows 64-bit**: file name ends with `win_amd64.whl`
- **Linux x64 (glibc)**: file name ends with `manylinux1_x86_64.whl`
- **macOS Intel**: file name ends with `macosx_10_14_x86_64.whl`
- **macOS Apple Silicon**: file name ends with `macosx_11_0_arm64.whl`

Posiziona la wheel scaricata nella cartella del tuo progetto, quindi installala:

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

Output previsto:

```bash
Processing ./groupdocs_redaction_net-26.6.0-py3-none-*.whl
Installing collected packages: groupdocs-redaction-net
Successfully installed groupdocs-redaction-net-26.6.0
```

## Platform Prerequisites

Su Windows non sono necessari passaggi aggiuntivi. Su Linux e macOS, installa le librerie native da cui dipende il motore di rendering:

```bash
apt install libgdiplus libfontconfig1 libicu-dev ttf-mscorefonts-installer
```

```bash
brew install mono-libgdiplus
```

Nella versione 26.6.0, **la rasterizzazione in PDF e la redazione di aree immagine funzionano solo su Windows** — su Linux/macOS generano `System.PlatformNotSupportedException`, e i pacchetti nativi sopra menzionati non rimuovono tale limitazione. Testo, metadati, annotazioni e redazione di pagine e salvataggi in formato originale funzionano su tutte le piattaforme. Consulta [System Requirements]() per la matrice completa di supporto delle funzionalità.

## Verify the Installation

Conferma che il pacchetto sia stato importato correttamente e controlla la versione installata:

```bash
python -c "import groupdocs.redaction; print('GroupDocs.Redaction is ready')"
```

Puoi anche elencare il pacchetto installato con `pip show groupdocs-redaction-net` per confermare la versione e la posizione.

## Next Steps

- Follow the [Hello, World!]() guide to run your first redaction.
- Read the [Features Overview]() to see everything you can redact.
- Clone the [examples repository](https://github.com/groupdocs-redaction/GroupDocs.Redaction-for-Python-via-.NET) and read [How to Run Examples]() to try every documented scenario locally.
