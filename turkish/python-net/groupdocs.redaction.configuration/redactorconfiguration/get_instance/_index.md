---
title: "get_instance yöntemi"
second_title: "GroupDocs.Redaction for Python via .NET API Referansları"
description: "Yerleşik formatların varsayılan yapılandırmasıyla bir tek örnek döndürür."
type: docs
url: /tr/python-net/groupdocs.redaction.configuration/redactorconfiguration/get_instance/
is_root: false
weight: 1040
---


## get_instance

Yerleşik formatların varsayılan yapılandırmasıyla bir tek örnek döndürür.

```python
def get_instance(cls):
    ...
```

**Returns:** RedactorConfiguration: Configuration instance.

### Örnek

```python
from groupdocs.redaction.configuration import RedactorConfiguration

# Singleton yapılandırmayı elde edin
config = RedactorConfiguration.get_instance()

# Düz metin formatları için desteklenen uzantıları genişletin
txt_settings = config.find_format(".txt")
txt_settings.extension_filter += ",.dump"
```

### Ayrıca Bakınız
* class [`RedactorConfiguration`](/redaction/python-net/groupdocs.redaction.configuration/redactorconfiguration/)
