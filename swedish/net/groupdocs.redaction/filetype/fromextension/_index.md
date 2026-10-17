---
title: "FromExtension"
second_title: "GroupDocs.Redaction för .NET API-referens"
description: "Karterar filändelse till filtyp."
type: docs
weight: 500
url: /sv/net/groupdocs.redaction/filetype/fromextension/
---
## FileType.FromExtension method

Karterar filändelse till filtyp.

```csharp
public static FileType FromExtension(string extension)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| extension | String | Filändelse (inklusive punkten "."). |

### Returvärde

När filtypen stöds returneras den, annars returneras standard [`Unknown`](../unknown) filtyp.

### Undantag

| undantag | villkor |
| --- | --- |
| ArgumentException | Kastas när *extension* är null eller en tom sträng. |

### Se även

* class [FileType](../../filetype)
* namespace [GroupDocs.Redaction](../../../groupdocs.redaction)
* assembly [GroupDocs.Redaction](../../../)

<!-- GÅ INTE ATT REDIGERA: genererad av xmldocmd för GroupDocs.Redaction.dll -->
