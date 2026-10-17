---
title: "propriété result"
second_title: "Références API de GroupDocs.Redaction pour Python via .NET"
description: "Le résultat renvoyé par DocumentFormatInstance."
type: docs
url: /fr/python-net/groupdocs.redaction/redactorlogentry/result/
is_root: false
weight: 2020
---


## result property

Le résultat retourné par [`DocumentFormatInstance`](/redaction/python-net/groupdocs.redaction.integration/documentformatinstance/).

Toutes les redactions de métadonnées s'appliquent à chaque élément de métadonnée séparément, et même si la redaction d'un élément de métadonnée échoue, le reste des éléments de métadonnées sera mis à jour. Vous pouvez trouver une liste des éléments de métadonnées échoués, ignorés (rejetés) et les raisons correspondantes dans la propriété `ErrorMessage` de [`RedactorLogEntry.Result`](/redaction/python-net/groupdocs.redaction/redactorlogentry/result/).

### Definition:
```python
@property
def result(self):
    ...
```

### Voir aussi
* class [`RedactorLogEntry`](/redaction/python-net/groupdocs.redaction/redactorlogentry/)
