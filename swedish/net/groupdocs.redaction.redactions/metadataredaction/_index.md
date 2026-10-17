---
title: "MetadataRedaction"
second_title: "GroupDocs.Redaction för .NET API-referens"
description: "Representerar en bas‑abstrakt klass för dokumentmetadata‑redigeringar."
type: docs
weight: 650
url: /sv/net/groupdocs.redaction.redactions/metadataredaction/
---
## MetadataRedaction class

Representerar en bas‑abstrakt klass för dokumentmetadata‑redigeringar.

```csharp
public abstract class MetadataRedaction : Redaction
```

## Egenskaper

| Namn | Beskrivning |
| --- | --- |
| virtual [Description](../../groupdocs.redaction/redaction/description) { get; } | Returnerar en sträng som beskriver redaction och dess parametrar. |
| [Filter](../../groupdocs.redaction.redactions/metadataredaction/filter) { get; set; } | Hämtar eller anger filtret som används för att välja all eller specifik metadata, till exempel Author eller Company. |

## Metoder

| Namn | Beskrivning |
| --- | --- |
| override [ApplyTo](../../groupdocs.redaction.redactions/metadataredaction/applyto)(DocumentFormatInstance) | Tillämpar redaction på en given formatinstans. |

### Anmärkningar

**Learn more**

* More details about document metadata redactions: [Metadata redactions](https://docs.groupdocs.com/redaction/net/metadata-redactions/)

### Se även

* class [Redaction](../../groupdocs.redaction/redaction)
* namespace [GroupDocs.Redaction.Redactions](../../groupdocs.redaction.redactions)
* assembly [GroupDocs.Redaction](../../)

<!-- GÅ INTE ATT REDIGERA: genererad av xmldocmd för GroupDocs.Redaction.dll -->
