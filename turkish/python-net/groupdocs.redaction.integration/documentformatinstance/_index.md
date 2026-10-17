---
title: "DocumentFormatInstance sınıfı"
second_title: "GroupDocs.Redaction for Python via .NET API Referansları"
description: "Belirli bir belge formatını temsil eder ve özel belge türleri eklemek için uygulanabilir."
type: docs
url: /tr/python-net/groupdocs.redaction.integration/documentformatinstance/
is_root: false
weight: 10
---


## DocumentFormatInstance class

Belirli bir belge formatını temsil eder ve özel belge türleri eklemek için uygulanabilir.

Daha fazla bilgi edinin

- More details about implementing custom formats: https://docs.groupdocs.com/redaction/net/create-custom-format-handler/

DocumentFormatInstance türü aşağıdaki üyeleri sunar:

### Yöntemler
| Yöntem | Açıklama |
| :- | :- |
| [initialize](/redaction/python-net/groupdocs.redaction.integration/documentformatinstance/initialize/#config-settings) | Belge formatı işleyici örneğini başlatır. |
| [initialize_document_format_configuration](/redaction/python-net/groupdocs.redaction.integration/documentformatinstance/initialize_document_format_configuration/) |  |
| [is_redaction_accepted](/redaction/python-net/groupdocs.redaction.integration/documentformatinstance/is_redaction_accepted/#description) | [`IRedactionCallback`](/redaction/python-net/groupdocs.redaction.redactions/iredactioncallback/) uygulamasını kontrol eder ve belirtilmişse çağırır. |
| [is_redaction_accepted_redaction_description](/redaction/python-net/groupdocs.redaction.integration/documentformatinstance/is_redaction_accepted_redaction_description/) |  |
| [load](/redaction/python-net/groupdocs.redaction.integration/documentformatinstance/load/#input) | Belgeyi bir akıştan yükler. |
| [load_stream](/redaction/python-net/groupdocs.redaction.integration/documentformatinstance/load_stream/) |  |
| [load_streams](/redaction/python-net/groupdocs.redaction.integration/documentformatinstance/load_streams/) |  |
| [perform_binary_check](/redaction/python-net/groupdocs.redaction.integration/documentformatinstance/perform_binary_check/#input) | Verilen akışın bu format örneği tarafından desteklenen bir belge içerip içermediğini kontrol eder. |
| [perform_binary_check_stream](/redaction/python-net/groupdocs.redaction.integration/documentformatinstance/perform_binary_check_stream/) |  |
| [perform_binary_check_streams](/redaction/python-net/groupdocs.redaction.integration/documentformatinstance/perform_binary_check_streams/) |  |
| [save](/redaction/python-net/groupdocs.redaction.integration/documentformatinstance/save/#output) | Belgeyi bir akışa kaydeder. |
| [save_stream](/redaction/python-net/groupdocs.redaction.integration/documentformatinstance/save_stream/) |  |
| [save_streams](/redaction/python-net/groupdocs.redaction.integration/documentformatinstance/save_streams/) |  |

### Özellikler
| Özellik | Açıklama |
| :- | :- |
| [password](/redaction/python-net/groupdocs.redaction.integration/documentformatinstance/password/) | Şifre korumalı belgeler için şifre. |

### Örnek

```python
class DummyDocument(DocumentFormatInstance):
    def load(self, output: io.RawIOBase) -> None:
        # dosya içeriğini yükle
        pass

    def save(self, output: io.RawIOBase) -> None:
        # değişiklikleri dosyaya kaydet
        pass
```

```python
class MyCustomHandler(DocumentFormatInstance):
    def __init__(self):
        self.my_property = None

    def initialize(self, config: DocumentFormatConfiguration) -> None:
        super().initialize(config)
        if "MyProperty" in config.initialization_data:
            self.my_property = config.initialization_data["MyProperty"]
```

### Ayrıca Bakınız
* module [`groupdocs.redaction.integration`](/redaction/python-net/groupdocs.redaction.integration/)
