---
title: "propiedad result"
second_title: "Referencias de API de GroupDocs.Redaction para Python a través de .NET"
description: "El resultado devuelto por DocumentFormatInstance."
type: docs
url: /es/python-net/groupdocs.redaction/redactorlogentry/result/
is_root: false
weight: 2020
---


## result property

El resultado devuelto por [`DocumentFormatInstance`](/redaction/python-net/groupdocs.redaction.integration/documentformatinstance/).

Todas las redacciones de metadatos se aplican a cada elemento de metadatos por separado, y aunque una redacción de un elemento de metadato falle, el resto de los elementos de metadatos se actualizará. Puedes encontrar una lista de elementos de metadatos fallidos, omitidos (rechazados) y sus razones en la propiedad `ErrorMessage` de [`RedactorLogEntry.Result`](/redaction/python-net/groupdocs.redaction/redactorlogentry/result/).

### Definition:
```python
@property
def result(self):
    ...
```

### Ver también
* class [`RedactorLogEntry`](/redaction/python-net/groupdocs.redaction/redactorlogentry/)
