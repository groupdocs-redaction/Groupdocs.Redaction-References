---
title: "Εγκαταστήστε το GroupDocs.Redaction for Python via .NET"
linkTitle: "Installation"
second_title: "Αναφορές API του GroupDocs.Redaction για Python μέσω .NET"
description: "Εγκαταστήστε το GroupDocs.Redaction for Python via .NET σε Windows, Linux ή macOS — από το PyPI ή από προ‑κατεβασμένο wheel, συμπεριλαμβανομένων των εκδόσεων για Intel και Apple Silicon."
type: docs
url: /el/python-net/guides/installation/
is_root: false
weight: 10
---


Το GroupDocs.Redaction για Python μέσω .NET διανέμεται ως προ-κατασκευασμένο wheel στο [PyPI](https://pypi.org/project/groupdocs-redaction-net/). Ο δείκτης PyPI φιλοξενεί ένα ξεχωριστό wheel για κάθε υποστηριζόμενη πλατφόρμα, και το `pip` επιλέγει αυτόματα το σωστό. Κάθε wheel είναι αυτόνομο: περιλαμβάνει το ενσωματωμένο runtime και όλες τις διαχειριζόμενες εξαρτήσεις, έτσι δεν απαιτείται εγκατάσταση του Microsoft Office, OpenOffice, Adobe Acrobat ή ξεχωριστού runtime.

Πριν από την εγκατάσταση, επιβεβαιώστε ότι το περιβάλλον σας ταιριάζει με τις υποστηριζόμενες πλατφόρμες και τις εκδόσεις Python που αναφέρονται στο θέμα [System Requirements]().

## Install Package from PyPI

Ανοίξτε ένα τερματικό και εκτελέστε την εντολή εγκατάστασης για την πλατφόρμα σας:

```ps
py -m pip install groupdocs-redaction-net
```

```bash
python3 -m pip install groupdocs-redaction-net
```

```bash
python3 -m pip install groupdocs-redaction-net
```

Μετά την εκτέλεση της εντολής, θα πρέπει να δείτε έξοδο παρόμοια με:

```bash
Collecting groupdocs-redaction-net
  Downloading groupdocs_redaction_net-26.6.0-py3-none-win_amd64.whl.metadata (3.0 kB)
  Downloading groupdocs_redaction_net-26.6.0-py3-none-win_amd64.whl (40.0 MB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 40.0/40.0 MB 2.8 MB/s eta 0:00:00
Installing collected packages: groupdocs-redaction-net
Successfully installed groupdocs-redaction-net-26.6.0
```

Το όνομα του αρχείου wheel θα περιλαμβάνει ένα επίθημα πλατφόρμας που ταιριάζει με το λειτουργικό σας σύστημα — για παράδειγμα `manylinux1_x86_64` σε Ubuntu/Debian, `macosx_11_0_arm64` σε Apple Silicon ή `win_amd64` σε 64-bit Windows.

## Add the Package to `requirements.txt`

Για αναπαραγώγιμα περιβάλλοντα, καθορίστε την έκδοση του πακέτου στο `requirements.txt`:

```txt
groupdocs-redaction-net==26.6.0
```

Στη συνέχεια εγκαταστήστε όλες τις εξαρτήσεις σε ένα βήμα:

```bash
pip install -r requirements.txt
```

## Install from a Pre-Downloaded Wheel

Εάν το περιβάλλον κατασκευής σας δεν μπορεί να προσεγγίσει το PyPI, κατεβάστε το κατάλληλο wheel από τον ιστότοπο [GroupDocs Releases website](https://releases.groupdocs.com/redaction/python-net/) και εγκαταστήστε το τοπικά. Τα wheels δημοσιεύονται για τις ακόλουθες τέσσερις πλατφόρμες:

- **Windows 64-bit**: file name ends with `win_amd64.whl`
- **Linux x64 (glibc)**: file name ends with `manylinux1_x86_64.whl`
- **macOS Intel**: file name ends with `macosx_10_14_x86_64.whl`
- **macOS Apple Silicon**: file name ends with `macosx_11_0_arm64.whl`

Τοποθετήστε το ληφθέν wheel στον φάκελο του έργου σας, στη συνέχεια εγκαταστήστε το:

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

Αναμενόμενη έξοδος:

```bash
Processing ./groupdocs_redaction_net-26.6.0-py3-none-*.whl
Installing collected packages: groupdocs-redaction-net
Successfully installed groupdocs-redaction-net-26.6.0
```

## Platform Prerequisites

Στα Windows δεν απαιτούνται επιπλέον βήματα. Στα Linux και macOS, εγκαταστήστε τις εγγενείς βιβλιοθήκες από τις οποίες εξαρτάται η μηχανή απόδοσης:

```bash
apt install libgdiplus libfontconfig1 libicu-dev ttf-mscorefonts-installer
```

```bash
brew install mono-libgdiplus
```

Στην έκδοση 26.6.0, **rasterization to PDF and image-area redaction run only on Windows** — σε Linux/macOS προκαλούν `System.PlatformNotSupportedException`, και τα παραπάνω εγγενή πακέτα δεν αφαιρούν αυτόν τον περιορισμό. Η επεξεργασία κειμένου, μεταδεδομένων, σχολίων και σελίδων καθώς και η αποθήκευση σε αρχικό μορφότυπο λειτουργούν σε κάθε πλατφόρμα. Δείτε το [System Requirements]() για τον πλήρη πίνακα υποστήριξης χαρακτηριστικών.

## Verify the Installation

Επιβεβαιώστε ότι το πακέτο εισήχθη σωστά και ελέγξτε την εγκατεστημένη έκδοση:

```bash
python -c "import groupdocs.redaction; print('GroupDocs.Redaction is ready')"
```

Μπορείτε επίσης να εμφανίσετε το εγκατεστημένο πακέτο με `pip show groupdocs-redaction-net` για να επιβεβαιώσετε την έκδοση και την τοποθεσία.

## Next Steps

- Follow the [Hello, World!]() guide to run your first redaction.
- Read the [Features Overview]() to see everything you can redact.
- Clone the [examples repository](https://github.com/groupdocs-redaction/GroupDocs.Redaction-for-Python-via-.NET) and read [How to Run Examples]() to try every documented scenario locally.
