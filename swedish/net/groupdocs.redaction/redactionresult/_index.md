---
title: "RedactionResult"
second_title: "GroupDocs.Redaction för .NET API-referens"
description: "Representerar resultatet av raderingsoperationen."
type: docs
weight: 510
url: /sv/net/groupdocs.redaction/redactionresult/
---
## RedactionResult class

Representerar resultatet av raderingsoperationen.

```csharp
public class RedactionResult
```

## Egenskaper

| Namn | Beskrivning |
| --- | --- |
| [ErrorMessage](../../groupdocs.redaction/redactionresult/errormessage) { get; } | Hämtar felmeddelandet för diagnostik. |
| [Status](../../groupdocs.redaction/redactionresult/status) { get; } | Hämtar körningsstatusen. |

## Metoder

| Namn | Beskrivning |
| --- | --- |
| static [Failed](../../groupdocs.redaction/redactionresult/failed)(string) | Initierar en ny instans av RedactionResult‑klassen med statusen Failed. |
| static [Partial](../../groupdocs.redaction/redactionresult/partial)(string) | Initierar en ny instans av RedactionResult‑klassen med statusen PartiallyApplied. |
| static [Skipped](../../groupdocs.redaction/redactionresult/skipped)(string) | Initierar en ny instans av RedactionResult‑klassen med statusen Skipped. |
| static [Successful](../../groupdocs.redaction/redactionresult/successful)() | Initierar en ny instans av RedactionResult‑klassen med statusen Applied (framgångsrik). |

### Anmärkningar

**Learn more**

* More details about redaction results: [Redaction basics](https://docs.groupdocs.com/redaction/net/redaction-basics/)

### Se även

* namespace [GroupDocs.Redaction](../../groupdocs.redaction)
* assembly [GroupDocs.Redaction](../../)

<!-- GÅ INTE ATT REDIGERA: genererad av xmldocmd för GroupDocs.Redaction.dll -->
