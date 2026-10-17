---
title: "Classe Redactor"
second_title: "Références API de GroupDocs.Redaction pour Python via .NET"
description: "Représente la classe principale qui contrôle le processus de censure de documents, permettant d'ouvrir, de censurer et d'enregistrer les documents."
type: docs
url: /fr/python-net/groupdocs.redaction/redactor/
is_root: false
weight: 150
---


## Redactor class

Représente la classe principale qui contrôle le processus de censure de documents, permettant d'ouvrir, de censurer et d'enregistrer les documents.

En savoir plus
- More details about applying redactions: https://docs.groupdocs.com/redaction/net/redaction-basics/
- More advanced redaction topics: https://docs.groupdocs.com/redaction/net/advanced-usage/

Le type Redactor expose les membres suivants:

### Constructeurs
| Constructeur | Description |
| :- | :- |
| [__init__](/redaction/python-net/groupdocs.redaction/redactor/__init__/#file_path) | Initialise une nouvelle instance de Redactor en utilisant un chemin de fichier. |
| [__init__](/redaction/python-net/groupdocs.redaction/redactor/__init__/#document) | Initialise une nouvelle instance de [`Redactor`](/redaction/python-net/groupdocs.redaction/redactor/) en utilisant un flux. |
| [__init__](/redaction/python-net/groupdocs.redaction/redactor/__init__/#file_path-load_options) | Initialise une nouvelle instance de [`Redactor`](/redaction/python-net/groupdocs.redaction/redactor/) pour un document protégé par mot de passe en utilisant son chemin. |
| [__init__](/redaction/python-net/groupdocs.redaction/redactor/__init__/#file_path-load_options-settings) | Initialise une nouvelle instance de Redactor pour un document protégé par mot de passe en utilisant son chemin et ses paramètres. |
| [__init__](/redaction/python-net/groupdocs.redaction/redactor/__init__/#document-load_options) | Initialise une nouvelle instance de Redactor pour un document protégé par mot de passe en utilisant un flux. |
| [__init__](/redaction/python-net/groupdocs.redaction/redactor/__init__/#document-load_options-settings) | Initialise une nouvelle instance de [`Redactor`](/redaction/python-net/groupdocs.redaction/redactor/) pour un document protégé par mot de passe en utilisant un flux et des paramètres. |

### Méthodes
| Méthode | Description |
| :- | :- |
| [apply](/redaction/python-net/groupdocs.redaction/redactor/apply/#redaction) | Applique une rédaction au document. |
| [apply](/redaction/python-net/groupdocs.redaction/redactor/apply/#redactions) | Applique un ensemble de rédactions au document. |
| [apply](/redaction/python-net/groupdocs.redaction/redactor/apply/#policy) | Applique une politique de rédaction au document. |
| [apply_redaction](/redaction/python-net/groupdocs.redaction/redactor/apply_redaction/) |  |
| [apply_redaction_policy](/redaction/python-net/groupdocs.redaction/redactor/apply_redaction_policy/) |  |
| [dispose](/redaction/python-net/groupdocs.redaction/redactor/dispose/) | Libère les ressources. |
| [generate_preview](/redaction/python-net/groupdocs.redaction/redactor/generate_preview/#preview_options) | Génère des images d’aperçu de pages spécifiques dans un format d’image donné. |
| [generate_preview_preview_options](/redaction/python-net/groupdocs.redaction/redactor/generate_preview_preview_options/) |  |
| [get_document_info](/redaction/python-net/groupdocs.redaction/redactor/get_document_info/) | Récupère les informations générales sur le document, telles que la taille et le nombre de pages. |
| [save](/redaction/python-net/groupdocs.redaction/redactor/save/) | Enregistre le document dans un fichier avec les options suivantes : AddSuffix = True, RasterizeToPDF = True. |
| [save](/redaction/python-net/groupdocs.redaction/redactor/save/#save_options) | Enregistre le document dans un fichier. |
| [save](/redaction/python-net/groupdocs.redaction/redactor/save/#document-rasterization_options) | Enregistre le document dans un flux, y compris l'emplacement personnalisé. |
| [save_save_options](/redaction/python-net/groupdocs.redaction/redactor/save_save_options/) |  |
| [save_stream](/redaction/python-net/groupdocs.redaction/redactor/save_stream/) |  |
| [save_streams](/redaction/python-net/groupdocs.redaction/redactor/save_streams/) |  |

### Exemple

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.redactions import RemovePageRedaction, PageSeekOrigin

# Ouvrez un document et supprimez la première page
with Redactor("document.pdf") as redactor:
    redactor.apply(RemovePageRedaction(PageSeekOrigin.BEGIN, 0, 1))
    redactor.save()
```

### Guides
Guides de tâches qui utilisent `Redactor` :

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

### Voir aussi
* module [`groupdocs.redaction`](/redaction/python-net/groupdocs.redaction/)
