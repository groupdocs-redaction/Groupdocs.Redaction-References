---
title: "proprietà result"
second_title: "Riferimenti API di GroupDocs.Redaction per Python tramite .NET"
description: "Il risultato restituito da DocumentFormatInstance."
type: docs
url: /it/python-net/groupdocs.redaction/redactorlogentry/result/
is_root: false
weight: 2020
---


## result property

Il risultato restituito da [`DocumentFormatInstance`](/redaction/python-net/groupdocs.redaction.integration/documentformatinstance/).

Tutte le redazioni dei metadati si applicano a ciascun elemento di metadati separatamente, e anche se la redazione di un elemento di metadati fallisce, gli altri elementi di metadati verranno aggiornati. È possibile trovare un elenco di elementi di metadati falliti, saltati (rifiutati) e le relative ragioni nella proprietà `ErrorMessage` di [`RedactorLogEntry.Result`](/redaction/python-net/groupdocs.redaction/redactorlogentry/result/).

### Definition:
```python
@property
def result(self):
    ...
```

### Vedi anche
* class [`RedactorLogEntry`](/redaction/python-net/groupdocs.redaction/redactorlogentry/)
