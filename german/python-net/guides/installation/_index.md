---
title: "Installieren Sie GroupDocs.Redaction für Python via .NET"
linkTitle: "Installation"
second_title: "GroupDocs.Redaction für Python über .NET API-Referenzen"
description: "Installieren Sie GroupDocs.Redaction für Python via .NET unter Windows, Linux oder macOS – von PyPI oder aus einem vorab heruntergeladenen Wheel, einschließlich Intel‑ und Apple‑Silicon‑Builds."
type: docs
url: /de/python-net/guides/installation/
is_root: false
weight: 10
---


GroupDocs.Redaction für Python via .NET wird als vorgefertigtes Wheel auf [PyPI](https://pypi.org/project/groupdocs-redaction-net/) verteilt. Der PyPI‑Index stellt für jede unterstützte Plattform ein separates Wheel bereit, und `pip` wählt automatisch das richtige aus. Jedes Wheel ist eigenständig: Es bündelt die eingebettete Laufzeit und alle verwalteten Abhängigkeiten, sodass keine Installation von Microsoft Office, OpenOffice, Adobe Acrobat oder einer separaten Laufzeit erforderlich ist.

Stellen Sie vor der Installation sicher, dass Ihre Umgebung den unterstützten Plattformen und Python‑Versionen entspricht, die im Thema [System Requirements]() aufgeführt sind.

## Install Package from PyPI

Öffnen Sie ein Terminal und führen Sie den Installationsbefehl für Ihre Plattform aus:

```ps
py -m pip install groupdocs-redaction-net
```

```bash
python3 -m pip install groupdocs-redaction-net
```

```bash
python3 -m pip install groupdocs-redaction-net
```

Nach dem Ausführen des Befehls sollten Sie eine Ausgabe ähnlich der folgenden sehen:

```bash
Collecting groupdocs-redaction-net
  Downloading groupdocs_redaction_net-26.6.0-py3-none-win_amd64.whl.metadata (3.0 kB)
  Downloading groupdocs_redaction_net-26.6.0-py3-none-win_amd64.whl (40.0 MB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 40.0/40.0 MB 2.8 MB/s eta 0:00:00
Installing collected packages: groupdocs-redaction-net
Successfully installed groupdocs-redaction-net-26.6.0
```

Der Wheel‑Dateiname enthält ein Plattform‑Suffix, das Ihrem Betriebssystem entspricht – zum Beispiel `manylinux1_x86_64` unter Ubuntu/Debian, `macosx_11_0_arm64` auf Apple‑Silicon oder `win_amd64` unter 64‑Bit‑Windows.

## Add the Package to `requirements.txt`

Für reproduzierbare Umgebungen sollten Sie die Paketversion in Ihrer `requirements.txt` festlegen:

```txt
groupdocs-redaction-net==26.6.0
```

Installieren Sie dann alle Abhängigkeiten in einem Schritt:

```bash
pip install -r requirements.txt
```

## Install from a Pre-Downloaded Wheel

Falls Ihre Build‑Umgebung PyPI nicht erreichen kann, laden Sie das passende Wheel von der [GroupDocs Releases website](https://releases.groupdocs.com/redaction/python-net/) herunter und installieren Sie es lokal. Wheels werden für die folgenden vier Plattformen bereitgestellt:

- **Windows 64-bit**: file name ends with `win_amd64.whl`
- **Linux x64 (glibc)**: file name ends with `manylinux1_x86_64.whl`
- **macOS Intel**: file name ends with `macosx_10_14_x86_64.whl`
- **macOS Apple Silicon**: file name ends with `macosx_11_0_arm64.whl`

Legen Sie das heruntergeladene Wheel in Ihren Projektordner und installieren Sie es anschließend:

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

Erwartete Ausgabe:

```bash
Processing ./groupdocs_redaction_net-26.6.0-py3-none-*.whl
Installing collected packages: groupdocs-redaction-net
Successfully installed groupdocs-redaction-net-26.6.0
```

## Platform Prerequisites

Unter Windows sind keine zusätzlichen Schritte erforderlich. Unter Linux und macOS installieren Sie die nativen Bibliotheken, von denen die Rendering‑Engine abhängt:

```bash
apt install libgdiplus libfontconfig1 libicu-dev ttf-mscorefonts-installer
```

```bash
brew install mono-libgdiplus
```

In Version 26.6.0 **läuft die Rasterisierung zu PDF und die Bildbereichs‑Redaktion nur unter Windows** – unter Linux/macOS wird eine `System.PlatformNotSupportedException` ausgelöst, und die oben genannten nativen Pakete heben diese Einschränkung nicht auf. Text‑, Metadaten‑, Annotations‑ und Seiten‑Redaktion sowie das Speichern im Originalformat funktionieren auf jeder Plattform. Siehe [System Requirements]() für die vollständige Funktions‑Unterstützungsmatrix.

## Verify the Installation

Bestätigen Sie, dass das Paket korrekt importiert wurde, und prüfen Sie die installierte Version:

```bash
python -c "import groupdocs.redaction; print('GroupDocs.Redaction is ready')"
```

Sie können das installierte Paket auch mit `pip show groupdocs-redaction-net` auflisten, um Version und Speicherort zu bestätigen.

## Next Steps

- Follow the [Hello, World!]() guide to run your first redaction.
- Read the [Features Overview]() to see everything you can redact.
- Clone the [examples repository](https://github.com/groupdocs-redaction/GroupDocs.Redaction-for-Python-via-.NET) and read [How to Run Examples]() to try every documented scenario locally.
