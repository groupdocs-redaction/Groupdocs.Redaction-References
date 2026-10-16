---
title: "MetadataRedaction"
second_title: "GroupDocs.Redaction voor .NET API-referentie"
description: "Stelt een basis abstracte klasse voor documentmetadata‑redacties voor."
type: docs
weight: 650
url: /nl/net/groupdocs.redaction.redactions/metadataredaction/
---
## MetadataRedaction class

Stelt een basis abstracte klasse voor documentmetadata‑redacties voor.

```csharp
public abstract class MetadataRedaction : Redaction
```

## Properties

| Naam | Beschrijving |
| --- | --- |
| virtual [Description](../../groupdocs.redaction/redaction/description) { get; } | Retourneert een string die de redactie en de parameters beschrijft. |
| [Filter](../../groupdocs.redaction.redactions/metadataredaction/filter) { get; set; } | Haalt de filter op of stelt deze in, die wordt gebruikt om alle of specifieke metadata te selecteren, bijvoorbeeld Auteur of Bedrijf. |

## Methoden

| Naam | Beschrijving |
| --- | --- |
| override [ApplyTo](../../groupdocs.redaction.redactions/metadataredaction/applyto)(DocumentFormatInstance) | Past de redactie toe op een gegeven format‑instantie. |

### Opmerkingen

**Learn more**

* More details about document metadata redactions: [Metadata redactions](https://docs.groupdocs.com/redaction/net/metadata-redactions/)

### Zie ook

* class [Redaction](../../groupdocs.redaction/redaction)
* namespace [GroupDocs.Redaction.Redactions](../../groupdocs.redaction.redactions)
* assembly [GroupDocs.Redaction](../../)

<!-- NIET BEWERKEN: gegenereerd door xmldocmd voor GroupDocs.Redaction.dll -->
