---
title: "méthode save"
second_title: "Références API de GroupDocs.Redaction pour Python via .NET"
description: "Enregistre la politique de rédaction dans un fichier."
type: docs
url: /fr/python-net/groupdocs.redaction/redactionpolicy/save/
is_root: false
weight: 1060
---


## save {#file_path}

Enregistre la politique de rédaction dans un fichier.

```python
def save(self, file_path):
    ...
```

| Paramètre | Type | Description |
| :- | :- | :- |
| file_path | `str` | Chemin du fichier. |

### Exemple

```python
    policy = RedactionPolicy([
        ExactPhraseRedaction("ACME", ReplacementOptions("[CO]")),
        RegexRedaction(r"\d{2,}", ReplacementOptions("[NUM]")),
    ])
    policy.save("./sample_policy.xml")
    ```

## save {#output}

Enregistre la politique de rédaction dans un flux.

```python
def save(self, output):
    ...
```

| Paramètre | Type | Description |
| :- | :- | :- |
| output | `io.RawIOBase` | Flux cible pour enregistrer la politique. |

**Returns:** None.

### Voir aussi
* class [`RedactionPolicy`](/redaction/python-net/groupdocs.redaction/redactionpolicy/)
