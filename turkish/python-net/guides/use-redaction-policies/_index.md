---
title: "Redaksiyon politikalarını kullanın"
linkTitle: "Use redaction policies"
second_title: "GroupDocs.Redaction for Python via .NET API Referansları"
description: "Nasıl başa çıkılacağını öğrenin. Kurumsal hassas veri silme politikanız bir redaksiyon kuralı listesi ise, bunları kodunuzda belirtmeniz gerekmez. Önceden yapılandırılmış redaksiyonların bir listesini içeren bir XML belgesi belirtebilirsiniz."
type: docs
url: /tr/python-net/guides/use-redaction-policies/
is_root: false
weight: 110
---


Kurumsal hassas veri silme politikanız bir redaksiyon kuralı listesi ise, bunları kodunuzda belirtmeniz gerekmez. Önceden yapılandırılmış redaksiyonların bir listesini içeren bir XML belgesi belirtebilirsiniz.

Aşağıda redaksiyon politikası XML dosyasının bir örneği (kod özellikleri eşlemesi açıktır) verilmiştir:

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
Bu yapıda XML belgeleri oluşturmak için RedactionPolicy.save() yöntemini kullanabilir, redaksiyonları çalışma zamanında yapılandırabilirsiniz.

Aşağıdaki örnek, bir [RedactionPolicy](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction/redactionpolicy/) öğesini XML dosyasına nasıl kaydedeceğinizi gösterir.
 

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
    # Redaksiyon rengini tanımlayın
    color = Color.from_argb(255, 220, 20, 60)

    # Redaksiyonları yapılandırın
    redactions = [
        ExactPhraseRedaction("Redaction", ReplacementOptions("[Product]")),
        RegexRedaction("\\d{2}\\s*\\d{2}[^\\d]*\\d{6}", ReplacementOptions(color)),
        DeleteAnnotationRedaction(),
        EraseMetadataRedaction(MetadataFilters.ALL),
    ]

    # Politikayı oluşturun
    policy = RedactionPolicy(redactions)

    # Redaksiyon politikasını bir XML dosyasına kaydedin
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

İhtiyacınız kadar politika oluşturabilirsiniz; bunları belgelerinizi redakte etmek için yükleyin.

Aşağıdaki örnek, bir XML dosyasından bir redaksiyon politikasını yükler ve içinde bulunan her kuralı tek bir `apply` çağrısında bir belgeye uygular:

```python
from groupdocs.redaction import Redactor, RedactionPolicy
from groupdocs.redaction.options import SaveOptions

def use_redaction_policy():
    # Redaksiyon politikasını bir XML dosyasından yükleyin
    policy = RedactionPolicy.load("./redaction_policy.xml")

    # Belgeyi yükleyin ve tüm politikayı tek bir çağrıda uygulayın
    with Redactor("./sample.docx") as redactor:
        redactor.apply(policy)

        # Orijinal formatı koruyun ve çıktı adının sonuna bir ek ekleyin
        save_options = SaveOptions()
        save_options.add_suffix = True
        save_options.rasterize_to_pdf = False
        save_options.redacted_file_suffix = "redacted"
        result_path = redactor.save(save_options)

    print(f"Redaction policy applied. Output saved to {result_path}.")

if __name__ == "__main__":
    use_redaction_policy()
```

`redaction_policy.xml` bu örnekte kullanılan politika dosyasıdır. İndirmek için [buraya](https://docs.groupdocs.com/redaction/python-net/_sample_files/developer-guide/advanced-usage/use-redaction-policies/redaction_policy.xml) tıklayın.

`sample.docx` bu örnekte redakte edilen belgedir. İndirmek için [buraya](https://docs.groupdocs.com/redaction/python-net/_sample_files/developer-guide/advanced-usage/use-redaction-policies/sample.docx) tıklayın.

  
```text
Binary file (DOCX, 16 KB)
```
[Download full output](https://docs.groupdocs.com/redaction/python-net/_output_files/developer-guide/advanced-usage/use-redaction-policies/use_redaction_policy/sample_redacted.docx)
