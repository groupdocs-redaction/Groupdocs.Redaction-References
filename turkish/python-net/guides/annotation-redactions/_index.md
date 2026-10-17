---
title: "Ek açıklama kırpmaları"
linkTitle: "Annotation redactions"
second_title: "GroupDocs.Redaction for Python via .NET API Referansları"
description: "Bu makale, PDF, DOC, DOCX, PPT, PPTX, XLS, XLSX ve diğerleri gibi farklı formatlardaki belgeler için ek açıklama kırpmasının uygulanmasını gösterir."
type: docs
url: /tr/python-net/guides/annotation-redactions/
is_root: false
weight: 80
---


GroupDocs.Redaction API ile PDF, DOC, DOCX, PPT, PPTX, XLS, XLSX ve diğerleri gibi farklı formatlardaki belgeler için ek açıklama kırpmaları uygulayabilirsiniz. Tam listeyi [desteklenen belge formatları]() makalesinde görebilirsiniz.

GroupDocs.Redactions, ek açıklama metninden hassas verileri kaldırmanıza veya düzenli ifade kullanarak ek açıklamaları tamamen silmenize olanak tanıyan esnek bir API sunar.

## Remove annotations (comments etc)

GroupDocs.Redaction'ı belge içindeki tüm veya belirli yorumları ve diğer ek açıklamaları kaldırmak için kullanabilirsiniz. Örneğin, içinde "use", "show" veya "describe" gibi metinler bulunan tüm yorumları belge üzerinden kaldırabiliriz:

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.options import SaveOptions
from groupdocs.redaction.redactions import DeleteAnnotationRedaction

def remove_all_annotations():
    # Desene uyan ek açıklamaları silmek için kırpma seçeneklerini belirtin
    a_red = DeleteAnnotationRedaction("(?im:(use|show|describe))")

    # Redakte edilecek belgeyi yükleyin
    with Redactor("./annotated.xlsx") as redactor:
        # Kırpma işlemini uygula
        result = redactor.apply(a_red)

        # Redakte edilmiş belgeyi kaynak dosyanın yanına kaydedin
        so = SaveOptions()
        so.add_suffix = True
        so.rasterize_to_pdf = False
        so.redacted_file_suffix = "redacted"
        redactor.save(so)

if __name__ == "__main__":
    remove_all_annotations()
```

`annotated.xlsx` bu örnekte kullanılan örnek dosyadır. İndirmek için [buraya](https://docs.groupdocs.com/redaction/python-net/_sample_files/developer-guide/basic-usage/annotation-redactions/annotated.xlsx) tıklayın.

  
```text
Binary file (XLSX, 12 KB)
```
[Download full output](https://docs.groupdocs.com/redaction/python-net/_output_files/developer-guide/basic-usage/annotation-redactions/remove_all_annotations/annotated_redacted.xlsx)

Belge içindeki tüm ek açıklamaları kaldırmak için yapıcıyı argümansız kullanabilirsiniz.

## Redact annotations

Tüm veya belirli açıklamaları kaldırmak yerine, açıklama metnindeki hassas verileri kaldırabilirsiniz. Örneğin, verilen belgede "John" adlı tüm geçişleri kaldırabiliriz, örn.:

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.options import SaveOptions
from groupdocs.redaction.redactions import AnnotationRedaction

def redact_annotations():
    # Redaksiyon seçeneklerini belirtin: arama deseni ve değiştirme dizesi
    a_red = AnnotationRedaction("(?im:john)", "[redacted]")

    # Redakte edilecek belgeyi yükleyin
    with Redactor("./annotated.xlsx") as redactor:
        # Kırpma işlemini uygula
        result = redactor.apply(a_red)

        # Redakte edilmiş belgeyi kaynak dosyanın yanına kaydedin
        so = SaveOptions()
        so.add_suffix = True
        so.rasterize_to_pdf = False
        so.redacted_file_suffix = "redacted"
        redactor.save(so)

if __name__ == "__main__":
    redact_annotations()
```

`annotated.xlsx` bu örnekte kullanılan örnek dosyadır. İndirmek için [buraya](https://docs.groupdocs.com/redaction/python-net/_sample_files/developer-guide/basic-usage/annotation-redactions/annotated.xlsx) tıklayın.

  
```text
Binary file (XLSX, 12 KB)
```
[Download full output](https://docs.groupdocs.com/redaction/python-net/_output_files/developer-guide/basic-usage/annotation-redactions/redact_annotations/annotated_redacted.xlsx)
