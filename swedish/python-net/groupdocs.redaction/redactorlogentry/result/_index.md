---
title: "result-egenskap"
second_title: "GroupDocs.Redaction för Python via .NET API-referenser"
description: "Resultatet som returneras av DocumentFormatInstance."
type: docs
url: /sv/python-net/groupdocs.redaction/redactorlogentry/result/
is_root: false
weight: 2020
---


## result property

Resultatet som returneras av [`DocumentFormatInstance`](/redaction/python-net/groupdocs.redaction.integration/documentformatinstance/).

Alla metadata-redigeringar tillämpas på varje metadata-objekt separat, och även om en metadata-redigering misslyckas, kommer resten av metadata-objekten att uppdateras. Du kan hitta en lista över misslyckade, överhoppade (avvisade) metadata-objekt och orsakerna till detta i `ErrorMessage`-egenskapen för [`RedactorLogEntry.Result`](/redaction/python-net/groupdocs.redaction/redactorlogentry/result/).

### Definition:
```python
@property
def result(self):
    ...
```

### Se även
* class [`RedactorLogEntry`](/redaction/python-net/groupdocs.redaction/redactorlogentry/)
