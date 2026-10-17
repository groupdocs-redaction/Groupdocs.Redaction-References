---
title: "find_format yöntemi"
second_title: "GroupDocs.Redaction for Python via .NET API Referansları"
description: "Belirli bir dosya uzantısı için format yapılandırmalarını bulur."
type: docs
url: /tr/python-net/groupdocs.redaction.configuration/redactorconfiguration/find_format/
is_root: false
weight: 1010
---


## find_format {#file_extension}

Belirli bir dosya uzantısı için format yapılandırmalarını bulur.

```python
def find_format(self, file_extension):
    ...
```

| Parametre | [ExactPhraseRedaction](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction.redactions/exactphraseredaction/), [RegexRedaction](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction.redactions/regexredaction/) | Açıklama |
| :- | :- | :- |
| file_extension | `str` | Dosya uzantısı, format ".ext". |

**Returns:** DocumentFormatConfiguration or None: If found, instance of DocumentFormatConfiguration, None otherwise.

### Örnek

```python
from groupdocs.redaction.configuration import RedactorConfiguration

# Singleton yapılandırma örneğini elde edin
config = RedactorConfiguration.get_instance()

# Belirli bir uzantı için format ayarlarını alın
settings = config.find_format(".txt")
if settings:
    # İşlenen uzantıların listesini genişletin, ör. .dump ekleyin
    settings.extension_filter = settings.extension_filter + ",.dump"
```

### Ayrıca Bakınız
* class [`RedactorConfiguration`](/redaction/python-net/groupdocs.redaction.configuration/redactorconfiguration/)
