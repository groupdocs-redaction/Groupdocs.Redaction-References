---
title: "Görüntü redaksiyonları"
linkTitle: "Image redactions"
second_title: "GroupDocs.Redaction for Python via .NET API Referansları"
description: "Bu makale, JPG, PNG, TIFF ve diğer çeşitli formatlardaki görüntülerden hassas nitelikteki verileri nasıl redakte edeceğinizi gösterir."
type: docs
url: /tr/python-net/guides/image-redactions/
is_root: false
weight: 60
---


GroupDocs.Redactions, JPG, PNG, TIFF ve diğer çeşitli formatlardaki görüntülerden hassas nitelikteki verileri redakte etmek için bir dizi özellik sunar. Tam listeyi [supported document formats]() makalesinde görebilirsiniz.

GroupDocs.Redaction, görüntüleri redakte etmenin iki yolunu destekler; ayrı görüntü dosyalarında ve gömülü görüntülerde:
*   You can put a colored box over a given area, such as header, footer, or an area, where customer's data are expected to appear.
*   You can use any 3-rd party OCR engine to process the image, search it for text and redact sensitive data within the image.   

GroupDocs.Redaction for Python via .NET ayrıca görüntü meta verilerini değiştirmenize (ör. bir görüntünün EXIF verilerini düzenleme veya "EXIF silici" olarak hareket etme) olanak tanır.

## Redact image area

Görüntü alanını redakte etmek için [ImageAreaRedaction](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction.redactions/imagearearedaction/) sınıfını kullanmanız gerekir:

```python
from groupdocs.redaction import Redactor, RedactionStatus
from groupdocs.redaction.options import SaveOptions
from groupdocs.redaction.redactions import ImageAreaRedaction, RegionReplacementOptions
from groupdocs.pydrawing import Color, Point, Size

def redact_image_area():
    # Redakte edilecek alanın sol üst konumunu tanımlayın
    sample_point = Point(385, 485)
    # Redakte edilmesi gereken alanın boyutunu tanımlayın
    sample_size = Size(1793, 2069)
    # Redaksiyon kutusunun rengini tanımlayın
    color = Color.from_argb(255, 220, 20, 60)

    # Redaksiyon seçeneklerini belirtin
    repl_opt = RegionReplacementOptions(color, sample_size)
    img_red = ImageAreaRedaction(sample_point, repl_opt)

    # Redakte edilecek belgeyi yükleyin
    with Redactor("./sample.jpg") as redactor:
        # Kırpma işlemini uygula
        result = redactor.apply(img_red)

        if result.status != RedactionStatus.FAILED:
            # Varsayılan olarak, redakte edilen belge PDF formatında kaydedilir
            save_options = SaveOptions()
            save_options.add_suffix = True
            save_options.rasterize_to_pdf = True
            save_options.redacted_file_suffix = "redacted"
            redactor.save(save_options)

if __name__ == "__main__":
    redact_image_area()
```

`sample.jpg` bu örnekte kullanılan örnek dosyadır. İndirmek için [buraya](https://docs.groupdocs.com/redaction/python-net/_sample_files/developer-guide/basic-usage/image-redactions/sample.jpg) tıklayın.

  
```text
Binary file (PDF, 2.7 MB)
```
[Download full output](https://docs.groupdocs.com/redaction/python-net/_output_files/developer-guide/basic-usage/image-redactions/redact_image_area/sample_redacted.pdf)

Redaksiyon bu dosya türüne uygulanamıyorsa, örneğin gömülü görüntüsü olmayan MS Word belgesi, [RedactorChangeLog.Status](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction/redactorchangelog/status/) [RedactionStatus.Skipped](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction/redactionstatus/) olacaktır.

## Clean image metadata

Aşağıdaki örnek, bir fotoğraftan veya başka bir görüntüden exif verilerini (silerek) nasıl düzenleyeceğinizi gösterir:

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.options import SaveOptions
from groupdocs.redaction.redactions import EraseMetadataRedaction, MetadataFilters

def clean_image_metadata():
    # Tüm görüntü meta verilerini (ör. EXIF) kaldırmak için redaksiyon seçeneklerini belirtin
    er_opt = EraseMetadataRedaction(MetadataFilters.ALL)

    # Redakte edilecek görüntüyü yükleyin
    with Redactor("./sample.jpg") as redactor:
        # Kırpma işlemini uygula
        result = redactor.apply(er_opt)

        # Redakte edilmiş görüntüyü kaynak dosyanın yanına kaydet
        so = SaveOptions()
        so.add_suffix = True
        so.rasterize_to_pdf = False
        so.redacted_file_suffix = "redacted"
        redactor.save(so)

if __name__ == "__main__":
    clean_image_metadata()
```

`sample.jpg` bu örnekte kullanılan örnek dosyadır. İndirmek için [buraya](https://docs.groupdocs.com/redaction/python-net/_sample_files/developer-guide/basic-usage/image-redactions/sample.jpg) tıklayın.

  
```text
Binary file (JPG, 3.1 MB)
```
[Download full output](https://docs.groupdocs.com/redaction/python-net/_output_files/developer-guide/basic-usage/image-redactions/clean_image_metadata/sample_redacted.jpg)

Redaksiyon bu dosya türüne uygulanamıyorsa, örneğin BMP görüntüsü, [RedactorChangeLog.Status](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction/redactorchangelog/status/) [RedactionStatus.Skipped](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction/redactionstatus/) olacaktır.

## Redact embedded images

Bir belgedeki tüm gömülü görüntüler içinde görüntü alanını redakte edebilirsiniz.

Aşağıdaki örnek, bir Microsoft Word belgesi içindeki tüm gömülü görüntüleri nasıl redakte edeceğinizi gösterir:

```python
from groupdocs.redaction import Redactor, RedactionStatus
from groupdocs.redaction.options import SaveOptions
from groupdocs.redaction.redactions import ImageAreaRedaction, RegionReplacementOptions
from groupdocs.pydrawing import Color, Point, Size

def redact_embedded_images():
    # Redakte edilecek alanın sol üst konumunu tanımlayın
    sample_point = Point(516, 311)
    # Redakte edilmesi gereken alanın boyutunu tanımlayın
    sample_size = Size(170, 35)
    # Redaksiyon kutusunun rengini tanımlayın
    color = Color.from_argb(255, 220, 20, 60)

    # Redaksiyon seçeneklerini belirtin
    repl_opt = RegionReplacementOptions(color, sample_size)
    img_red = ImageAreaRedaction(sample_point, repl_opt)

    # Redakte edilecek belgeyi yükleyin
    with Redactor("./sample.docx") as redactor:
        # Redaksiyonu tüm gömülü görüntülere uygulayın
        result = redactor.apply(img_red)

        if result.status != RedactionStatus.FAILED:
            # Varsayılan olarak, redakte edilen belge PDF formatında kaydedilir
            save_options = SaveOptions()
            save_options.add_suffix = True
            save_options.rasterize_to_pdf = True
            save_options.redacted_file_suffix = "redacted"
            redactor.save(save_options)

if __name__ == "__main__":
    redact_embedded_images()
```

`sample.docx` bu örnekte kullanılan örnek dosyadır. İndirmek için [buraya](https://docs.groupdocs.com/redaction/python-net/_sample_files/developer-guide/basic-usage/image-redactions/sample.docx) tıklayın.

  
```text
Binary file (PDF, 1022 KB)
```
[Download full output](https://docs.groupdocs.com/redaction/python-net/_output_files/developer-guide/basic-usage/image-redactions/redact_embedded_images/sample_redacted.pdf)

Redaksiyon bu dosya türüne uygulanamıyorsa, örneğin bir elektronik tablo belgesi, [RedactorChangeLog.Status](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction/redactorchangelog/status/) [RedactionStatus.Skipped](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction/redactionstatus/) olacaktır.

## Multi-frame images

Belirli bir başlangıç ve çerçeve sayısı ile çok çerçeveli bir görüntüden çerçeveleri kaldırabilirsiniz. Daha fazla bilgi için [sayfa redaksiyonlarını kaldırma]() makalesine bakın.

DjVu belgeleri gibi bazı görüntü formatları, [pre-rasterization]() ve ardından PDF formatında kaydetme gerektirir.
