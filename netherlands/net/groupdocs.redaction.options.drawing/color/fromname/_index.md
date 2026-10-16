---
title: "FromName"
second_title: "GroupDocs.Redaction voor .NET API-referentie"
description: "Maakt een kleur aan op basis van de opgegeven naam van een bekende kleur. Als de naam geen bekende kleurnaam is, wordt er een uitzondering gegooid."
type: docs
weight: 1440
url: /nl/net/groupdocs.redaction.options.drawing/color/fromname/
---
## Color.FromName method

Maakt een kleur aan op basis van de opgegeven naam van een bekende kleur. Als *name* geen bekende kleurnaam is, wordt er een uitzondering gegooid.

```csharp
public static Color FromName(string name)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| name | String | De naam van een bekende kleur, zoals `Red` of `Black`. |

### Retourwaarde

De benoemde kleur.

### Uitzonderingen

| uitzondering | conditie |
| --- | --- |
| ArgumentNullException | *name* is `null`. |
| ArgumentException | *name* is geen bekende kleurnaam. |

### Zie ook

* struct [Color](../../color)
* namespace [GroupDocs.Redaction.Options.Drawing](../../../groupdocs.redaction.options.drawing)
* assembly [GroupDocs.Redaction](../../../)

<!-- NIET BEWERKEN: gegenereerd door xmldocmd voor GroupDocs.Redaction.dll -->
