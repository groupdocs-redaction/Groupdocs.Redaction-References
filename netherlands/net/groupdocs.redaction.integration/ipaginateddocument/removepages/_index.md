---
title: "RemovePages"
second_title: "GroupDocs.Redaction voor .NET API-referentie"
description: "Verwijdert één of meerdere pagina's afhankelijk van de offset van de startpositie en het aantal."
type: docs
weight: 10
url: /nl/net/groupdocs.redaction.integration/ipaginateddocument/removepages/
---
## IPaginatedDocument.RemovePages method

Verwijdert één of meerdere pagina's afhankelijk van de startpositie, offset en aantal.

```csharp
public RedactionResult RemovePages(PageSeekOrigin origin, int index, int count)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| herkomst | PageSeekOrigin | Zoek de herkomstpositie, het begin of het einde van het document |
| index | Int32 | Startpositie-index (0-gebaseerd) |
| aantal | Int32 | Aantal te verwijderen pagina's |

### Retourwaarde

Resultaat van het verwijderen van pagina's

### Zie ook

* class [RedactionResult](../../../groupdocs.redaction/redactionresult)
* enum [PageSeekOrigin](../../../groupdocs.redaction.redactions/pageseekorigin)
* interface [IPaginatedDocument](../../ipaginateddocument)
* namespace [GroupDocs.Redaction.Integration](../../../groupdocs.redaction.integration)
* assembly [GroupDocs.Redaction](../../../)

<!-- NIET BEWERKEN: gegenereerd door xmldocmd voor GroupDocs.Redaction.dll -->
