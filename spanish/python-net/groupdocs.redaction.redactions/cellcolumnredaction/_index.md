---
title: "Clase CellColumnRedaction"
second_title: "Referencias de API de GroupDocs.Redaction para Python a través de .NET"
description: "Representa una redacción de texto que reemplaza el texto en un documento de hoja de cálculo (CSV, Excel, etc.)."
type: docs
url: /es/python-net/groupdocs.redaction.redactions/cellcolumnredaction/
is_root: false
weight: 20
---


## CellColumnRedaction class

Representa una redacción de texto que reemplaza el texto en un documento de hoja de cálculo (CSV, Excel, etc.).

- Learn more: https://docs.groupdocs.com/redaction/net/redaction-basics/
- More details about spreadsheet redactions: https://docs.groupdocs.com/redaction/net/spreadsheet-redactions/

El tipo CellColumnRedaction expone los siguientes miembros:

### Constructores
| Constructor | Descripción |
| :- | :- |
| [__init__](/redaction/python-net/groupdocs.redaction.redactions/cellcolumnredaction/__init__/#filter-reg_ex-options) | Inicializa una nueva CellColumnRedaction. |

### Métodos
| Método | Descripción |
| :- | :- |
| [apply_to](/redaction/python-net/groupdocs.redaction.redactions/cellcolumnredaction/apply_to/#format_instance) | Aplica la redacción a una instancia de formato dada. |
| [apply_to_document_format_instance](/redaction/python-net/groupdocs.redaction.redactions/cellcolumnredaction/apply_to_document_format_instance/) |  |

### Propiedades
| Propiedad | Descripción |
| :- | :- |
| [description](/redaction/python-net/groupdocs.redaction.redactions/cellcolumnredaction/description/) | La descripción de la redacción, que contiene su nombre y parámetros. |
| [filter](/redaction/python-net/groupdocs.redaction.redactions/cellcolumnredaction/filter/) | El filtro de columna y hoja de cálculo. |
| [pattern](/redaction/python-net/groupdocs.redaction.redactions/cellcolumnredaction/pattern/) | El patrón de expresión regular para coincidir. |
| [action_options](/redaction/python-net/groupdocs.redaction.redactions/textredaction/action_options/) | La instancia [`ReplacementOptions`](/redaction/python-net/groupdocs.redaction.redactions/replacementoptions/) que especifica el tipo de reemplazo de texto. (heredada de [`TextRedaction`](/redaction/python-net/groupdocs.redaction.redactions/textredaction/)) |
| [ocr_connector](/redaction/python-net/groupdocs.redaction.redactions/textredaction/ocr_connector/) | La implementación IOcrConnector usada para extraer texto del contenido gráfico. (heredada de [`TextRedaction`](/redaction/python-net/groupdocs.redaction.redactions/textredaction/)) |

### Ejemplo

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.redactions import CellColumnRedaction, ReplacementOptions
from groupdocs.redaction.filters import CellFilter

with Redactor("Sales in September.xlsx") as redactor:
    filter = CellFilter(column_index=1, worksheet_name="Customers")
    regex = r"^\w+([-+.']\w+)*@\w+([-.]\w+)*\.\w+([-.]\w+)*$"
    redactor.apply(CellColumnRedaction(filter, regex, ReplacementOptions("[customer email]")))
    redactor.save()
```

### Ver también
* module [`groupdocs.redaction.redactions`](/redaction/python-net/groupdocs.redaction.redactions/)
