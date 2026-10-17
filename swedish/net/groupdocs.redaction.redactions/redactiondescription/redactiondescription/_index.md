---
title: "RedactionDescription"
second_title: "GroupDocs.Redaction för .NET API-referens"
description: "Initierar en ny instans av klassen RedactionDescription utan ersättningsinformation."
type: docs
weight: 10
url: /sv/net/groupdocs.redaction.redactions/redactiondescription/redactiondescription/
---
## RedactionDescription(RedactionType, RedactionActionType, string) {#constructor_1}

Initierar en ny instans av klassen RedactionDescription utan ersättningsinformation.

```csharp
public RedactionDescription(RedactionType redactionType, RedactionActionType actionType, 
    string originalText)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| redactionType | RedactionType | Typ av data som redigeras |
| actionType | RedactionActionType | Åtgärd som ska utföras på dessa data |
| originalText | String | Matchad text, kommentar eller annoteringsinnehåll |

### Se även

* enum [RedactionType](../../redactiontype)
* enum [RedactionActionType](../../redactionactiontype)
* class [RedactionDescription](../../redactiondescription)
* namespace [GroupDocs.Redaction.Redactions](../../../groupdocs.redaction.redactions)
* assembly [GroupDocs.Redaction](../../../)

---

## RedactionDescription(RedactionType, RedactionActionType, string, TextReplacement) {#constructor_2}

Initierar en ny instans av klassen RedactionDescription med ersättningsinformation.

```csharp
public RedactionDescription(RedactionType redactionType, RedactionActionType actionType, 
    string originalText, TextReplacement replacement)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| redactionType | RedactionType | Typ av data som redigeras |
| actionType | RedactionActionType | Åtgärd som ska utföras på dessa data |
| originalText | String | Matchad text, kommentar eller annoteringsinnehåll |
| ersättning | TextReplacement | Ersättningstext, matchad text och dess position inom originalsträngen |

### Se även

* enum [RedactionType](../../redactiontype)
* enum [RedactionActionType](../../redactionactiontype)
* class [TextReplacement](../../textreplacement)
* class [RedactionDescription](../../redactiondescription)
* namespace [GroupDocs.Redaction.Redactions](../../../groupdocs.redaction.redactions)
* assembly [GroupDocs.Redaction](../../../)

---

## RedactionDescription(RedactionType, RedactionActionType, RegionReplacementOptions, string) {#constructor}

Initierar en ny instans av klassen RedactionDescription med ersättningsinformation för bildområde.

```csharp
public RedactionDescription(RedactionType redactionType, RedactionActionType actionType, 
    RegionReplacementOptions imageAreaReplacement, string imageDetails)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| redactionType | RedactionType | Typ av data som redigeras |
| actionType | RedactionActionType | Åtgärd som ska utföras på dessa data |
| imageAreaReplacement | RegionReplacementOptions | Information om bildområdesersättning |
| imageDetails | String | Bildtextuell beskrivning, som standard är den String.Empty |

### Se även

* enum [RedactionType](../../redactiontype)
* enum [RedactionActionType](../../redactionactiontype)
* class [RegionReplacementOptions](../../regionreplacementoptions)
* class [RedactionDescription](../../redactiondescription)
* namespace [GroupDocs.Redaction.Redactions](../../../groupdocs.redaction.redactions)
* assembly [GroupDocs.Redaction](../../../)

<!-- GÅ INTE ATT REDIGERA: genererad av xmldocmd för GroupDocs.Redaction.dll -->
