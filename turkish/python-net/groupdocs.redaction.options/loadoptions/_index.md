---
title: "LoadOptions sınıfı"
second_title: "GroupDocs.Redaction for Python via .NET API Referansları"
description: "Bir dosyayı açmak için kullanılacak seçenekleri sağlar."
type: docs
url: /tr/python-net/groupdocs.redaction.options/loadoptions/
is_root: false
weight: 40
---


## LoadOptions class

Bir dosyayı açmak için kullanılacak seçenekleri sağlar.

Daha fazla bilgi edinin
- [Loading documents](https://docs.groupdocs.com/redaction/net/loading-documents/)
- [Load from local disk](https://docs.groupdocs.com/redaction/net/load-from-local-disc/)
- [Load from stream](https://docs.groupdocs.com/redaction/net/load-from-stream/)
- [Load password-protected document](https://docs.groupdocs.com/redaction/net/load-password-protected-file/)

LoadOptions türü aşağıdaki üyeleri gösterir:

### Yapıcılar
| Yapıcı | Açıklama |
| :- | :- |
| [__init__](/redaction/python-net/groupdocs.redaction.options/loadoptions/__init__/) | LoadOptions sınıfının yeni bir örneğini başlatır. |
| [__init__](/redaction/python-net/groupdocs.redaction.options/loadoptions/__init__/#password) | Belirtilen şifre ile LoadOptions'ın yeni bir örneğini başlatır. |
| [__init__](/redaction/python-net/groupdocs.redaction.options/loadoptions/__init__/#pre_rasterize) | Belirtilen ön‑tarama bayrağı ile yeni bir LoadOptions örneğini başlatır. |
| [__init__](/redaction/python-net/groupdocs.redaction.options/loadoptions/__init__/#password-pre_rasterize) | Belirtilen şifre ile yeni bir LoadOptions örneğini başlatır. |

### Özellikler
| Özellik | Açıklama |
| :- | :- |
| [password](/redaction/python-net/groupdocs.redaction.options/loadoptions/password/) | Şifre korumalı belgeler için şifre. |
| [pre_rasterize](/redaction/python-net/groupdocs.redaction.options/loadoptions/pre_rasterize/) | pre_rasterize bayrağı, dosyanın ön‑tarama yapılması gerekip gerekmediğini gösterir. |

### Örnek

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.options import LoadOptions, SaveOptions
from groupdocs.redaction.redactions import ExactPhraseRedaction, ReplacementOptions

# Belge şifresi ile yükleme seçeneklerini belirtin
load_opt = LoadOptions("mypassword")

# Bir redaksiyon tanımlayın
repl_opt = ReplacementOptions("[personal]")
ex_red = ExactPhraseRedaction("John Doe", repl_opt)

# Şifre korumalı belgeyi açın
with Redactor("./protected.docx", load_opt) as redactor:
    redactor.apply(ex_red)

    # Redakte edilmiş belgeyi kaydedin
    save_opt = SaveOptions()
    save_opt.add_suffix = True
    result_path = redactor.save(save_opt)
    print(f"Document redacted successfully. Check output in {result_path}.")
```

### Ayrıca Bakınız
* module [`groupdocs.redaction.options`](/redaction/python-net/groupdocs.redaction.options/)
