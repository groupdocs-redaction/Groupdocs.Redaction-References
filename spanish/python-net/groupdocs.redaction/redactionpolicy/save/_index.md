---
title: "método save"
second_title: "Referencias de API de GroupDocs.Redaction para Python a través de .NET"
description: "Guarda la política de redacción en un archivo."
type: docs
url: /es/python-net/groupdocs.redaction/redactionpolicy/save/
is_root: false
weight: 1060
---


## save {#file_path}

Guarda la política de redacción en un archivo.

```python
def save(self, file_path):
    ...
```

| Parámetro | Tipo | Descripción |
| :- | :- | :- |
| file_path | `str` | Ruta al archivo. |

### Ejemplo

```python
    policy = RedactionPolicy([
        ExactPhraseRedaction("ACME", ReplacementOptions("[CO]")),
        RegexRedaction(r"\d{2,}", ReplacementOptions("[NUM]")),
    ])
    policy.save("./sample_policy.xml")
    ```

## save {#output}

Guarda la política de redacción en un flujo.

```python
def save(self, output):
    ...
```

| Parámetro | Tipo | Descripción |
| :- | :- | :- |
| output | `io.RawIOBase` | Secuencia de destino para guardar la política. |

**Returns:** None.

### Ver también
* class [`RedactionPolicy`](/redaction/python-net/groupdocs.redaction/redactionpolicy/)
