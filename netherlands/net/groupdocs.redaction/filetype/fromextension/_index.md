---
title: "FromExtension"
second_title: "GroupDocs.Redaction voor .NET API-referentie"
description: "Koppelt bestandsextensie aan bestandstype."
type: docs
weight: 500
url: /nl/net/groupdocs.redaction/filetype/fromextension/
---
## FileType.FromExtension method

Koppelt bestandsextensie aan bestandstype.

```csharp
public static FileType FromExtension(string extension)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| extensie | String | Bestandsextensie (inclusief de punt "."). |

### Retourwaarde

Wanneer het bestandstype wordt ondersteund, retourneert het, anders retourneert het het standaard [`Unknown`](../unknown) bestandstype.

### Uitzonderingen

| uitzondering | conditie |
| --- | --- |
| ArgumentException | Wordt gegooid wanneer *extension* null of een lege tekenreeks is. |

### Zie ook

* class [FileType](../../filetype)
* namespace [GroupDocs.Redaction](../../../groupdocs.redaction)
* assembly [GroupDocs.Redaction](../../../)

<!-- NIET BEWERKEN: gegenereerd door xmldocmd voor GroupDocs.Redaction.dll -->
