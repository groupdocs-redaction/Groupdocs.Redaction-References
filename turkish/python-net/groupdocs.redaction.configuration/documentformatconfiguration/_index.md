---
title: "DocumentFormatConfiguration sınıfı"
second_title: "GroupDocs.Redaction for Python via .NET API Referansları"
description: "DocumentFormatInstance türevi sınıfı için bir tür referansı ve daha hızlı format algılaması için desteklenen dosya uzantılarının bir listesini temsil eder."
type: docs
url: /tr/python-net/groupdocs.redaction.configuration/documentformatconfiguration/
is_root: false
weight: 10
---


## DocumentFormatConfiguration class

`[`DocumentFormatInstance`](/redaction/python-net/groupdocs.redaction.integration/documentformatinstance/)-türetilmiş sınıfı için bir tip referansını ve daha hızlı format algılaması için desteklenen dosya uzantılarının listesini temsil eder.

Daha fazla bilgi edinin

- More details about **GroupDocs.Redaction** configuration: https://docs.groupdocs.com/redaction/net/extend-supported-extensions-list/
- More details about implementing custom formats: https://docs.groupdocs.com/redaction/net/create-custom-format-handler/

DocumentFormatConfiguration türü aşağıdaki üyeleri gösterir:

### Yapıcılar
| Yapıcı | Açıklama |
| :- | :- |
| [__init__](/redaction/python-net/groupdocs.redaction.configuration/documentformatconfiguration/__init__/) | Yeni bir DocumentFormatConfiguration örneği başlatır. |

### Yöntemler
| Yöntem | Açıklama |
| :- | :- |
| [supports_extension](/redaction/python-net/groupdocs.redaction.configuration/documentformatconfiguration/supports_extension/#file_extension) | Verilen bir dosya uzantısının DocumentType olarak işlenip işlenemeyeceğini kontrol eder. |
| [supports_extension_file](/redaction/python-net/groupdocs.redaction.configuration/documentformatconfiguration/supports_extension_file/) |  |
| [supports_extension_string](/redaction/python-net/groupdocs.redaction.configuration/documentformatconfiguration/supports_extension_string/) |  |

### Özellikler
| Özellik | Açıklama |
| :- | :- |
| [document_type](/redaction/python-net/groupdocs.redaction.configuration/documentformatconfiguration/document_type/) | [`DocumentFormatInstance`](/redaction/python-net/groupdocs.redaction.integration/documentformatinstance/) sınıfından miras alan bir sınıfın türü. |
| [extension_filter](/redaction/python-net/groupdocs.redaction.configuration/documentformatconfiguration/extension_filter/) | Virgül‑ile ayrılmış dosya uzantıları listesi (örneğin ".pdf"), büyük‑küçük harfe duyarsız. |
| [initialization_data](/redaction/python-net/groupdocs.redaction.configuration/documentformatconfiguration/initialization_data/) | [`DocumentFormatInstance`](/redaction/python-net/groupdocs.redaction.integration/documentformatinstance/) başlatması için gereken veri. |

### Örnek

```python
from groupdocs.redaction import DocumentFormatConfiguration

# Özel bir format yapılandırması oluşturun
config = DocumentFormatConfiguration()
config.ExtensionFilter = ".psd"
config.DocumentType = MyAdobePhotoshopFormatInstance
```

### Ayrıca Bakınız
* module [`groupdocs.redaction.configuration`](/redaction/python-net/groupdocs.redaction.configuration/)
