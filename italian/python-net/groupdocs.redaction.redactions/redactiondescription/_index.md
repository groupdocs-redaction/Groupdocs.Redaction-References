---
title: "Classe RedactionDescription"
second_title: "Riferimenti API di GroupDocs.Redaction per Python tramite .NET"
description: "Rappresenta le informazioni di una singola azione di modifica eseguita durante il processo di redazione."
type: docs
url: /it/python-net/groupdocs.redaction.redactions/redactiondescription/
is_root: false
weight: 200
---


## RedactionDescription class

Rappresenta le informazioni di una singola azione di modifica eseguita durante il processo di redazione.

Per saperne di più

- More details about [`RedactionDescription`](/redaction/python-net/groupdocs.redaction.redactions/redactiondescription/) class and [`IRedactionCallback`](/redaction/python-net/groupdocs.redaction.redactions/iredactioncallback/) interface: Use redaction callback https://docs.groupdocs.com/redaction/net/use-redaction-callback/

Il tipo RedactionDescription espone i seguenti membri:

### Costruttori
| Costruttore | Descrizione |
| :- | :- |
| [__init__](/redaction/python-net/groupdocs.redaction.redactions/redactiondescription/__init__/#redaction_type-action_type-original_text) | Inizializza una nuova istanza della classe RedactionDescription senza informazioni di sostituzione. |
| [__init__](/redaction/python-net/groupdocs.redaction.redactions/redactiondescription/__init__/#redaction_type-action_type-original_text-replacement) | Inizializza una nuova istanza della classe RedactionDescription con informazioni di sostituzione. |
| [__init__](/redaction/python-net/groupdocs.redaction.redactions/redactiondescription/__init__/#redaction_type-action_type-image_area_replacement-image_details) | Inizializza un nuovo RedactionDescription con informazioni di sostituzione dell'area immagine. |

### Proprietà
| Proprietà | Descrizione |
| :- | :- |
| [action_type](/redaction/python-net/groupdocs.redaction.redactions/redactiondescription/action_type/) | L'operazione di redazione: sostituzione, pulizia o eliminazione. |
| [details](/redaction/python-net/groupdocs.redaction.redactions/redactiondescription/details/) | Le informazioni opzionali sui dettagli dell'elemento redatto. |
| [image_area_replacement](/redaction/python-net/groupdocs.redaction.redactions/redactiondescription/image_area_replacement/) | Le informazioni di sostituzione per le redazioni dell'area immagine, o None per le redazioni testuali. |
| [original_text](/redaction/python-net/groupdocs.redaction.redactions/redactiondescription/original_text/) | Il testo corrispondente, se è fornita un'espressione. |
| [redaction_type](/redaction/python-net/groupdocs.redaction.redactions/redactiondescription/redaction_type/) | Il tipo di dati del documento – testo, metadati o annotazioni. |
| [replacement](/redaction/python-net/groupdocs.redaction.redactions/redactiondescription/replacement/) | Le informazioni di sostituzione, possono essere None. |

### Vedi anche
* module [`groupdocs.redaction.redactions`](/redaction/python-net/groupdocs.redaction.redactions/)
