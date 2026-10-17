---
title: "Meta veri redaksiyonları"
linkTitle: "Metadata redactions"
second_title: "GroupDocs.Redaction for Python via .NET API Referansları"
description: "Bu makale, Python redaksiyon API'sinin filtreler veya düzenli ifade araması kullanarak meta verileri değiştirme veya kaldırma imkanı sağladığını gösterir."
type: docs
url: /tr/python-net/guides/metadata-redactions/
is_root: false
weight: 70
---


GroupDocs.Redaction API ile PDF, DOC, DOCX, PPT, PPTX, XLS, XLSX ve diğer farklı formatlardaki belgeler için meta veri redaksiyonları uygulayabilirsiniz. Tam listeyi [supported document formats]() makalesinde görebilirsiniz.

GroupDocs.Redactions, filtreler veya düzenli ifade araması kullanarak meta verileri değiştirme veya kaldırma imkanı sunan esnek bir API sağlar.

## Filter metadata

Tüm redaksiyonların temel işlevselliği, [MetadataRedaction](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction.redactions/metadataredaction/) temel sınıfından türetilmiştir ve *metadata filtering* olarak adlandırılır; meta veri redaksiyonları için zorunludur. En sık kullanılan meta veri girişlerini içeren işaretli enum [MetadataFilters](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction.redactions/metadatafilters/) kullanır. Filtreyi *All* ya da meta verilerin herhangi bir kombinasyonuna ayarlayabilirsiniz. Örneğin, aşağıdaki örnek filtreyi *Author*, *Manager* ve *NameOfApplication* olarak ayarlar - metin redaksiyonu için ya da bunları temizlemek amacıyla:

```python
# MetadataRedaction'dan türetilen redaksiyon
redaction.filter = MetadataFilters.AUTHOR | MetadataFilters.MANAGER | MetadataFilters.NAME_OF_APPLICATION
```

Aşağıda, [MetadataFilters](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction.redactions/metadatafilters/) öğelerinin tam listesi bulunan tablo yer almaktadır:

| Filtre | Sayısal değer | Açıklama |
| --- | --- | --- |
| *None* | 0 | Boş filtre ayarı, hiçbir meta veri öğesiyle eşleşmez |
| *Author* | 1 | Belgenin yazarı |
| *Kategori* | 2 | Belgenin kategorisi |
| *Yorumlar* | 4 | Belge yorumu |
| *Şirket* | 8 | Yazarın şirketi |
| *ContentStatus* | 16 | İçerik durumu |
| *CreatedTime* | 32 | Oluşturma zamanı |
| *HyperlinkBase* | 64 | Köprü temeli |
| *LastPrinted* | 128 | Son yazdırma tarih ve saati |
| *LastSavedBy* | 256 | Kullanıcı tarafından son kaydedildi |
| *LastSavedTime* | 1024 | Son kaydedilen tarih ve saat |
| *NameOfApplication* | 2048 | Belgenin oluşturulduğu uygulamanın adı |
| *Manager* | 4096 | Yazarın yöneticisinin adı |
| *RevisionNumber* | 8192 | Revizyon numarası |
| *Subject* | 16384 | Belgenin konusu |
| *Template* | 32768 | Belge şablonu adı |
| *Title* | 65536 | Belge başlığı |
| *TotalEditingTime* | 131072 | Toplam düzenleme süresi |
| *Sürüm* | 262144 | Belgenin sürümü |
| *Açıklama* | 524288 | Belgenin açıklaması |
| *Anahtar Kelimeler* | 1048576 | Belgenin anahtar kelimeleri |
| *ContentType* | 2097152 | İçerik türü |
| *Tümü* | 2147483647 | Meta veri öğelerinin tüm türleri |

## Clean metadata

Belgedeki tüm veya belirli meta verileri boş (boş veya minimal) değerlerle değiştirmek için [EraseMetadataRedaction](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction.redactions/erasemetadataredaction/) sınıfını kullanabilirsiniz. Aşağıdaki örnek, belgenin tüm özelliklerini boşaltır:

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.options import SaveOptions
from groupdocs.redaction.redactions import EraseMetadataRedaction, MetadataFilters

def clean_all_metadata():
    # Tüm meta verileri silmek için redaksiyon seçeneklerini belirtin
    met_red = EraseMetadataRedaction(MetadataFilters.ALL)

    # Redakte edilecek belgeyi yükleyin
    with Redactor("./sample.docx") as redactor:
        # Kırpma işlemini uygula
        result = redactor.apply(met_red)

        # Redakte edilmiş belgeyi kaynak dosyanın yanına kaydedin
        so = SaveOptions()
        so.add_suffix = True
        so.rasterize_to_pdf = False
        so.redacted_file_suffix = "redacted"
        redactor.save(so)

if __name__ == "__main__":
    clean_all_metadata()
```

`sample.docx` bu örnekte kullanılan örnek dosyadır. İndirmek için [buraya](https://docs.groupdocs.com/redaction/python-net/_sample_files/developer-guide/basic-usage/metadata-redactions/sample.docx) tıklayın.

  
```text
Binary file (DOCX, 16 KB)
```
[Download full output](https://docs.groupdocs.com/redaction/python-net/_output_files/developer-guide/basic-usage/metadata-redactions/clean_all_metadata/sample_redacted.docx)

Verilen belgede tüm meta verileri boşaltmak için [MetadataFilter.All](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction.redactions/metadatafilters/) belirtebilir veya varsayılan yapıcıyı kullanabilirsiniz, Custom - tüm özel meta veri girişlerini temizlemek için.

## Redact metadata

[MetadataSearchRedaction](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction.redactions/metadatasearchredaction/) sınıfını, belge meta verilerindeki hassas verileri düzenli ifadeler kullanarak kaldırmak için kullanabilirsiniz. Örneğin, "Company Ltd." ifadesinin tüm geçişlerini kaldırabiliriz:

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.options import SaveOptions
from groupdocs.redaction.redactions import MetadataSearchRedaction

def redact_metadata():
    # Redaksiyon seçeneklerini belirtin: arama deseni ve değiştirme dizesi
    met_red = MetadataSearchRedaction("Company Ltd.", "--company--")

    # Redakte edilecek belgeyi yükleyin
    with Redactor("./sample.docx") as redactor:
        # Kırpma işlemini uygula
        result = redactor.apply(met_red)

        # Redakte edilmiş belgeyi kaynak dosyanın yanına kaydedin
        so = SaveOptions()
        so.add_suffix = True
        so.rasterize_to_pdf = False
        so.redacted_file_suffix = "redacted"
        redactor.save(so)

if __name__ == "__main__":
    redact_metadata()
```

`sample.docx` bu örnekte kullanılan örnek dosyadır. İndirmek için [buraya](https://docs.groupdocs.com/redaction/python-net/_sample_files/developer-guide/basic-usage/metadata-redactions/sample.docx) tıklayın.

  
```text
Binary file (DOCX, 16 KB)
```
[Download full output](https://docs.groupdocs.com/redaction/python-net/_output_files/developer-guide/basic-usage/metadata-redactions/redact_metadata/sample_redacted.docx)

İlk argüman düzenli ifadedir, ikincisi bir değiştirme dizesidir. Filtre ayarlayarak redaksiyon kapsamını belirleyebilirsiniz, örneğin [MetadataFilter.Company](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction.redactions/metadatafilters/). - Bu, "Company" özelliği dışındaki tüm meta veri öğelerinde düzenli ifade eşleşmelerini bırakır:

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.options import SaveOptions
from groupdocs.redaction.redactions import MetadataSearchRedaction, MetadataFilters

def redact_metadata_with_filter():
    # Redaksiyon seçeneklerini belirtin: arama deseni ve değiştirme dizesi
    met_red = MetadataSearchRedaction("Company Ltd.", "--company--")

    # Redaksiyon kapsamını yalnızca Company meta veri öğesiyle sınırlayın
    met_red.filter = MetadataFilters.COMPANY

    # Redakte edilecek belgeyi yükleyin
    with Redactor("./sample.docx") as redactor:
        # Kırpma işlemini uygula
        result = redactor.apply(met_red)

        # Redakte edilmiş belgeyi kaynak dosyanın yanına kaydedin
        so = SaveOptions()
        so.add_suffix = True
        so.rasterize_to_pdf = False
        so.redacted_file_suffix = "redacted"
        redactor.save(so)

if __name__ == "__main__":
    redact_metadata_with_filter()
```

`sample.docx` bu örnekte kullanılan örnek dosyadır. İndirmek için [buraya](https://docs.groupdocs.com/redaction/python-net/_sample_files/developer-guide/basic-usage/metadata-redactions/sample.docx) tıklayın.

  
```text
Binary file (DOCX, 16 KB)
```
[Download full output](https://docs.groupdocs.com/redaction/python-net/_output_files/developer-guide/basic-usage/metadata-redactions/redact_metadata_with_filter/sample_redacted.docx)

## Metadata redaction status

Tüm meta veri redaksiyonları her meta veri öğesine ayrı ayrı uygulanır ve bir meta veri öğesi redaksiyonu başarısız olsa bile diğer meta veri öğeleri güncellenir. Başarısız, atlanan (reddedilen) meta veri öğelerinin ve bunun nedenlerinin listesini [ErrorMessage](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction/redactionresult/error_message/) özelliğinde, [RedactorLogEntry.Result](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction/redactorlogentry/result/) içinde bulabilirsiniz.
