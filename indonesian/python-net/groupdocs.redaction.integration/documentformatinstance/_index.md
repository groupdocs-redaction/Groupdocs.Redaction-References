---
title: "Kelas DocumentFormatInstance"
second_title: "Referensi API GroupDocs.Redaction untuk Python via .NET"
description: "Mewakili format khusus dari sebuah dokumen dan dapat diimplementasikan untuk menambahkan tipe dokumen khusus."
type: docs
url: /id/python-net/groupdocs.redaction.integration/documentformatinstance/
is_root: false
weight: 10
---


## DocumentFormatInstance class

Mewakili format khusus dari sebuah dokumen dan dapat diimplementasikan untuk menambahkan tipe dokumen khusus.

Pelajari lebih lanjut

- More details about implementing custom formats: https://docs.groupdocs.com/redaction/net/create-custom-format-handler/

Tipe DocumentFormatInstance menampilkan anggota-anggota berikut:

### Metode
| Metode | Deskripsi |
| :- | :- |
| [initialize](/redaction/python-net/groupdocs.redaction.integration/documentformatinstance/initialize/#config-settings) | Menginisialisasi instance penangan format dokumen. |
| [initialize_document_format_configuration](/redaction/python-net/groupdocs.redaction.integration/documentformatinstance/initialize_document_format_configuration/) |  |
| [is_redaction_accepted](/redaction/python-net/groupdocs.redaction.integration/documentformatinstance/is_redaction_accepted/#description) | Memeriksa implementasi [`IRedactionCallback`](/redaction/python-net/groupdocs.redaction.redactions/iredactioncallback/) dan memanggilnya, jika ditentukan. |
| [is_redaction_accepted_redaction_description](/redaction/python-net/groupdocs.redaction.integration/documentformatinstance/is_redaction_accepted_redaction_description/) |  |
| [load](/redaction/python-net/groupdocs.redaction.integration/documentformatinstance/load/#input) | Memuat dokumen dari aliran. |
| [load_stream](/redaction/python-net/groupdocs.redaction.integration/documentformatinstance/load_stream/) |  |
| [load_streams](/redaction/python-net/groupdocs.redaction.integration/documentformatinstance/load_streams/) |  |
| [perform_binary_check](/redaction/python-net/groupdocs.redaction.integration/documentformatinstance/perform_binary_check/#input) | Memeriksa apakah aliran yang diberikan berisi dokumen yang didukung oleh instance format ini. |
| [perform_binary_check_stream](/redaction/python-net/groupdocs.redaction.integration/documentformatinstance/perform_binary_check_stream/) |  |
| [perform_binary_check_streams](/redaction/python-net/groupdocs.redaction.integration/documentformatinstance/perform_binary_check_streams/) |  |
| [save](/redaction/python-net/groupdocs.redaction.integration/documentformatinstance/save/#output) | Menyimpan dokumen ke aliran. |
| [save_stream](/redaction/python-net/groupdocs.redaction.integration/documentformatinstance/save_stream/) |  |
| [save_streams](/redaction/python-net/groupdocs.redaction.integration/documentformatinstance/save_streams/) |  |

### Properti
| Properti | Deskripsi |
| :- | :- |
| [password](/redaction/python-net/groupdocs.redaction.integration/documentformatinstance/password/) | Kata sandi untuk dokumen yang dilindungi kata sandi. |

### Contoh

```python
class DummyDocument(DocumentFormatInstance):
    def load(self, output: io.RawIOBase) -> None:
        # memuat konten file
        pass

    def save(self, output: io.RawIOBase) -> None:
        # menyimpan perubahan ke file
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

### Lihat Juga
* module [`groupdocs.redaction.integration`](/redaction/python-net/groupdocs.redaction.integration/)
