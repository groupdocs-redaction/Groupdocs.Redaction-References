---
title: "Gunakan kebijakan redaksi"
linkTitle: "Use redaction policies"
second_title: "Referensi API GroupDocs.Redaction untuk Python via .NET"
description: "Pelajari cara menanganinya. Jika Anda memiliki kebijakan penghapusan data sensitif perusahaan berupa daftar aturan redaksi, Anda tidak perlu menyebutkannya dalam kode Anda. Anda dapat menentukan dokumen XML dengan daftar redaksi yang telah dikonfigurasi sebelumnya."
type: docs
url: /id/python-net/guides/use-redaction-policies/
is_root: false
weight: 110
---


Jika Anda memiliki kebijakan penghapusan data sensitif perusahaan berupa daftar aturan redaksi, Anda tidak perlu menyebutkannya dalam kode Anda. Anda dapat menentukan dokumen XML dengan daftar redaksi yang telah dikonfigurasi sebelumnya.

Berikut adalah contoh file XML kebijakan redaksi (pemetaan properti kode jelas):

**RedactionPolicy.xml**

```xml
<?xml version="1.0" encoding="utf-8"?>  
<redactionPolicy xmlns="http://www.groupdocs.com/redaction">  
  <regexRedaction regularExpression="(dolor)" actionType="ReplaceString" replacement="foobar" />  
  <exactPhraseRedaction searchPhrase="dolor" caseSensitive="true" actionType="DrawBox" color="Red" />   
  
  <eraseMetadataRedaction filter="All" />  
  <metadataSearchRedaction filter="Title, Author" replacement="foobar" valueExpression="(metasearch)" keyExpression="" />  
  
  <annotationRedaction regularExpression="(anno1)" replacement="foobar" />  
  <deleteAnnotationRedaction regularExpression="(anno2)" />  
  
  <imageAreaRedaction pointX="15" pointY="17" width="200" height="10" color="#AA50FC"  />  
  <imageAreaRedaction pointX="110" pointY="120" width="60" height="20" color="Magenta"  />  
</redactionPolicy> 
```
Anda dapat menggunakan metode RedactionPolicy.save() untuk membuat dokumen XML dengan struktur ini, mengonfigurasi redaksi pada waktu berjalan.

Contoh berikut menunjukkan cara menyimpan sebuah [RedactionPolicy](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction/redactionpolicy/) ke file XML.
 

```python
from groupdocs.redaction import RedactionPolicy
from groupdocs.redaction.redactions import (
    ExactPhraseRedaction,
    ReplacementOptions,
    RegexRedaction,
    DeleteAnnotationRedaction,
    EraseMetadataRedaction,
    MetadataFilters,
)
from groupdocs.pydrawing import Color

def create_redaction_policy():
    # Tentukan warna redaksi
    color = Color.from_argb(255, 220, 20, 60)

    # Konfigurasikan redaksi
    redactions = [
        ExactPhraseRedaction("Redaction", ReplacementOptions("[Product]")),
        RegexRedaction("\\d{2}\\s*\\d{2}[^\\d]*\\d{6}", ReplacementOptions(color)),
        DeleteAnnotationRedaction(),
        EraseMetadataRedaction(MetadataFilters.ALL),
    ]

    # Buat kebijakan
    policy = RedactionPolicy(redactions)

    # Simpan kebijakan redaksi ke file XML
    policy.save("./sample_policy.xml")
    print("Redactions policy saved to ./sample_policy.xml")

if __name__ == "__main__":
    create_redaction_policy()
```

  
```text
<?xml version="1.0"?>
<redactionPolicy>
  <exactPhraseRedaction actionType="ReplaceString" replacement="[Product]" searchPhrase="Redaction" />
  <regexRedaction actionType="DrawBox" color="#DC143C" regularExpression="\d{2}\s*\d{2}[^\d]*\d{6}" />
  <deleteAnnotationRedaction regularExpression="[.]*" />
  <eraseMetadataRedaction filter="All" />
</redactionPolicy>
```
[Download full output](https://docs.groupdocs.com/redaction/python-net/_output_files/developer-guide/advanced-usage/use-redaction-policies/create_redaction_policy/sample_policy.xml)

Anda dapat memiliki sebanyak mungkin kebijakan yang Anda perlukan, memuatnya untuk meredaksi dokumen Anda.

Contoh di bawah ini memuat kebijakan redaksi dari file XML dan menerapkan setiap aturan yang terkandung di dalamnya ke sebuah dokumen dalam satu panggilan `apply`:

```python
from groupdocs.redaction import Redactor, RedactionPolicy
from groupdocs.redaction.options import SaveOptions

def use_redaction_policy():
    # Muat kebijakan redaksi dari file XML
    policy = RedactionPolicy.load("./redaction_policy.xml")

    # Muat dokumen dan terapkan seluruh kebijakan dalam satu panggilan
    with Redactor("./sample.docx") as redactor:
        redactor.apply(policy)

        # Pertahankan format asli dan tambahkan akhiran pada nama output
        save_options = SaveOptions()
        save_options.add_suffix = True
        save_options.rasterize_to_pdf = False
        save_options.redacted_file_suffix = "redacted"
        result_path = redactor.save(save_options)

    print(f"Redaction policy applied. Output saved to {result_path}.")

if __name__ == "__main__":
    use_redaction_policy()
```

`redaction_policy.xml` adalah file kebijakan yang digunakan dalam contoh ini. Klik [di sini](https://docs.groupdocs.com/redaction/python-net/_sample_files/developer-guide/advanced-usage/use-redaction-policies/redaction_policy.xml) untuk mengunduhnya.

`sample.docx` adalah dokumen yang direduksi dalam contoh ini. Klik [di sini](https://docs.groupdocs.com/redaction/python-net/_sample_files/developer-guide/advanced-usage/use-redaction-policies/sample.docx) untuk mengunduhnya.

  
```text
Binary file (DOCX, 16 KB)
```
[Download full output](https://docs.groupdocs.com/redaction/python-net/_output_files/developer-guide/advanced-usage/use-redaction-policies/use_redaction_policy/sample_redacted.docx)
