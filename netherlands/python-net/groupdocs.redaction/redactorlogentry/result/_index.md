---
title: "result-eigenschap"
second_title: "GroupDocs.Redaction voor Python via .NET API-referenties"
description: "Het resultaat geretourneerd door DocumentFormatInstance."
type: docs
url: /nl/python-net/groupdocs.redaction/redactorlogentry/result/
is_root: false
weight: 2020
---


## result property

Het resultaat geretourneerd door [`DocumentFormatInstance`](/redaction/python-net/groupdocs.redaction.integration/documentformatinstance/).

Alle metadata-redacties worden afzonderlijk op elk metadata-item toegepast, en zelfs als een metadata-itemredactie faalt, worden de overige metadata-items bijgewerkt. Je kunt een lijst met mislukte, overgeslagen (afgewezen) metadata-items en de redenen daarvoor vinden in de `ErrorMessage`-eigenschap van [`RedactorLogEntry.Result`](/redaction/python-net/groupdocs.redaction/redactorlogentry/result/).

### Definition:
```python
@property
def result(self):
    ...
```

### Zie ook
* class [`RedactorLogEntry`](/redaction/python-net/groupdocs.redaction/redactorlogentry/)
