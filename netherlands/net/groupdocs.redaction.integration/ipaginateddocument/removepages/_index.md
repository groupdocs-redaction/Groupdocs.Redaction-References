---
title: RemovePages
second_title: GroupDocs.Redaction voor .NET API-referentie
description: Verwijdert een of meerdere paginas afhankelijk van de startpositie offset en aantal.
type: docs
weight: 10
url: /nl/net/groupdocs.redaction.integration/ipaginateddocument/removepages/
---
## IPaginatedDocument.RemovePages method

Verwijdert een of meerdere pagina's, afhankelijk van de startpositie, offset en aantal.

```csharp
public RedactionResult RemovePages(PageSeekOrigin origin, int index, int count)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| origin | PageSeekOrigin | Zoek oorsprongspositie, het begin of het einde van het document |
| index | Int32 | Startpositie-index (0-gebaseerd) |
| count | Int32 | Aantal te verwijderen pagina's |

### Winstwaarde

Redactieresultaat van verwijdering van pagina's

### Zie ook

* class [RedactionResult](../../../groupdocs.redaction/redactionresult)
* enum [PageSeekOrigin](../../../groupdocs.redaction.redactions/pageseekorigin)
* interface [IPaginatedDocument](../../ipaginateddocument)
* naamruimte [GroupDocs.Redaction.Integration](../../ipaginateddocument)
* montage [GroupDocs.Redaction](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Redaction.dll -->