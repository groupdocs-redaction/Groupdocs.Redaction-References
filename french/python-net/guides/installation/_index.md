---
title: "Installez GroupDocs.Redaction for Python via .NET"
linkTitle: "Installation"
second_title: "Références API de GroupDocs.Redaction pour Python via .NET"
description: "Installez GroupDocs.Redaction for Python via .NET sur Windows, Linux ou macOS — depuis PyPI ou depuis une roue pré‑téléchargée, incluant les versions Intel et Apple Silicon."
type: docs
url: /fr/python-net/guides/installation/
is_root: false
weight: 10
---


GroupDocs.Redaction pour Python via .NET est distribué sous forme de roue pré‑construite sur [PyPI](https://pypi.org/project/groupdocs-redaction-net/). L'index PyPI héberge une roue distincte pour chaque plateforme prise en charge, et `pip` sélectionne automatiquement la bonne. Chaque roue est autonome : elle regroupe le runtime intégré et toutes les dépendances gérées, de sorte qu'aucune installation de Microsoft Office, OpenOffice, Adobe Acrobat ou d’un runtime séparé n’est requise.

Avant l'installation, confirmez que votre environnement correspond aux plateformes prises en charge et aux versions de Python répertoriées dans le sujet [System Requirements]().

## Install Package from PyPI

Ouvrez un terminal et exécutez la commande d'installation pour votre plateforme :

```ps
py -m pip install groupdocs-redaction-net
```

```bash
python3 -m pip install groupdocs-redaction-net
```

```bash
python3 -m pip install groupdocs-redaction-net
```

Après avoir exécuté la commande, vous devriez voir une sortie similaire à :

```bash
Collecting groupdocs-redaction-net
  Downloading groupdocs_redaction_net-26.6.0-py3-none-win_amd64.whl.metadata (3.0 kB)
  Downloading groupdocs_redaction_net-26.6.0-py3-none-win_amd64.whl (40.0 MB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 40.0/40.0 MB 2.8 MB/s eta 0:00:00
Installing collected packages: groupdocs-redaction-net
Successfully installed groupdocs-redaction-net-26.6.0
```

Le nom du fichier de roue comprendra un suffixe de plateforme correspondant à votre système d'exploitation — par exemple `manylinux1_x86_64` sur Ubuntu/Debian, `macosx_11_0_arm64` sur Apple Silicon, ou `win_amd64` sur Windows 64 bits.

## Add the Package to `requirements.txt`

Pour des environnements reproductibles, épinglez la version du paquet dans votre `requirements.txt` :

```txt
groupdocs-redaction-net==26.6.0
```

Ensuite, installez toutes les dépendances en une seule étape :

```bash
pip install -r requirements.txt
```

## Install from a Pre-Downloaded Wheel

Si votre environnement de construction ne peut pas accéder à PyPI, téléchargez la roue appropriée depuis le [site des releases GroupDocs](https://releases.groupdocs.com/redaction/python-net/) et installez‑la localement. Les roues sont publiées pour les quatre plateformes suivantes :

- **Windows 64-bit**: file name ends with `win_amd64.whl`
- **Linux x64 (glibc)**: file name ends with `manylinux1_x86_64.whl`
- **macOS Intel**: file name ends with `macosx_10_14_x86_64.whl`
- **macOS Apple Silicon**: file name ends with `macosx_11_0_arm64.whl`

Placez la roue téléchargée dans le dossier de votre projet, puis installez‑la :

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

Sortie attendue :

```bash
Processing ./groupdocs_redaction_net-26.6.0-py3-none-*.whl
Installing collected packages: groupdocs-redaction-net
Successfully installed groupdocs-redaction-net-26.6.0
```

## Platform Prerequisites

Sur Windows, aucune étape supplémentaire n’est requise. Sur Linux et macOS, installez les bibliothèques natives dont dépend le moteur de rendu :

```bash
apt install libgdiplus libfontconfig1 libicu-dev ttf-mscorefonts-installer
```

```bash
brew install mono-libgdiplus
```

Dans la version 26.6.0, **la rasterisation en PDF et la rédaction de zones d’image ne fonctionnent que sous Windows** — sous Linux/macOS elles lèvent `System.PlatformNotSupportedException`, et les packages natifs ci‑dessus ne suppriment pas cette restriction. La rédaction de texte, métadonnées, annotations et pages ainsi que les sauvegardes au format original fonctionnent sur toutes les plateformes. Consultez [System Requirements]() pour la matrice complète de prise en charge des fonctionnalités.

## Verify the Installation

Confirmez que le paquet a été importé correctement et vérifiez la version installée :

```bash
python -c "import groupdocs.redaction; print('GroupDocs.Redaction is ready')"
```

Vous pouvez également lister le paquet installé avec `pip show groupdocs-redaction-net` pour confirmer la version et l’emplacement.

## Next Steps

- Follow the [Hello, World!]() guide to run your first redaction.
- Read the [Features Overview]() to see everything you can redact.
- Clone the [examples repository](https://github.com/groupdocs-redaction/GroupDocs.Redaction-for-Python-via-.NET) and read [How to Run Examples]() to try every documented scenario locally.
