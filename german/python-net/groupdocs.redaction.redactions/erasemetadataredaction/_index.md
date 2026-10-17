---
title: "EraseMetadataRedaction Klasse"
second_title: "GroupDocs.Redaction für Python über .NET API-Referenzen"
description: "Stellt eine Metadaten-Redaktion dar, die alle Metadaten oder Metadaten, die bestimmten MetadataFilters entsprechen, aus dem Dokument entfernt."
type: docs
url: /de/python-net/groupdocs.redaction.redactions/erasemetadataredaction/
is_root: false
weight: 70
---


## EraseMetadataRedaction class

Stellt eine Metadaten-Redaktion dar, die alle Metadaten oder Metadaten, die bestimmten MetadataFilters entsprechen, aus dem Dokument entfernt.

- More details about applying redactions: https://docs.groupdocs.com/redaction/net/redaction-basics/
- More details about document metadata redactions: https://docs.groupdocs.com/redaction/net/metadata-redactions/

Der Typ EraseMetadataRedaction stellt die folgenden Mitglieder bereit:

### Konstruktoren
| Konstruktor | Beschreibung |
| :- | :- |
| [__init__](/redaction/python-net/groupdocs.redaction.redactions/erasemetadataredaction/__init__/) | Initialisiert eine neue Instanz der EraseMetadataRedaction Klasse und löscht alle Metadaten. |
| [__init__](/redaction/python-net/groupdocs.redaction.redactions/erasemetadataredaction/__init__/#filter) | Initialisiert eine neue Instanz von EraseMetadataRedaction und löscht Metadaten, die den angegebenen `MetadataFilters` entsprechen. |

### Methoden
| Methode | Beschreibung |
| :- | :- |
| [apply_to](/redaction/python-net/groupdocs.redaction.redactions/metadataredaction/apply_to/) | Wendet die Redaktion auf eine gegebene Formatinstanz an. (geerbt von [`MetadataRedaction`](/redaction/python-net/groupdocs.redaction.redactions/metadataredaction/)) |
| [apply_to_document_format_instance](/redaction/python-net/groupdocs.redaction.redactions/metadataredaction/apply_to_document_format_instance/) | (geerbt von [`MetadataRedaction`](/redaction/python-net/groupdocs.redaction.redactions/metadataredaction/)) |

### Eigenschaften
| Eigenschaft | Beschreibung |
| :- | :- |
| [description](/redaction/python-net/groupdocs.redaction.redactions/erasemetadataredaction/description/) | Die Beschreibung der Redaktion und ihrer Parameter. |
| [filter](/redaction/python-net/groupdocs.redaction.redactions/metadataredaction/filter/) | Der Filter, der verwendet wird, um alle oder bestimmte Metadaten auszuwählen, wie z. B. Autor oder Unternehmen. (geerbt von [`MetadataRedaction`](/redaction/python-net/groupdocs.redaction.redactions/metadataredaction/)) |

### Beispiel

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.redactions import EraseMetadataRedaction, MetadataFilters

with Redactor("document.docx") as redactor:
    # Alle Metadaten löschen
    redactor.apply(EraseMetadataRedaction(MetadataFilters.ALL))
    # Nur das Autorenfeld löschen
    redactor.apply(EraseMetadataRedaction(MetadataFilters.AUTHOR))
    redactor.save()
```

### Guides
Aufgabenleitfäden, die `EraseMetadataRedaction` verwenden:

* [Redaction basics](/redaction/python-net/guides/redaction-basics/)
* [Image redactions](/redaction/python-net/guides/image-redactions/)
* [Metadata redactions](/redaction/python-net/guides/metadata-redactions/)
* [Use redaction policies](/redaction/python-net/guides/use-redaction-policies/)

### Siehe auch
* module [`groupdocs.redaction.redactions`](/redaction/python-net/groupdocs.redaction.redactions/)
