---
title: "SaveOptions‑klasse"
second_title: "GroupDocs.Redaction voor Python via .NET API-referenties"
description: "Biedt opties om de naam van een uitvoerbestand te wijzigen en/of het document te converteren naar een op afbeeldingen gebaseerde PDF (rasterisatie)."
type: docs
url: /nl/python-net/groupdocs.redaction.options/saveoptions/
is_root: false
weight: 110
---


## SaveOptions class

Biedt opties om de naam van een uitvoerbestand te wijzigen en/of het document te converteren naar een op afbeeldingen gebaseerde PDF (rasterisatie).

Meer informatie:
- [Save with default options](https://docs.groupdocs.com/redaction/net/save-with-default-options/)
- [Save in rasterized PDF](https://docs.groupdocs.com/redaction/net/save-in-rasterized-pdf/)
- [Select specific pages for rasterized PDF](https://docs.groupdocs.com/redaction/net/select-specific-pages-for-rasterized-pdf/)
- [Save in original format](https://docs.groupdocs.com/redaction/net/save-in-original-format/)
- [Save overwriting original file](https://docs.groupdocs.com/redaction/net/save-overwriting-original-file/)
- [Save to stream](https://docs.groupdocs.com/redaction/net/save-to-stream/)

Het SaveOptions‑type bevat de volgende leden:

### Constructors
| Constructor | Beschrijving |
| :- | :- |
| [__init__](/redaction/python-net/groupdocs.redaction.options/saveoptions/__init__/) | Initialiseert een nieuw exemplaar met standaardinstellingen: rasterize_to_pdf is False en add_suffix is False. |
| [__init__](/redaction/python-net/groupdocs.redaction.options/saveoptions/__init__/#rasterize_to_pdf-suffix) | Initialiseert een nieuw exemplaar met opgegeven parameters. |

### Eigenschappen
| Eigenschap | Beschrijving |
| :- | :- |
| [add_suffix](/redaction/python-net/groupdocs.redaction.options/saveoptions/add_suffix/) | De add_suffix‑eigenschap geeft aan of de bestandsnaam moet worden gewijzigd vóór het opslaan. Standaard is False. |
| [rasterization](/redaction/python-net/groupdocs.redaction.options/saveoptions/rasterization/) | De rasterisatie‑instellingen. |
| [rasterize_to_pdf](/redaction/python-net/groupdocs.redaction.options/saveoptions/rasterize_to_pdf/) | De vlag die aangeeft of alle pagina's in het document worden geconverteerd naar afbeeldingen en samengevoegd tot één PDF‑bestand. |
| [redacted_file_suffix](/redaction/python-net/groupdocs.redaction.options/saveoptions/redacted_file_suffix/) | Het aangepaste achtervoegsel voor de uitvoerbestandsnaam. Indien niet gespecificeerd, wordt de [`SaveOptions.SaveSuffix`](/redaction/python-net/groupdocs.redaction.options/saveoptions/save_suffix/)‑constante gebruikt. |

### Velden
| Veld | Beschrijving |
| :- | :- |
| [SAVE_SUFFIX](/redaction/python-net/groupdocs.redaction.options/saveoptions/save_suffix/) | Stelt de standaardwaarde voor het achtervoegsel voor, namelijk "Redacted". |

### Voorbeeld

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.options import SaveOptions
from groupdocs.redaction.redactions import ExactPhraseRedaction, ReplacementOptions

def save_with_default_options():
    repl_opt = ReplacementOptions("[personal]")
    ex_red = ExactPhraseRedaction("John Doe", repl_opt)

    with Redactor("./sample.docx") as redactor:
        redactor.apply(ex_red)

        # Sla het document op met standaardopties (rasterize to PDF en voeg achtervoegsel toe)
        save_options = SaveOptions()
        save_options.add_suffix = True
        save_options.rasterize_to_pdf = True
        save_options.redacted_file_suffix = "redacted"

        result_path = redactor.save(save_options)
        print(f"Document redacted successfully. Check output in {result_path}.")
```

### Guides
Taakgidsen die `SaveOptions` gebruiken:

* [Hello, World!](/redaction/python-net/guides/hello-world/)
* [Redaction basics](/redaction/python-net/guides/redaction-basics/)
* [Text redaction](/redaction/python-net/guides/text-redactions/)
* [Image redactions](/redaction/python-net/guides/image-redactions/)
* [Metadata redactions](/redaction/python-net/guides/metadata-redactions/)
* [Annotation redactions](/redaction/python-net/guides/annotation-redactions/)
* [Spreadsheet redactions](/redaction/python-net/guides/spreadsheet-redactions/)
* [Remove page redactions](/redaction/python-net/guides/remove-page-redactions/)
* [Use redaction policies](/redaction/python-net/guides/use-redaction-policies/)

### Zie ook
* module [`groupdocs.redaction.options`](/redaction/python-net/groupdocs.redaction.options/)
