---
title: "Merhaba, Dünya!"
linkTitle: "Hello, World!"
second_title: "GroupDocs.Redaction for Python via .NET API Referansları"
description: "GroupDocs.Redaction for Python via .NET'i basit bir örnek oluşturarak ve çalıştırarak hızlıca başlayın."
type: docs
url: /tr/python-net/guides/hello-world/
is_root: false
weight: 20
---


## Introduction
GroupDocs.Redaction for Python via .NET'i keşfederken "Hello, World!" örneği genellikle ilk adımdır. Bu, geliştirme ortamınızın doğru şekilde kurulduğunu ve kütüphanenin beklendiği gibi çalıştığını doğrulamak için basit bir test işlevi görür.

## Overview
GroupDocs.Redaction for Python via .NET, çeşitli belge formatlarından hassas bilgileri aramanıza, kırpmanıza ve kaldırmanıza olanak tanır. Geniş bir [desteklenen formatlar](https://docs.groupdocs.com/redaction/python-net/getting-started/supported-document-formats/) yelpazesi, farklı kullanım senaryoları için çok yönlü olmasını sağlar.

## How to redact a document
Aşağıdaki adımlar, GroupDocs.Redaction for Python via .NET kullanarak bir belgeden hassas bilgileri nasıl kırpacağınızı gösterir:

1. İhtiyacınız olan `groupdocs.redaction` sınıflarını içe aktarın.
2. Kırpmayı tanımlayın (burada, renkli bir kutuyla değiştirilecek tam ifadeyi).
3. Örnek belge yolunu kullanarak bir [`Redactor`](/redaction/python-net/groupdocs.redaction/redactor/) nesnesi oluşturun.
4. Kırpmayı uygulayın.
5. Sonucu kaydedin.

## Complete example
Aşağıdaki örnek, "John Doe" ifadesinin her geçişini yarı saydam kırmızı bir kutuyla değiştirir ve kırpılmış belgeyi kaydeder:

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.options import SaveOptions
from groupdocs.redaction.redactions import ExactPhraseRedaction, ReplacementOptions
from groupdocs.pydrawing import Color

def hello_world():
    # "John Doe" ifadesinin her geçişinin üzerine yarı saydam kırmızı bir kutu çizin
    options = ReplacementOptions(Color.from_argb(128, 255, 0, 0))
    redaction = ExactPhraseRedaction("John Doe", options)

    # Belgeyi yükleyin, kırpmayı uygulayın ve sonucu kaydedin
    with Redactor("./sample.docx") as redactor:
        redactor.apply(redaction)
        save_options = SaveOptions()
        save_options.add_suffix = True
        save_options.rasterize_to_pdf = True
        save_options.redacted_file_suffix = "redacted"
        result_path = redactor.save(save_options)

    print(f"Document redacted successfully. Output saved to {result_path}.")

if __name__ == "__main__":
    hello_world()
```

`sample.docx` bu örnekte kullanılan örnek dosyadır. İndirmek için [buraya](https://docs.groupdocs.com/redaction/python-net/_sample_files/getting-started/hello-world/sample.docx) tıklayın.

  
```text
Binary file (PDF, 1.0 MB)
```
[Download full output](https://docs.groupdocs.com/redaction/python-net/_output_files/getting-started/hello-world/hello_world/sample_redacted.pdf)

Bu örnek, sonucu `sample_redacted.pdf` adlı bir PDF'ye rasterleştirir, böylece kırpılmış içerik geri alınamaz (`save()` varsayılan olarak PDF'ye rasterleştirir; `redacted_file_suffix` seçeneği yalnızca çıktı adını kontrol eder). Orijinal formatı korumak için `rasterize_to_pdf = False` olarak ayarlayın.

## Additional resources
Bu demo, GroupDocs.Redaction for Python via .NET [kod örneklerine](https://github.com/groupdocs-redaction/GroupDocs.Redaction-for-Python-via-.NET/) referans verir.
