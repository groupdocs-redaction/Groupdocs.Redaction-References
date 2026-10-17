---
title: "SaveOptions‑Klasse"
second_title: "GroupDocs.Redaction für Python über .NET API-Referenzen"
description: "Stellt Optionen zum Ändern eines Ausgabedateinamens und/oder zum Konvertieren des Dokuments in ein bildbasiertes PDF (Rasterisierung) bereit."
type: docs
url: /de/python-net/groupdocs.redaction.options/saveoptions/
is_root: false
weight: 110
---


## SaveOptions class

Stellt Optionen zum Ändern eines Ausgabedateinamens und/oder zum Konvertieren des Dokuments in ein bildbasiertes PDF (Rasterisierung) bereit.

Mehr erfahren:
- [Save with default options](https://docs.groupdocs.com/redaction/net/save-with-default-options/)
- [Save in rasterized PDF](https://docs.groupdocs.com/redaction/net/save-in-rasterized-pdf/)
- [Select specific pages for rasterized PDF](https://docs.groupdocs.com/redaction/net/select-specific-pages-for-rasterized-pdf/)
- [Save in original format](https://docs.groupdocs.com/redaction/net/save-in-original-format/)
- [Save overwriting original file](https://docs.groupdocs.com/redaction/net/save-overwriting-original-file/)
- [Save to stream](https://docs.groupdocs.com/redaction/net/save-to-stream/)

Der SaveOptions‑Typ stellt die folgenden Mitglieder bereit:

### Konstruktoren
| Konstruktor | Beschreibung |
| :- | :- |
| [__init__](/redaction/python-net/groupdocs.redaction.options/saveoptions/__init__/) | Initialisiert eine neue Instanz mit Standardeinstellungen: rasterize_to_pdf ist False und add_suffix ist False. |
| [__init__](/redaction/python-net/groupdocs.redaction.options/saveoptions/__init__/#rasterize_to_pdf-suffix) | Initialisiert eine neue Instanz mit angegebenen Parametern. |

### Eigenschaften
| Eigenschaft | Beschreibung |
| :- | :- |
| [add_suffix](/redaction/python-net/groupdocs.redaction.options/saveoptions/add_suffix/) | Die Eigenschaft add_suffix gibt an, ob der Dateiname vor dem Speichern geändert werden soll. Standardwert ist False. |
| [rasterization](/redaction/python-net/groupdocs.redaction.options/saveoptions/rasterization/) | Die Rasterisierungseinstellungen. |
| [rasterize_to_pdf](/redaction/python-net/groupdocs.redaction.options/saveoptions/rasterize_to_pdf/) | Das Flag, das angibt, ob alle Seiten im Dokument in Bilder konvertiert und zu einer einzigen PDF‑Datei zusammengeführt werden. |
| [redacted_file_suffix](/redaction/python-net/groupdocs.redaction.options/saveoptions/redacted_file_suffix/) | Der benutzerdefinierte Suffix für den Ausgabedateinamen. Wenn nicht angegeben, wird die Konstante [`SaveOptions.SaveSuffix`](/redaction/python-net/groupdocs.redaction.options/saveoptions/save_suffix/) verwendet. |

### Felder
| Feld | Beschreibung |
| :- | :- |
| [SAVE_SUFFIX](/redaction/python-net/groupdocs.redaction.options/saveoptions/save_suffix/) | Stellt den Standard‑Suffixwert dar, der "Redacted" ist. |

### Beispiel

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.options import SaveOptions
from groupdocs.redaction.redactions import ExactPhraseRedaction, ReplacementOptions

def save_with_default_options():
    repl_opt = ReplacementOptions("[personal]")
    ex_red = ExactPhraseRedaction("John Doe", repl_opt)

    with Redactor("./sample.docx") as redactor:
        redactor.apply(ex_red)

        # Speichere das Dokument mit den Standardoptionen (Rasterisierung zu PDF und Suffix hinzufügen)
        save_options = SaveOptions()
        save_options.add_suffix = True
        save_options.rasterize_to_pdf = True
        save_options.redacted_file_suffix = "redacted"

        result_path = redactor.save(save_options)
        print(f"Document redacted successfully. Check output in {result_path}.")
```

### Guides
Aufgabenleitfäden, die `SaveOptions` verwenden:

* [Hello, World!](/redaction/python-net/guides/hello-world/)
* [Redaction basics](/redaction/python-net/guides/redaction-basics/)
* [Text redaction](/redaction/python-net/guides/text-redactions/)
* [Image redactions](/redaction/python-net/guides/image-redactions/)
* [Metadata redactions](/redaction/python-net/guides/metadata-redactions/)
* [Annotation redactions](/redaction/python-net/guides/annotation-redactions/)
* [Spreadsheet redactions](/redaction/python-net/guides/spreadsheet-redactions/)
* [Remove page redactions](/redaction/python-net/guides/remove-page-redactions/)
* [Use redaction policies](/redaction/python-net/guides/use-redaction-policies/)

### Siehe auch
* module [`groupdocs.redaction.options`](/redaction/python-net/groupdocs.redaction.options/)
