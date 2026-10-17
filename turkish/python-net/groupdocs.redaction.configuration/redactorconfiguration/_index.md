---
title: "RedactorConfiguration sınıfı"
second_title: "GroupDocs.Redaction for Python via .NET API Referansları"
description: "Yerleşik ve özel kullanıcı formatları dahil olmak üzere desteklenen formatların bir listesine erişim sağlar."
type: docs
url: /tr/python-net/groupdocs.redaction.configuration/redactorconfiguration/
is_root: false
weight: 20
---


## RedactorConfiguration class

Yerleşik ve özel kullanıcı formatları dahil olmak üzere desteklenen formatların bir listesine erişim sağlar.

Daha fazla bilgi:

- More details about GroupDocs.Redaction configuration: https://docs.groupdocs.com/redaction/net/extend-supported-extensions-list/
- More details about implementing custom formats: https://docs.groupdocs.com/redaction/net/create-custom-format-handler/

RedactorConfiguration türü aşağıdaki üyeleri gösterir:

### Yöntemler
| Yöntem | Açıklama |
| :- | :- |
| [find_format](/redaction/python-net/groupdocs.redaction.configuration/redactorconfiguration/find_format/#file_extension) | Belirli bir dosya uzantısı için format yapılandırmalarını bulur. |
| [find_format_file](/redaction/python-net/groupdocs.redaction.configuration/redactorconfiguration/find_format_file/) |  |
| [find_format_string](/redaction/python-net/groupdocs.redaction.configuration/redactorconfiguration/find_format_string/) |  |
| [get_instance](/redaction/python-net/groupdocs.redaction.configuration/redactorconfiguration/get_instance/) | Yerleşik formatların varsayılan yapılandırmasıyla bir tek örnek döndürür. |

### Özellikler
| Özellik | Açıklama |
| :- | :- |
| [available_formats](/redaction/python-net/groupdocs.redaction.configuration/redactorconfiguration/available_formats/) | Tanımlanan formatların listesi, bakınız [`DocumentFormatConfiguration`](/redaction/python-net/groupdocs.redaction.configuration/documentformatconfiguration/). |

### Örnek

```python
# Özel bir kullanıcı format işleyicisi ekleyin
adobe_photoshop_settings = DocumentFormatConfiguration()
adobe_photoshop_settings.extension_filter = ".psd"
adobe_photoshop_settings.document_type = MyAdobePhotoshopFormatInstance

config = RedactorConfiguration.get_instance()
config.available_formats.add(adobe_photoshop_settings)
```

```python
# Yerleşik veya özel bir kullanıcı format işleyicisini alın
config = RedactorConfiguration.get_instance()
format_settings = config.find_format(".psd")
```

### Ayrıca Bakınız
* module [`groupdocs.redaction.configuration`](/redaction/python-net/groupdocs.redaction.configuration/)
