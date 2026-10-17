---
title: "Sayfa redaksiyonlarını kaldır"
linkTitle: "Remove page redactions"
second_title: "GroupDocs.Redaction for Python via .NET API Referansları"
description: "Bu makale, PDF, sunum ve elektronik tablo belgelerinizdeki hassas verileri içeren sayfaların nasıl kaldırılacağını gösterir."
type: docs
url: /tr/python-net/guides/remove-page-redactions/
is_root: false
weight: 100
---


GroupDocs.Redaction, PDF belgelerinden sayfaları, sunumlardan slaytları ve elektronik tablo belgelerinden çalışma sayfalarını kolayca kaldırmanıza olanak tanır.

GroupDocs.Redaction API'si ile sayfa aralığını göreceli konumu (başlangıç veya son), sıfır tabanlı indeks ve kaldırılacak sayfa sayısı ile belirterek sayfaları kaldırabilirsiniz. Şu anda desteklenen formatlar: PDF, sunumlar (Microsoft PowerPoint, OpenOffice Presentations), kelime işlem belgeleri (Microsoft Word, OpenOffice Texts, Rich Text Files), elektronik tablolar (Microsoft Excel, OpenOffice Spreadsheets, vb.) ve çok çerçeveli görüntüler.

## Remove page range

Aşağıdaki örnekte, belge yeterli sayfaya sahipse 2., 3. ve 4. sayfaları kaldırıyoruz:

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.options import SaveOptions
from groupdocs.redaction.redactions import RemovePageRedaction, PageSeekOrigin

def remove_page_range():
    # Redakte edilecek belgeyi yükleyin
    with Redactor("./multipage_sample.pdf") as redactor:
        # Belge bilgilerini al
        doc_info = redactor.get_document_info()

        # En az 4 sayfa gerektirir
        if doc_info.page_count > 3:
            # 2. sayfadan (sıfır tabanlı indeks 1) başlayarak 3 sayfa kaldır
            rem_opt = RemovePageRedaction(PageSeekOrigin.BEGIN, 1, 3)

            # Kırpma işlemini uygula
            result = redactor.apply(rem_opt)

            # Redakte edilmiş belgeyi kaynak dosyanın yanına kaydedin
            so = SaveOptions()
            so.add_suffix = True
            so.rasterize_to_pdf = False
            so.redacted_file_suffix = "redacted"
            redactor.save(so)

if __name__ == "__main__":
    remove_page_range()
```

`multipage_sample.pdf` bu örnekte kullanılan örnek dosyadır. İndirmek için [buraya](https://docs.groupdocs.com/redaction/python-net/_sample_files/developer-guide/basic-usage/remove-page-redactions/multipage_sample.pdf) tıklayın.

## Remove last page

Bazı durumlarda, sayfa sayısı ne olursa olsun, son sayfayı veya birden fazla sayfayı silmeniz gerekebilir.

Aşağıdaki örnek, bir belgeden son sayfanın nasıl kaldırılacağını gösterir:

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.options import SaveOptions
from groupdocs.redaction.redactions import RemovePageRedaction, PageSeekOrigin

def remove_last_page():
    # Belgenin sonundan itibaren 1 sayfa kaldır
    rem_opt = RemovePageRedaction(PageSeekOrigin.END, 0, 1)

    # Redakte edilecek belgeyi yükleyin
    with Redactor("./multipage_sample.pdf") as redactor:
        # Belge bilgilerini al
        doc_info = redactor.get_document_info()

        # Belgenin boş kalmaması için en az 2 sayfa gerektirir
        if doc_info.page_count > 1:
            # Kırpma işlemini uygula
            result = redactor.apply(rem_opt)

            # Redakte edilmiş belgeyi kaynak dosyanın yanına kaydedin
            so = SaveOptions()
            so.add_suffix = True
            so.rasterize_to_pdf = False
            so.redacted_file_suffix = "redacted"
            redactor.save(so)

if __name__ == "__main__":
    remove_last_page()
```

`multipage_sample.pdf` bu örnekte kullanılan örnek dosyadır. İndirmek için [buraya](https://docs.groupdocs.com/redaction/python-net/_sample_files/developer-guide/basic-usage/remove-page-redactions/multipage_sample.pdf) tıklayın.

  
```text
Binary file (PDF, 190 KB)
```
[Download full output](https://docs.groupdocs.com/redaction/python-net/_output_files/developer-guide/basic-usage/remove-page-redactions/remove_last_page/multipage_sample_redacted.pdf)

## Remove frame from image

Çok çerçeveli bir görüntü durumunda, birden fazla çerçeveyi ("sayfalar" olarak kabul edilen) silmeniz gerekebilir.

Aşağıdaki örnek, hareketli bir GIF görüntüsünden 3 çerçeveyi nasıl kaldıracağınızı gösterir:

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.options import SaveOptions
from groupdocs.redaction.redactions import RemovePageRedaction, PageSeekOrigin

def remove_frame_from_image():
    # 3. çerçeveden (sıfır tabanlı indeks 2) başlayarak çerçeveleri kaldır
    rem_opt = RemovePageRedaction(PageSeekOrigin.BEGIN, 2, 5)

    # Redakte edilecek çok çerçeveli görüntüyü yükle
    with Redactor("./sample.gif") as redactor:
        # Belge bilgilerini al
        doc_info = redactor.get_document_info()

        # En az 7 çerçeve gerektirir
        if doc_info.page_count >= 7:
            # Kırpma işlemini uygula
            result = redactor.apply(rem_opt)

            # Redakte edilmiş görüntüyü kaynak dosyanın yanına kaydet
            so = SaveOptions()
            so.add_suffix = True
            so.rasterize_to_pdf = False
            so.redacted_file_suffix = "redacted"
            redactor.save(so)

if __name__ == "__main__":
    remove_frame_from_image()
```

`sample.gif` bu örnekte kullanılan örnek dosyadır. İndirmek için [buraya](https://docs.groupdocs.com/redaction/python-net/_sample_files/developer-guide/basic-usage/remove-page-redactions/sample.gif) tıklayın.

  
```text
Binary file (GIF, 704 KB)
```
[Download full output](https://docs.groupdocs.com/redaction/python-net/_output_files/developer-guide/basic-usage/remove-page-redactions/remove_frame_from_image/sample_redacted.gif)
