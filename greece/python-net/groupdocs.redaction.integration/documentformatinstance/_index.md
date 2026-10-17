---
title: "DocumentFormatInstance κλάση"
second_title: "Αναφορές API του GroupDocs.Redaction για Python μέσω .NET"
description: "Αντιπροσωπεύει μια συγκεκριμένη μορφή εγγράφου και μπορεί να υλοποιηθεί για την προσθήκη προσαρμοσμένων τύπων εγγράφων."
type: docs
url: /el/python-net/groupdocs.redaction.integration/documentformatinstance/
is_root: false
weight: 10
---


## DocumentFormatInstance class

Αντιπροσωπεύει μια συγκεκριμένη μορφή εγγράφου και μπορεί να υλοποιηθεί για την προσθήκη προσαρμοσμένων τύπων εγγράφων.

Μάθετε περισσότερα

- More details about implementing custom formats: https://docs.groupdocs.com/redaction/net/create-custom-format-handler/

Ο τύπος DocumentFormatInstance εκθέτει τα παρακάτω μέλη:

### Μέθοδοι
| Μέθοδος | Περιγραφή |
| :- | :- |
| [initialize](/redaction/python-net/groupdocs.redaction.integration/documentformatinstance/initialize/#config-settings) | Αρχικοποιεί την παρουσία του χειριστή μορφής εγγράφου. |
| [initialize_document_format_configuration](/redaction/python-net/groupdocs.redaction.integration/documentformatinstance/initialize_document_format_configuration/) |  |
| [is_redaction_accepted](/redaction/python-net/groupdocs.redaction.integration/documentformatinstance/is_redaction_accepted/#description) | Ελέγχει για [`IRedactionCallback`](/redaction/python-net/groupdocs.redaction.redactions/iredactioncallback/) υλοποίηση και την καλεί, εάν καθοριστεί. |
| [is_redaction_accepted_redaction_description](/redaction/python-net/groupdocs.redaction.integration/documentformatinstance/is_redaction_accepted_redaction_description/) |  |
| [load](/redaction/python-net/groupdocs.redaction.integration/documentformatinstance/load/#input) | Φορτώνει το έγγραφο από μια ροή. |
| [load_stream](/redaction/python-net/groupdocs.redaction.integration/documentformatinstance/load_stream/) |  |
| [load_streams](/redaction/python-net/groupdocs.redaction.integration/documentformatinstance/load_streams/) |  |
| [perform_binary_check](/redaction/python-net/groupdocs.redaction.integration/documentformatinstance/perform_binary_check/#input) | Ελέγχει αν η δοθείσα ροή περιέχει έγγραφο που υποστηρίζεται από αυτήν την παρουσία μορφής. |
| [perform_binary_check_stream](/redaction/python-net/groupdocs.redaction.integration/documentformatinstance/perform_binary_check_stream/) |  |
| [perform_binary_check_streams](/redaction/python-net/groupdocs.redaction.integration/documentformatinstance/perform_binary_check_streams/) |  |
| [save](/redaction/python-net/groupdocs.redaction.integration/documentformatinstance/save/#output) | Αποθηκεύει το έγγραφο σε μια ροή. |
| [save_stream](/redaction/python-net/groupdocs.redaction.integration/documentformatinstance/save_stream/) |  |
| [save_streams](/redaction/python-net/groupdocs.redaction.integration/documentformatinstance/save_streams/) |  |

### Ιδιότητες
| Ιδιότητα | Περιγραφή |
| :- | :- |
| [password](/redaction/python-net/groupdocs.redaction.integration/documentformatinstance/password/) | Ο κωδικός πρόσβασης για έγγραφα με προστασία κωδικού. |

### Παράδειγμα

```python
class DummyDocument(DocumentFormatInstance):
    def load(self, output: io.RawIOBase) -> None:
        # φόρτωση περιεχομένου αρχείου
        pass

    def save(self, output: io.RawIOBase) -> None:
        # αποθήκευση αλλαγών στο αρχείο
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

### Δείτε επίσης
* module [`groupdocs.redaction.integration`](/redaction/python-net/groupdocs.redaction.integration/)
