---
title: "metodo save"
second_title: "Riferimenti API di GroupDocs.Redaction per Python tramite .NET"
description: "Salva la politica di redazione su un file."
type: docs
url: /it/python-net/groupdocs.redaction/redactionpolicy/save/
is_root: false
weight: 1060
---


## save {#file_path}

Salva la politica di redazione su un file.

```python
def save(self, file_path):
    ...
```

| Parametro | Tipo | Descrizione |
| :- | :- | :- |
| file_path | `str` | Percorso del file. |

### Esempio

```python
    policy = RedactionPolicy([
        ExactPhraseRedaction("ACME", ReplacementOptions("[CO]")),
        RegexRedaction(r"\d{2,}", ReplacementOptions("[NUM]")),
    ])
    policy.save("./sample_policy.xml")
    ```

## save {#output}

Salva la politica di redazione su uno stream.

```python
def save(self, output):
    ...
```

| Parametro | Tipo | Descrizione |
| :- | :- | :- |
| output | `io.RawIOBase` | Stream di destinazione per salvare la policy. |

**Returns:** None.

### Vedi anche
* class [`RedactionPolicy`](/redaction/python-net/groupdocs.redaction/redactionpolicy/)
