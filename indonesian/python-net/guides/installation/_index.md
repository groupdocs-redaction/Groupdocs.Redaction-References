---
title: "Instal GroupDocs.Redaction untuk Python via .NET"
linkTitle: "Installation"
second_title: "Referensi API GroupDocs.Redaction untuk Python via .NET"
description: "Instal GroupDocs.Redaction untuk Python via .NET di Windows, Linux, atau macOS — dari PyPI atau dari wheel yang sudah diunduh sebelumnya, termasuk build untuk Intel dan Apple Silicon."
type: docs
url: /id/python-net/guides/installation/
is_root: false
weight: 10
---


GroupDocs.Redaction untuk Python via .NET didistribusikan sebagai wheel pra-bangun di [PyPI](https://pypi.org/project/groupdocs-redaction-net/). Indeks PyPI menyimpan wheel terpisah untuk setiap platform yang didukung, dan `pip` secara otomatis memilih yang tepat. Setiap wheel bersifat mandiri: ia menyertakan runtime terbenam dan semua dependensi yang dikelola, sehingga tidak diperlukan instalasi Microsoft Office, OpenOffice, Adobe Acrobat, atau runtime terpisah.

Sebelum menginstal, pastikan lingkungan Anda cocok dengan platform yang didukung dan versi Python yang tercantum dalam topik [System Requirements]().

## Install Package from PyPI

Buka terminal dan jalankan perintah instalasi untuk platform Anda:

```ps
py -m pip install groupdocs-redaction-net
```

```bash
python3 -m pip install groupdocs-redaction-net
```

```bash
python3 -m pip install groupdocs-redaction-net
```

Setelah menjalankan perintah, Anda akan melihat output serupa dengan:

```bash
Collecting groupdocs-redaction-net
  Downloading groupdocs_redaction_net-26.6.0-py3-none-win_amd64.whl.metadata (3.0 kB)
  Downloading groupdocs_redaction_net-26.6.0-py3-none-win_amd64.whl (40.0 MB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 40.0/40.0 MB 2.8 MB/s eta 0:00:00
Installing collected packages: groupdocs-redaction-net
Successfully installed groupdocs-redaction-net-26.6.0
```

Nama file wheel akan menyertakan sufiks platform yang cocok dengan sistem operasi Anda — misalnya `manylinux1_x86_64` pada Ubuntu/Debian, `macosx_11_0_arm64` pada Apple Silicon, atau `win_amd64` pada Windows 64-bit.

## Add the Package to `requirements.txt`

Untuk lingkungan yang dapat direproduksi, tentukan versi paket dalam `requirements.txt` Anda:

```txt
groupdocs-redaction-net==26.6.0
```

Kemudian instal semua dependensi dalam satu langkah:

```bash
pip install -r requirements.txt
```

## Install from a Pre-Downloaded Wheel

Jika lingkungan build Anda tidak dapat mengakses PyPI, unduh wheel yang sesuai dari [situs web GroupDocs Releases](https://releases.groupdocs.com/redaction/python-net/) dan instal secara lokal. Wheel dipublikasikan untuk empat platform berikut:

- **Windows 64-bit**: file name ends with `win_amd64.whl`
- **Linux x64 (glibc)**: file name ends with `manylinux1_x86_64.whl`
- **macOS Intel**: file name ends with `macosx_10_14_x86_64.whl`
- **macOS Apple Silicon**: file name ends with `macosx_11_0_arm64.whl`

Letakkan wheel yang diunduh ke dalam folder proyek Anda, lalu instal:

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

Output yang diharapkan:

```bash
Processing ./groupdocs_redaction_net-26.6.0-py3-none-*.whl
Installing collected packages: groupdocs-redaction-net
Successfully installed groupdocs-redaction-net-26.6.0
```

## Platform Prerequisites

Di Windows tidak diperlukan langkah tambahan. Di Linux dan macOS, instal pustaka native yang dibutuhkan oleh mesin rendering:

```bash
apt install libgdiplus libfontconfig1 libicu-dev ttf-mscorefonts-installer
```

```bash
brew install mono-libgdiplus
```

Pada versi 26.6.0, **rasterisasi ke PDF dan redaksi area gambar hanya berjalan di Windows** — di Linux/macOS mereka menghasilkan `System.PlatformNotSupportedException`, dan paket native di atas tidak mengangkat pembatasan tersebut. Redaksi teks, metadata, anotasi, dan halaman serta penyimpanan format asli berfungsi di setiap platform. Lihat [System Requirements]() untuk matriks dukungan fitur lengkap.

## Verify the Installation

Pastikan paket diimpor dengan benar dan periksa versi yang terinstal:

```bash
python -c "import groupdocs.redaction; print('GroupDocs.Redaction is ready')"
```

Anda juga dapat menampilkan paket yang terinstal dengan `pip show groupdocs-redaction-net` untuk mengonfirmasi versi dan lokasinya.

## Next Steps

- Follow the [Hello, World!]() guide to run your first redaction.
- Read the [Features Overview]() to see everything you can redact.
- Clone the [examples repository](https://github.com/groupdocs-redaction/GroupDocs.Redaction-for-Python-via-.NET) and read [How to Run Examples]() to try every documented scenario locally.
