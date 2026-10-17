---
title: "result Eigenschaft"
second_title: "GroupDocs.Redaction für Python über .NET API-Referenzen"
description: "Das Ergebnis, das von DocumentFormatInstance zurückgegeben wird."
type: docs
url: /de/python-net/groupdocs.redaction/redactorlogentry/result/
is_root: false
weight: 2020
---


## result property

Das Ergebnis, das von [`DocumentFormatInstance`](/redaction/python-net/groupdocs.redaction.integration/documentformatinstance/) zurückgegeben wird.

Alle Metadaten-Redaktionen gelten für jedes Metadaten-Element einzeln, und selbst wenn eine Metadaten-Element-Redaktion fehlschlägt, werden die restlichen Metadaten-Elemente aktualisiert. Sie können eine Liste fehlgeschlagener, übersprungener (abgelehnter) Metadaten-Elemente und deren Gründe in der `ErrorMessage` Eigenschaft von [`RedactorLogEntry.Result`](/redaction/python-net/groupdocs.redaction/redactorlogentry/result/) finden.

### Definition:
```python
@property
def result(self):
    ...
```

### Siehe auch
* class [`RedactorLogEntry`](/redaction/python-net/groupdocs.redaction/redactorlogentry/)
