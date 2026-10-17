---
title: "FromName"
second_title: "GroupDocs.Redaction för .NET API-referens"
description: "Skapar en färg från det angivna namnet på en känd färg. Om namnet inte är ett känt färgnamn kastas ett undantag."
type: docs
weight: 1440
url: /sv/net/groupdocs.redaction.options.drawing/color/fromname/
---
## Color.FromName method

Skapar en färg från det angivna namnet på en känd färg. Om *name* inte är ett känt färgnamn kastas ett undantag.

```csharp
public static Color FromName(string name)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| name | String | Namnet på en känd färg, till exempel `Red` eller `Black`. |

### Returvärde

Den namngivna färgen.

### Undantag

| undantag | villkor |
| --- | --- |
| ArgumentNullException | *name* är `null`. |
| ArgumentException | *name* är inte ett känt färgnamn. |

### Se även

* struct [Color](../../color)
* namespace [GroupDocs.Redaction.Options.Drawing](../../../groupdocs.redaction.options.drawing)
* assembly [GroupDocs.Redaction](../../../)

<!-- GÅ INTE ATT REDIGERA: genererad av xmldocmd för GroupDocs.Redaction.dll -->
