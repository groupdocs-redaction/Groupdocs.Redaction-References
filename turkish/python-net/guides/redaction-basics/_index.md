---
title: "Bu makale, Python geliştiricilerinin belgelerinde meta veri, görüntü, açıklama ve metin redaksiyonu nasıl uygulayabileceklerini gösterir. PDF, DOC, DOCX, PPT, PPTX, XLS, XLSX ve diğerleri gibi geniş bir belge formatı yelpazesi desteklenir."
linkTitle: "Redaction basics"
second_title: "GroupDocs.Redaction for Python via .NET API Referansları"
description: "GroupDocs.Redaction, etkili bir belge redaksiyon özellikleri setini destekler. [metin](), [meta veri](), [açıklamalar](), [görüntüler]() için redaksiyon uygulamanıza olanak tanır."
type: docs
url: /tr/python-net/guides/redaction-basics/
is_root: false
weight: 40
---


PDF, DOC, DOCX, PPT, PPTX, XLS, XLSX ve diğerleri gibi geniş bir belge formatı yelpazesi desteklenir. Tam desteklenen formatlar listesini [desteklenen belge formatları]() makalesinde görebilirsiniz.

GroupDocs.Redaction aşağıdaki redaksiyon türleriyle birlikte gelir:

## Redaction types

Tür

| [ExactPhraseRedaction](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction.redactions/exactphraseredaction/), [RegexRedaction](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction.redactions/regexredaction/) | Açıklama | Sınıflar |
| --- | --- | --- |
| [Text]() | Replaces or hides with color block a portion of text within document body | [EraseMetadataRedaction](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction.redactions/erasemetadataredaction/), [MetadataSearchRedaction](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction.redactions/metadatasearchredaction/) |
| [Metadata]() | Replace metadata values with empty ones or redacts metadata texts | [EraseMetadataRedaction](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction.redactions/erasemetadataredaction/), [MetadataSearchRedaction](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction.redactions/metadatasearchredaction/) |
| [Annotations]() | Deletes annotations from document or redacts its texts | [DeleteAnnotationRedaction](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction.redactions/deleteannotationredaction/), [AnnotationRedaction](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction.redactions/annotationredaction/) |
| [Images]() | Replaces specific area of an image with a colored box | [ImageAreaRedaction](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction.redactions/imagearearedaction/) |
| [Pages]() | Removes specific range of pages (slides, worksheets, etc.) | [RemovePageRedaction](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction.redactions/removepageredaction/) |

## Apply redaction

Bir belgeye redaksiyon uygulamak, [Redactor.Apply](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction/redactor/apply/) yöntemiyle yapılır. Sonuç olarak, uygulanan her redaksiyon için bir günlük girdisi içeren bir [RedactorChangeLog](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction/redactorchangelog/) örneği alırsınız. Girdi, seçenekleri, işlemin durumu (aşağıya bakın) ve gerektiğinde metinsel açıklamaları içeren bir [Redacton](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction/redaction/) örneğine referans içerir. En az bir redaksiyon başarısız olursa, [Status == RedactionStatus.Failed](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction/redactionstatus/) göreceksiniz:

```python
from groupdocs.redaction import Redactor, RedactionStatus
from groupdocs.redaction.options import SaveOptions
from groupdocs.redaction.redactions import ExactPhraseRedaction, ReplacementOptions

def apply_redaction():
    # Redaksiyon seçeneklerini belirtin
    repl_opt = ReplacementOptions("[personal]")
    ex_red = ExactPhraseRedaction("John Doe", repl_opt)

    # Redakte edilecek belgeyi yükleyin
    with Redactor("./sample.docx") as redactor:
        # Kırpma işlemini uygula
        result = redactor.apply(ex_red)

        if result.status != RedactionStatus.FAILED:
            # Redakte edilmiş belgeyi kaynak dosyanın yanına kaydedin
            so = SaveOptions()
            so.add_suffix = True
            so.rasterize_to_pdf = False
            so.redacted_file_suffix = "redacted"
            redactor.save(so)

if __name__ == "__main__":
    apply_redaction()
```

`sample.docx` bu örnekte kullanılan örnek dosyadır. İndirmek için [here](https://docs.groupdocs.com/redaction/python-net/_sample_files/developer-guide/basic-usage/redaction-basics/sample.docx) tıklayın.

  
```text
Binary file (DOCX, 16 KB)
```
[Download full output](https://docs.groupdocs.com/redaction/python-net/_output_files/developer-guide/basic-usage/redaction-basics/apply_redaction/sample_redacted.docx)

Tüm olası durumlar [RedactionStatus](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction/redactionstatus/) sayımında bu tabloda listelenmiştir:

| Durum | Açıklama | Olası nedenler |
| --- | --- | --- |
| *Applied* | Redaksiyon tamamen ve başarılı bir şekilde uygulandı | Redaksiyon sürecindeki tüm işlemler başarılı bir şekilde uygulandı |
| *PartiallyApplied* | Redaksiyon yalnızca eşleşmelerinin bir kısmına uygulandı | 1) Değiştirmeler için deneme sınırlamaları aşıldı2) En az bir değişiklik kullanıcı tarafından reddedildi |
| *Skipped* | Redaksiyon atlandı (uygulanmadı) | 1) Redaksiyonlar için deneme sınırlamaları aşıldı2) Redaksiyon bu belge türüne uygulanamaz3) Tüm değiştirmeler kullanıcı tarafından reddedildi ve hiçbir değişiklik yapılmadı |
| *Failed* | Redaksiyon bir istisna ile başarısız oldu | Redaksiyon sürecinde bir istisna oluştu |

Ayrıntılı bilgi için [RedactorChangeLog.RedactionLog](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction/redactorchangelog/redaction_log/) içindeki redaksiyon günlük girdileri arasında döngü yapmalı ve *Applied* olmayan durumdaki öğelerin [ErrorMessage](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction/redactionresult/error_message/) özelliğini kontrol etmelisiniz:

```python
result = redactor.apply(redaction)
if result.status != RedactionStatus.FAILED:
    # Varsayılan olarak, redakte edilen belge PDF formatında kaydedilir
    save_options = SaveOptions()
    save_options.add_suffix = True
    save_options.rasterize_to_pdf = True
    save_options.redacted_file_suffix = "redacted"
    result_path = redactor.save(save_options)
    print(f"Document redacted successfully.\nCheck output in {result_path}")
else:
    # Tüm başarısız veya atlanan redaksiyonları dökümle
    print("Redaction failed!")
    for log_entry in result.redaction_log:
        if log_entry.result.status != RedactionStatus.APPLIED:
            print(f"Status is {log_entry.result.status}, details: {log_entry.result.error_message}")
```

## Apply multiple redactions

İhtiyacınız kadar redaksiyonu tek bir [Redactor.Apply](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction/redactor/apply/) yöntemi çağrısında uygulayabilirsiniz, çünkü aşırı yüklemesi bir redaksiyon dizisi ve redaksiyon politikası kabul eder. Bu durumda, redaksiyonlar dizide göründükleri sırayla uygulanır. Kodunuzda redaksiyon setlerini belirtmeye alternatif olarak, [here]() adresinde açıklandığı gibi redaksiyon politikası içeren bir XML dosyası oluşturabilirsiniz.

```python
from groupdocs.redaction import Redactor, RedactionStatus
from groupdocs.redaction.options import SaveOptions
from groupdocs.redaction.redactions import (
    ExactPhraseRedaction,
    RegexRedaction,
    ReplacementOptions,
    DeleteAnnotationRedaction,
    EraseMetadataRedaction,
    MetadataFilters,
)
from groupdocs.pydrawing import Color

def apply_multiple_redactions():
    # Redaksiyon kutusunun rengini tanımlayın
    color = Color.from_argb(255, 220, 20, 60)

    # Uygulanacak redaksiyonların sıralı bir listesini sağlayın
    redaction_list = [
        ExactPhraseRedaction("John Doe", ReplacementOptions("[Client]")),
        RegexRedaction("Redaction", ReplacementOptions("[Product]")),
        RegexRedaction("\\d{2}\\s*\\d{2}[^\\d]*\\d{6}", ReplacementOptions(color)),
        DeleteAnnotationRedaction(),
        EraseMetadataRedaction(MetadataFilters.ALL),
    ]

    # Redakte edilecek belgeyi yükleyin
    with Redactor("./sample.docx") as redactor:
        # Kırpma listesini uygula
        result = redactor.apply(redaction_list)

        if result.status != RedactionStatus.FAILED:
            # Varsayılan olarak, redakte edilen belge PDF formatında kaydedilir
            save_options = SaveOptions()
            save_options.add_suffix = True
            save_options.rasterize_to_pdf = True
            save_options.redacted_file_suffix = "redacted"
            redactor.save(save_options)
        else:
            # Tüm başarısız veya atlanan redaksiyonları dökümle
            print("Redaction failed!")
            for log_entry in result.redaction_log:
                if log_entry.result.status != RedactionStatus.APPLIED:
                    print(f"Status is {log_entry.result.status}, details: {log_entry.result.error_message}")

if __name__ == "__main__":
    apply_multiple_redactions()
```

`sample.docx` bu örnekte kullanılan örnek dosyadır. İndirmek için [here](https://docs.groupdocs.com/redaction/python-net/_sample_files/developer-guide/basic-usage/redaction-basics/sample.docx) tıklayın.

  
```text
Binary file (PDF, 1.2 MB)
```
[Download full output](https://docs.groupdocs.com/redaction/python-net/_output_files/developer-guide/basic-usage/redaction-basics/apply_multiple_redactions/sample_redacted.pdf)
