---
title: "méthode rasterize"
second_title: "Références API de GroupDocs.Redaction pour Python via .NET"
description: "Enregistre le document dans un flux au format PDF."
type: docs
url: /fr/python-net/groupdocs.redaction.integration/irasterizabledocument/rasterize/
is_root: false
weight: 1010
---


## rasterize {#output}

Enregistre le document dans un flux au format PDF.

```python
def rasterize(self, output):
    ...
```

| Paramètre | Type | Description |
| :- | :- | :- |
| output | `io.RawIOBase` | Flux cible. |

## rasterize {#output-options}

Enregistre le document dans un flux au format PDF avec des options de plage de pages et de conformité.

```python
def rasterize(self, output, options):
    ...
```

| Paramètre | Type | Description |
| :- | :- | :- |
| output | `io.RawIOBase` | Flux cible. |
| options | `RasterizationOptions` | Options de conversion PDF. |

### Voir aussi
* class [`IRasterizableDocument`](/redaction/python-net/groupdocs.redaction.integration/irasterizabledocument/)
