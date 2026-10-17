---
title: "GroupDocs.Redaction for Python via .NET'i kurun"
linkTitle: "Installation"
second_title: "GroupDocs.Redaction for Python via .NET API Referansları"
description: "Windows, Linux veya macOS üzerinde GroupDocs.Redaction for Python via .NET'i kurun — PyPI'dan veya önceden indirilmiş bir wheel'dan, Intel ve Apple Silicon sürümleri dahil."
type: docs
url: /tr/python-net/guides/installation/
is_root: false
weight: 10
---


GroupDocs.Redaction for Python via .NET, [PyPI](https://pypi.org/project/groupdocs-redaction-net/) üzerinde önceden derlenmiş bir tekerlek (wheel) olarak dağıtılır. PyPI dizini, desteklenen her platform için ayrı bir tekerlek barındırır ve `pip` doğru olanı otomatik olarak seçer. Her tekerlek kendi içinde bağımsızdır: gömülü çalışma zamanını ve tüm yönetilen bağımlılıkları paketler, böylece Microsoft Office, OpenOffice, Adobe Acrobat veya ayrı bir çalışma zamanı kurulumu gerekmez.

Kurulumdan önce, ortamınızın desteklenen platformlar ve [System Requirements]() konusunda listelenen Python sürümleriyle eşleştiğini doğrulayın.

## Install Package from PyPI

Bir terminal açın ve platformunuz için kurulum komutunu çalıştırın:

```ps
py -m pip install groupdocs-redaction-net
```

```bash
python3 -m pip install groupdocs-redaction-net
```

```bash
python3 -m pip install groupdocs-redaction-net
```

Komutu çalıştırdıktan sonra aşağıdakine benzer bir çıktı görmelisiniz:

```bash
Collecting groupdocs-redaction-net
  Downloading groupdocs_redaction_net-26.6.0-py3-none-win_amd64.whl.metadata (3.0 kB)
  Downloading groupdocs_redaction_net-26.6.0-py3-none-win_amd64.whl (40.0 MB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 40.0/40.0 MB 2.8 MB/s eta 0:00:00
Installing collected packages: groupdocs-redaction-net
Successfully installed groupdocs-redaction-net-26.6.0
```

Tekerlek dosya adı, işletim sisteminizle eşleşen bir platform soneki içerecektir — örneğin Ubuntu/Debian üzerinde `manylinux1_x86_64`, Apple Silicon üzerinde `macosx_11_0_arm64` veya 64-bit Windows üzerinde `win_amd64`.

## Add the Package to `requirements.txt`

Tekrarlanabilir ortamlar için, paket sürümünü `requirements.txt` dosyanıza sabitleyin:

```txt
groupdocs-redaction-net==26.6.0
```

Ardından tüm bağımlılıkları tek adımda kurun:

```bash
pip install -r requirements.txt
```

## Install from a Pre-Downloaded Wheel

Derleme ortamınız PyPI'ye erişemiyorsa, uygun tekerleği [GroupDocs Releases website](https://releases.groupdocs.com/redaction/python-net/) adresinden indirin ve yerel olarak kurun. Tekerlekler aşağıdaki dört platform için yayınlanmıştır:

- **Windows 64-bit**: file name ends with `win_amd64.whl`
- **Linux x64 (glibc)**: file name ends with `manylinux1_x86_64.whl`
- **macOS Intel**: file name ends with `macosx_10_14_x86_64.whl`
- **macOS Apple Silicon**: file name ends with `macosx_11_0_arm64.whl`

İndirilen tekerleği proje klasörünüze koyun, ardından kurun:

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

Beklenen çıktı:

```bash
Processing ./groupdocs_redaction_net-26.6.0-py3-none-*.whl
Installing collected packages: groupdocs-redaction-net
Successfully installed groupdocs-redaction-net-26.6.0
```

## Platform Prerequisites

Windows'ta ekstra bir adım gerekmez. Linux ve macOS'ta, render motorunun bağımlı olduğu yerel kütüphaneleri kurun:

```bash
apt install libgdiplus libfontconfig1 libicu-dev ttf-mscorefonts-installer
```

```bash
brew install mono-libgdiplus
```

26.6.0 sürümünde, **rasterization to PDF and image-area redaction run only on Windows** — Linux/macOS'ta `System.PlatformNotSupportedException` hatası verir ve yukarıdaki yerel paketler bu kısıtlamayı kaldırmaz. Metin, meta veri, açıklama ve sayfa redaksiyonu ve özgün formatta kaydetme her platformda çalışır. Tam özellik‑destek matrisı için [System Requirements]() sayfasına bakın.

## Verify the Installation

Paketin doğru şekilde içe aktarıldığını doğrulayın ve kurulu sürümü kontrol edin:

```bash
python -c "import groupdocs.redaction; print('GroupDocs.Redaction is ready')"
```

`pip show groupdocs-redaction-net` komutuyla kurulu paketi listeleyerek sürüm ve konumunu doğrulayabilirsiniz.

## Next Steps

- Follow the [Hello, World!]() guide to run your first redaction.
- Read the [Features Overview]() to see everything you can redact.
- Clone the [examples repository](https://github.com/groupdocs-redaction/GroupDocs.Redaction-for-Python-via-.NET) and read [How to Run Examples]() to try every documented scenario locally.
