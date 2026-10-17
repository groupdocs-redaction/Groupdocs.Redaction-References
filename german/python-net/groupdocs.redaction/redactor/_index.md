---
title: "Redactor-Klasse"
second_title: "GroupDocs.Redaction für Python über .NET API-Referenzen"
description: "Stellt eine Hauptklasse dar, die den Dokumenten‑Redaktionsprozess steuert und das Öffnen, Redigieren und Speichern von Dokumenten ermöglicht."
type: docs
url: /de/python-net/groupdocs.redaction/redactor/
is_root: false
weight: 150
---


## Redactor class

Stellt eine Hauptklasse dar, die den Dokumenten‑Redaktionsprozess steuert und das Öffnen, Redigieren und Speichern von Dokumenten ermöglicht.

Mehr erfahren
- More details about applying redactions: https://docs.groupdocs.com/redaction/net/redaction-basics/
- More advanced redaction topics: https://docs.groupdocs.com/redaction/net/advanced-usage/

Der Redactor-Typ stellt die folgenden Mitglieder bereit:

### Konstruktoren
| Konstruktor | Beschreibung |
| :- | :- |
| [__init__](/redaction/python-net/groupdocs.redaction/redactor/__init__/#file_path) | Initialisiert eine neue Redactor-Instanz mittels eines Dateipfads. |
| [__init__](/redaction/python-net/groupdocs.redaction/redactor/__init__/#document) | Initialisiert eine neue Instanz von [`Redactor`](/redaction/python-net/groupdocs.redaction/redactor/) mittels eines Streams. |
| [__init__](/redaction/python-net/groupdocs.redaction/redactor/__init__/#file_path-load_options) | Initialisiert eine neue Instanz von [`Redactor`](/redaction/python-net/groupdocs.redaction/redactor/) für ein passwortgeschütztes Dokument mittels seines Pfads. |
| [__init__](/redaction/python-net/groupdocs.redaction/redactor/__init__/#file_path-load_options-settings) | Initialisiert eine neue Redactor-Instanz für ein passwortgeschütztes Dokument mittels seines Pfads und seiner Einstellungen. |
| [__init__](/redaction/python-net/groupdocs.redaction/redactor/__init__/#document-load_options) | Initialisiert eine neue Redactor-Instanz für ein passwortgeschütztes Dokument mittels eines Streams. |
| [__init__](/redaction/python-net/groupdocs.redaction/redactor/__init__/#document-load_options-settings) | Initialisiert eine neue Instanz von [`Redactor`](/redaction/python-net/groupdocs.redaction/redactor/) für ein passwortgeschütztes Dokument mittels eines Streams und Einstellungen. |

### Methoden
| Methode | Beschreibung |
| :- | :- |
| [apply](/redaction/python-net/groupdocs.redaction/redactor/apply/#redaction) | Wendet eine Redaktion auf das Dokument an. |
| [apply](/redaction/python-net/groupdocs.redaction/redactor/apply/#redactions) | Wendet eine Menge von Redaktionen auf das Dokument an. |
| [apply](/redaction/python-net/groupdocs.redaction/redactor/apply/#policy) | Wendet eine Redaktionsrichtlinie auf das Dokument an. |
| [apply_redaction](/redaction/python-net/groupdocs.redaction/redactor/apply_redaction/) |  |
| [apply_redaction_policy](/redaction/python-net/groupdocs.redaction/redactor/apply_redaction_policy/) |  |
| [dispose](/redaction/python-net/groupdocs.redaction/redactor/dispose/) | Gibt Ressourcen frei. |
| [generate_preview](/redaction/python-net/groupdocs.redaction/redactor/generate_preview/#preview_options) | Erzeugt Vorschaubilder bestimmter Seiten in einem angegebenen Bildformat. |
| [generate_preview_preview_options](/redaction/python-net/groupdocs.redaction/redactor/generate_preview_preview_options/) |  |
| [get_document_info](/redaction/python-net/groupdocs.redaction/redactor/get_document_info/) | Ruft die allgemeinen Informationen über das Dokument ab, wie Größe und Seitenanzahl. |
| [save](/redaction/python-net/groupdocs.redaction/redactor/save/) | Speichert das Dokument in einer Datei mit den folgenden Optionen: AddSuffix = True, RasterizeToPDF = True. |
| [save](/redaction/python-net/groupdocs.redaction/redactor/save/#save_options) | Speichert das Dokument in einer Datei. |
| [save](/redaction/python-net/groupdocs.redaction/redactor/save/#document-rasterization_options) | Speichert das Dokument in einen Stream, einschließlich benutzerdefiniertem Speicherort. |
| [save_save_options](/redaction/python-net/groupdocs.redaction/redactor/save_save_options/) |  |
| [save_stream](/redaction/python-net/groupdocs.redaction/redactor/save_stream/) |  |
| [save_streams](/redaction/python-net/groupdocs.redaction/redactor/save_streams/) |  |

### Beispiel

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.redactions import RemovePageRedaction, PageSeekOrigin

# Öffnet ein Dokument und entfernt die erste Seite
with Redactor("document.pdf") as redactor:
    redactor.apply(RemovePageRedaction(PageSeekOrigin.BEGIN, 0, 1))
    redactor.save()
```

### Guides
Aufgabenleitfäden, die `Redactor` verwenden:

* [Hello, World!](/redaction/python-net/guides/hello-world/)
* [Redaction basics](/redaction/python-net/guides/redaction-basics/)
* [Text redaction](/redaction/python-net/guides/text-redactions/)
* [Image redactions](/redaction/python-net/guides/image-redactions/)
* [Metadata redactions](/redaction/python-net/guides/metadata-redactions/)
* [Annotation redactions](/redaction/python-net/guides/annotation-redactions/)
* [Spreadsheet redactions](/redaction/python-net/guides/spreadsheet-redactions/)
* [Remove page redactions](/redaction/python-net/guides/remove-page-redactions/)
* [Use redaction policies](/redaction/python-net/guides/use-redaction-policies/)
* [Get file info](/redaction/python-net/guides/get-file-info/)

### Siehe auch
* module [`groupdocs.redaction`](/redaction/python-net/groupdocs.redaction/)
