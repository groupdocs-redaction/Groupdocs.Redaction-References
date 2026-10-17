---
title: "Metin redaksiyonu"
linkTitle: "Text redaction"
second_title: "GroupDocs.Redaction for Python via .NET API Referansları"
description: "Bu makale, Python redaksiyon API'sinin belgelerinizdeki hassas veya özel nitelikteki verileri kolayca redakte etmenizi nasıl sağladığını açıklar. PDF, DOC, DOCX, PPT, PPTX, XLS, XLSX ve diğer formatlardaki belgeler için kesin ifadeler veya düzenli ifadeler kullanarak metin redaksiyonu uygulayabilirsiniz."
type: docs
url: /tr/python-net/guides/text-redactions/
is_root: false
weight: 50
---


GroupDocs.Redaction, belgelerinizdeki hassas veya özel nitelikteki verileri kolayca redakte etmenizi sağlar. En yaygın redaksiyon durumu, bir belgeden metin kaldırmaktır.

GroupDocs.Redaction API'si ile PDF, DOC, DOCX, PPT, PPTX, XLS, XLSX ve diğer formatlardaki belgeler için kesin ifade veya [düzenli ifade](https://docs.microsoft.com/en-us/dotnet/standard/base-types/regular-expressions) kullanarak metin redaksiyonu uygulayabilirsiniz. Tam listeyi [desteklenen belge formatları]() makalesinde görebilirsiniz.

## Use exact phrase redaction

Aşağıdaki örnekte, kişisel kesin ifade "John Doe"yi "\[personal\]" (veya herhangi bir muafiyet kodu) ile değiştirerek metin redaksiyonu uyguluyoruz:

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.options import SaveOptions
from groupdocs.redaction.redactions import ExactPhraseRedaction, ReplacementOptions

def redact_exact_phrase():
    # Redaksiyon seçeneklerini belirtin
    repl_opt = ReplacementOptions("[personal]")
    ex_red = ExactPhraseRedaction("John Doe", repl_opt)

    # Redakte edilecek belgeyi yükleyin
    with Redactor("./sample.docx") as redactor:
        # Kırpma işlemini uygula
        result = redactor.apply(ex_red)

        # Redakte edilmiş belgeyi kaynak dosyanın yanına kaydedin
        so = SaveOptions()
        so.add_suffix = True
        so.rasterize_to_pdf = False
        so.redacted_file_suffix = "redacted"
        redactor.save(so)

if __name__ == "__main__":
    redact_exact_phrase()
```

`sample.docx` bu örnekte kullanılan örnek dosyadır. İndirmek için [buraya](https://docs.groupdocs.com/redaction/python-net/_sample_files/developer-guide/basic-usage/text-redactions/sample.docx) tıklayın.

  
```text
Binary file (DOCX, 16 KB)
```
[Download full output](https://docs.groupdocs.com/redaction/python-net/_output_files/developer-guide/basic-usage/text-redactions/redact_exact_phrase/sample_redacted.docx)

Varsayılan olarak, tam ifadeyi arama büyük/küçük harfe duyarsızdır. Büyük/küçük harfe duyarlı bir redaksiyon için bir yapıcı parametresi ve ilgili ortak özellik vardır:

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.options import SaveOptions
from groupdocs.redaction.redactions import ExactPhraseRedaction, ReplacementOptions

def redact_case_sensitive_phrase():
    # Büyük/küçük harfe duyarlı eşleşmeyi etkinleştir
    case_sensitive = True

    # Redaksiyon seçeneklerini belirtin
    repl_opt = ReplacementOptions("[personal]")
    ex_red = ExactPhraseRedaction("John Doe", case_sensitive, repl_opt)

    # Redakte edilecek belgeyi yükleyin
    with Redactor("./sample.docx") as redactor:
        # Kırpma işlemini uygula
        result = redactor.apply(ex_red)

        # Redakte edilmiş belgeyi kaynak dosyanın yanına kaydedin
        so = SaveOptions()
        so.add_suffix = True
        so.rasterize_to_pdf = False
        so.redacted_file_suffix = "redacted"
        redactor.save(so)

if __name__ == "__main__":
    redact_case_sensitive_phrase()
```

`sample.docx` bu örnekte kullanılan örnek dosyadır. İndirmek için [buraya](https://docs.groupdocs.com/redaction/python-net/_sample_files/developer-guide/basic-usage/text-redactions/sample.docx) tıklayın.

  
```text
Binary file (DOCX, 16 KB)
```
[Download full output](https://docs.groupdocs.com/redaction/python-net/_output_files/developer-guide/basic-usage/text-redactions/redact_case_sensitive_phrase/sample_redacted.docx)

Kırpılmış metnin üzerine renkli bir kutu eklemeniz gerekiyorsa, yerine geçecek dize yerine renk kullanabilirsiniz. Redaksiyon eşleşen metni silecek ve kırpılmış metnin yerine belirtilen renkte bir dikdörtgen yerleştirecektir:

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.options import SaveOptions
from groupdocs.redaction.redactions import ExactPhraseRedaction, ReplacementOptions
from groupdocs.pydrawing import Color

def redact_with_color_box():
    # Redaksiyon kutusunun rengini tanımlayın
    color = Color.from_argb(255, 220, 20, 60)

    # Redaksiyon seçeneklerini belirtin
    repl_opt = ReplacementOptions(color)
    ex_red = ExactPhraseRedaction("John Doe", repl_opt)

    # Redakte edilecek belgeyi yükleyin
    with Redactor("./sample.docx") as redactor:
        # Kırpma işlemini uygula
        result = redactor.apply(ex_red)

        # Redakte edilmiş belgeyi kaynak dosyanın yanına kaydedin
        so = SaveOptions()
        so.add_suffix = True
        so.rasterize_to_pdf = False
        so.redacted_file_suffix = "redacted"
        redactor.save(so)

if __name__ == "__main__":
    redact_with_color_box()
```

`sample.docx` bu örnekte kullanılan örnek dosyadır. İndirmek için [buraya](https://docs.groupdocs.com/redaction/python-net/_sample_files/developer-guide/basic-usage/text-redactions/sample.docx) tıklayın.

  
```text
Binary file (DOCX, 17 KB)
```
[Download full output](https://docs.groupdocs.com/redaction/python-net/_output_files/developer-guide/basic-usage/text-redactions/redact_with_color_box/sample_redacted.docx)

Sağdan sola yazılan bir belgeye, örneğin Arapça veya İbranice, redaksiyon uygulamanız gerekebilir. Aşağıdaki örnek, ExactPhraseRedaction'ı bir Arapça PDF belgesine nasıl uygulayacağınızı gösterir:

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.options import SaveOptions
from groupdocs.redaction.redactions import ExactPhraseRedaction, ReplacementOptions

def redact_right_to_left_text():
    # `arabic.pdf` bu örnekte kullanılan örnek dosyadır. İndirmek için [buraya](https://docs.groupdocs.com/redaction/python-net/_sample_files/developer-guide/basic-usage/text-redactions/arabic.pdf) tıklayın.
    repl_opt = ReplacementOptions("[test]")
    ex_red = ExactPhraseRedaction("انتقد", repl_opt)

    # Redakte edilecek belgeyi yükleyin
    with Redactor("./arabic.pdf") as redactor:
        # Kırpma işlemini uygula
        result = redactor.apply(ex_red)

        # Redakte edilmiş belgeyi kaynak dosyanın yanına kaydedin
        so = SaveOptions()
        so.add_suffix = True
        so.rasterize_to_pdf = False
        so.redacted_file_suffix = "redacted"
        redactor.save(so)

if __name__ == "__main__":
    redact_right_to_left_text()
```

Arka planda, "tam ifade" redaksiyonu, redaksiyon için temel yaklaşım olan düzenli ifadeler aracılığıyla çalışır. Aşağıdaki örnekte, "2 rakam, boşluk ya da hiç bir şey, 2 rakam, tekrar boşluk ve 6 rakam" eşleşen herhangi bir metni mavi renkli bir kutu ile kırpıyoruz:

  
```text
Binary file (PDF, 23 KB)
```
[Download full output](https://docs.groupdocs.com/redaction/python-net/_output_files/developer-guide/basic-usage/text-redactions/redact_right_to_left_text/arabic_redacted.pdf)

## Use regular expression

Tüm bir paragrafı kırpmak istiyorsanız, RegexRedaction kullanmanız da gerekebilir. Aşağıdaki örnek, bir PDF belgesinde tüm paragrafı nasıl kırpacağınızı gösterir:

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.options import SaveOptions
from groupdocs.redaction.redactions import RegexRedaction, ReplacementOptions
from groupdocs.pydrawing import Color

def redact_with_regex():
    # Redaksiyon kutusunun rengini tanımlayın
    color = Color.from_argb(255, 220, 20, 60)

    # Redaksiyon seçeneklerini belirtin
    repl_opt = ReplacementOptions(color)
    reg_red = RegexRedaction("\\d{2}\\s*\\d{2}[^\\d]*\\d{6}", repl_opt)

    # Redakte edilecek belgeyi yükleyin
    with Redactor("./sample.docx") as redactor:
        # Kırpma işlemini uygula
        result = redactor.apply(reg_red)

        # Redakte edilmiş belgeyi kaynak dosyanın yanına kaydedin
        so = SaveOptions()
        so.add_suffix = True
        so.rasterize_to_pdf = False
        so.redacted_file_suffix = "redacted"
        redactor.save(so)

if __name__ == "__main__":
    redact_with_regex()
```

`sample.docx` bu örnekte kullanılan örnek dosyadır. İndirmek için [buraya](https://docs.groupdocs.com/redaction/python-net/_sample_files/developer-guide/basic-usage/text-redactions/sample.docx) tıklayın.

  
```text
Binary file (DOCX, 16 KB)
```
[Download full output](https://docs.groupdocs.com/redaction/python-net/_output_files/developer-guide/basic-usage/text-redactions/redact_with_regex/sample_redacted.docx)

Tüm bir paragrafı eşleyecek redaksiyon seçeneklerini belirtin

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.options import SaveOptions
from groupdocs.redaction.redactions import RegexRedaction, ReplacementOptions
from groupdocs.pydrawing import Color

def redact_whole_paragraph():
    # Redaksiyon kutusunun rengini tanımlayın
    color = Color.from_argb(255, 220, 20, 60)

    # `sample.pdf` bu örnekte kullanılan örnek dosyadır. İndirmek için [buraya](https://docs.groupdocs.com/redaction/python-net/_sample_files/developer-guide/basic-usage/text-redactions/sample.pdf) tıklayın.
    repl_opt = ReplacementOptions(color)
    reg_red = RegexRedaction("(Lorem(\n|.)+?urna)", repl_opt)

    # Redakte edilecek belgeyi yükleyin
    with Redactor("./sample.pdf") as redactor:
        # Kırpma işlemini uygula
        result = redactor.apply(reg_red)

        # Redakte edilmiş belgeyi kaynak dosyanın yanına kaydedin
        so = SaveOptions()
        so.add_suffix = True
        so.rasterize_to_pdf = False
        so.redacted_file_suffix = "redacted"
        redactor.save(so)

if __name__ == "__main__":
    redact_whole_paragraph()
```

Desteklenen dosya formatlarını alın

  
```text
Binary file (PDF, 68 KB)
```
[Download full output](https://docs.groupdocs.com/redaction/python-net/_output_files/developer-guide/basic-usage/text-redactions/redact_whole_paragraph/sample_redacted.pdf)
