---
title: "Redaksi teks"
linkTitle: "Text redaction"
second_title: "Referensi API GroupDocs.Redaction untuk Python via .NET"
description: "Artikel ini menjelaskan bagaimana API redaksi Python memungkinkan Anda dengan mudah meredaksi data yang bersifat sensitif atau pribadi dari dokumen Anda. Anda dapat menerapkan redaksi teks menggunakan frasa tepat atau ekspresi reguler untuk dokumen dengan berbagai format seperti PDF, DOC, DOCX, PPT, PPTX, XLS, XLSX, dan lainnya."
type: docs
url: /id/python-net/guides/text-redactions/
is_root: false
weight: 50
---


GroupDocs.Redaction memungkinkan dengan mudah meredaksi data yang bersifat sensitif atau pribadi dari dokumen Anda. Kasus redaksi yang paling populer adalah menghapus teks dari sebuah dokumen.

Dengan API GroupDocs.Redaction Anda dapat menerapkan redaksi teks menggunakan frasa tepat atau [ekspresi reguler](https://docs.microsoft.com/en-us/dotnet/standard/base-types/regular-expressions) untuk dokumen dengan berbagai format seperti PDF, DOC, DOCX, PPT, PPTX, XLS, XLSX, dan lainnya. Lihat daftar lengkap pada artikel [format dokumen yang didukung]().

## Use exact phrase redaction

Pada contoh di bawah, kami menerapkan redaksi teks, mengganti frasa tepat pribadi "John Doe" dengan "\[personal\]" (atau kode pengecualian apa pun):

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.options import SaveOptions
from groupdocs.redaction.redactions import ExactPhraseRedaction, ReplacementOptions

def redact_exact_phrase():
    # Tentukan opsi redaksi
    repl_opt = ReplacementOptions("[personal]")
    ex_red = ExactPhraseRedaction("John Doe", repl_opt)

    # Muat dokumen yang akan direduksi
    with Redactor("./sample.docx") as redactor:
        # Terapkan penyensoran
        result = redactor.apply(ex_red)

        # Simpan dokumen yang telah diredaksi di samping file sumber
        so = SaveOptions()
        so.add_suffix = True
        so.rasterize_to_pdf = False
        so.redacted_file_suffix = "redacted"
        redactor.save(so)

if __name__ == "__main__":
    redact_exact_phrase()
```

`sample.docx` adalah file contoh yang digunakan dalam contoh ini. Klik [di sini](https://docs.groupdocs.com/redaction/python-net/_sample_files/developer-guide/basic-usage/text-redactions/sample.docx) untuk mengunduhnya.

  
```text
Binary file (DOCX, 16 KB)
```
[Download full output](https://docs.groupdocs.com/redaction/python-net/_output_files/developer-guide/basic-usage/text-redactions/redact_exact_phrase/sample_redacted.docx)

Secara default, pencarian frasa tepat tidak memperhatikan huruf besar/kecil. Untuk redaksi yang sensitif huruf, terdapat parameter konstruktor dan properti publik yang sesuai:

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.options import SaveOptions
from groupdocs.redaction.redactions import ExactPhraseRedaction, ReplacementOptions

def redact_case_sensitive_phrase():
    # Aktifkan pencocokan sensitif huruf
    case_sensitive = True

    # Tentukan opsi redaksi
    repl_opt = ReplacementOptions("[personal]")
    ex_red = ExactPhraseRedaction("John Doe", case_sensitive, repl_opt)

    # Muat dokumen yang akan direduksi
    with Redactor("./sample.docx") as redactor:
        # Terapkan penyensoran
        result = redactor.apply(ex_red)

        # Simpan dokumen yang telah diredaksi di samping file sumber
        so = SaveOptions()
        so.add_suffix = True
        so.rasterize_to_pdf = False
        so.redacted_file_suffix = "redacted"
        redactor.save(so)

if __name__ == "__main__":
    redact_case_sensitive_phrase()
```

`sample.docx` adalah file contoh yang digunakan dalam contoh ini. Klik [di sini](https://docs.groupdocs.com/redaction/python-net/_sample_files/developer-guide/basic-usage/text-redactions/sample.docx) untuk mengunduhnya.

  
```text
Binary file (DOCX, 16 KB)
```
[Download full output](https://docs.groupdocs.com/redaction/python-net/_output_files/developer-guide/basic-usage/text-redactions/redact_case_sensitive_phrase/sample_redacted.docx)

Jika Anda membutuhkan kotak berwarna di atas teks yang disensor, Anda dapat menggunakan warna alih-alih string pengganti. Redaksi akan menghapus teks yang cocok dan menempatkan persegi panjang berwarna yang ditentukan di tempat teks yang disensor:

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.options import SaveOptions
from groupdocs.redaction.redactions import ExactPhraseRedaction, ReplacementOptions
from groupdocs.pydrawing import Color

def redact_with_color_box():
    # Tentukan warna kotak redaksi
    color = Color.from_argb(255, 220, 20, 60)

    # Tentukan opsi redaksi
    repl_opt = ReplacementOptions(color)
    ex_red = ExactPhraseRedaction("John Doe", repl_opt)

    # Muat dokumen yang akan direduksi
    with Redactor("./sample.docx") as redactor:
        # Terapkan penyensoran
        result = redactor.apply(ex_red)

        # Simpan dokumen yang telah diredaksi di samping file sumber
        so = SaveOptions()
        so.add_suffix = True
        so.rasterize_to_pdf = False
        so.redacted_file_suffix = "redacted"
        redactor.save(so)

if __name__ == "__main__":
    redact_with_color_box()
```

`sample.docx` adalah file contoh yang digunakan dalam contoh ini. Klik [di sini](https://docs.groupdocs.com/redaction/python-net/_sample_files/developer-guide/basic-usage/text-redactions/sample.docx) untuk mengunduhnya.

  
```text
Binary file (DOCX, 17 KB)
```
[Download full output](https://docs.groupdocs.com/redaction/python-net/_output_files/developer-guide/basic-usage/text-redactions/redact_with_color_box/sample_redacted.docx)

Anda mungkin perlu menerapkan redaksi pada dokumen dari kanan ke kiri, seperti Arab atau Ibrani. Contoh berikut menunjukkan cara menerapkan ExactPhraseRedaction pada dokumen PDF berbahasa Arab:

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.options import SaveOptions
from groupdocs.redaction.redactions import ExactPhraseRedaction, ReplacementOptions

def redact_right_to_left_text():
    # Tentukan opsi redaksi dengan frasa Arab
    repl_opt = ReplacementOptions("[test]")
    ex_red = ExactPhraseRedaction("انتقد", repl_opt)

    # Muat dokumen yang akan direduksi
    with Redactor("./arabic.pdf") as redactor:
        # Terapkan penyensoran
        result = redactor.apply(ex_red)

        # Simpan dokumen yang telah diredaksi di samping file sumber
        so = SaveOptions()
        so.add_suffix = True
        so.rasterize_to_pdf = False
        so.redacted_file_suffix = "redacted"
        redactor.save(so)

if __name__ == "__main__":
    redact_right_to_left_text()
```

`arabic.pdf` adalah file contoh yang digunakan dalam contoh ini. Klik [di sini](https://docs.groupdocs.com/redaction/python-net/_sample_files/developer-guide/basic-usage/text-redactions/arabic.pdf) untuk mengunduhnya.

  
```text
Binary file (PDF, 23 KB)
```
[Download full output](https://docs.groupdocs.com/redaction/python-net/_output_files/developer-guide/basic-usage/text-redactions/redact_right_to_left_text/arabic_redacted.pdf)

## Use regular expression

Di balik layar, redaksi "frasa tepat" bekerja melalui ekspresi reguler, yang merupakan pendekatan dasar untuk redaksi. Pada contoh di bawah, kami menyensor semua teks yang cocok dengan "2 digit, spasi atau tidak ada, 2 digit, lagi spasi dan 6 digit" dengan kotak berwarna biru:

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.options import SaveOptions
from groupdocs.redaction.redactions import RegexRedaction, ReplacementOptions
from groupdocs.pydrawing import Color

def redact_with_regex():
    # Tentukan warna kotak redaksi
    color = Color.from_argb(255, 220, 20, 60)

    # Tentukan opsi redaksi
    repl_opt = ReplacementOptions(color)
    reg_red = RegexRedaction("\\d{2}\\s*\\d{2}[^\\d]*\\d{6}", repl_opt)

    # Muat dokumen yang akan direduksi
    with Redactor("./sample.docx") as redactor:
        # Terapkan penyensoran
        result = redactor.apply(reg_red)

        # Simpan dokumen yang telah diredaksi di samping file sumber
        so = SaveOptions()
        so.add_suffix = True
        so.rasterize_to_pdf = False
        so.redacted_file_suffix = "redacted"
        redactor.save(so)

if __name__ == "__main__":
    redact_with_regex()
```

`sample.docx` adalah file contoh yang digunakan dalam contoh ini. Klik [di sini](https://docs.groupdocs.com/redaction/python-net/_sample_files/developer-guide/basic-usage/text-redactions/sample.docx) untuk mengunduhnya.

  
```text
Binary file (DOCX, 16 KB)
```
[Download full output](https://docs.groupdocs.com/redaction/python-net/_output_files/developer-guide/basic-usage/text-redactions/redact_with_regex/sample_redacted.docx)

Jika Anda perlu menyensor seluruh paragraf, Anda mungkin juga harus menggunakan RegexRedaction. Contoh berikut menunjukkan cara menyensor seluruh paragraf dalam dokumen PDF:

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.options import SaveOptions
from groupdocs.redaction.redactions import RegexRedaction, ReplacementOptions
from groupdocs.pydrawing import Color

def redact_whole_paragraph():
    # Tentukan warna kotak redaksi
    color = Color.from_argb(255, 220, 20, 60)

    # Tentukan opsi redaksi yang cocok dengan seluruh paragraf
    repl_opt = ReplacementOptions(color)
    reg_red = RegexRedaction("(Lorem(\n|.)+?urna)", repl_opt)

    # Muat dokumen yang akan direduksi
    with Redactor("./sample.pdf") as redactor:
        # Terapkan penyensoran
        result = redactor.apply(reg_red)

        # Simpan dokumen yang telah diredaksi di samping file sumber
        so = SaveOptions()
        so.add_suffix = True
        so.rasterize_to_pdf = False
        so.redacted_file_suffix = "redacted"
        redactor.save(so)

if __name__ == "__main__":
    redact_whole_paragraph()
```

`sample.pdf` adalah file contoh yang digunakan dalam contoh ini. Klik [di sini](https://docs.groupdocs.com/redaction/python-net/_sample_files/developer-guide/basic-usage/text-redactions/sample.pdf) untuk mengunduhnya.

  
```text
Binary file (PDF, 68 KB)
```
[Download full output](https://docs.groupdocs.com/redaction/python-net/_output_files/developer-guide/basic-usage/text-redactions/redact_whole_paragraph/sample_redacted.pdf)
