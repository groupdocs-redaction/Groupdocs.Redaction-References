---
title: "PreviewOptions"
second_title: "GroupDocs.Redaction voor .NET API-referentie"
description: "Initialiseert een nieuw exemplaar van de PreviewOptions-klasse waardoor de outputstroom wordt gesloten."
type: docs
weight: 10
url: /nl/net/groupdocs.redaction.options/previewoptions/previewoptions/
---
## PreviewOptions(CreatePageStream) {#constructor}

Initialiseert een nieuwe instantie van de klasse PreviewOptions, waardoor de uitvoerstroom wordt gesloten.

```csharp
public PreviewOptions(CreatePageStream createPageStream)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| createPageStream | CreatePageStream | Maakt een stream voor een specifiek paginavoorbeeld |

### Zie ook

* delegate [CreatePageStream](../../createpagestream)
* class [PreviewOptions](../../previewoptions)
* namespace [GroupDocs.Redaction.Options](../../../groupdocs.redaction.options)
* assembly [GroupDocs.Redaction](../../../)

---

## PreviewOptions(CreatePageStream, ReleasePageStream) {#constructor_1}

Initialiseert een nieuwe instantie van de klasse PreviewOptions, waardoor de uitvoerstroom wordt teruggegeven aan de client voor verder gebruik.

```csharp
public PreviewOptions(CreatePageStream createPageStream, ReleasePageStream releasePageStream)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| createPageStream | CreatePageStream | Maakt een stream voor een specifiek paginavoorbeeld |
| releasePageStream | ReleasePageStream | Meldt dat de generatie van het paginavoorbeeld is voltooid en haalt de outputstream |

### Zie ook

* delegate [CreatePageStream](../../createpagestream)
* delegate [ReleasePageStream](../../releasepagestream)
* class [PreviewOptions](../../previewoptions)
* namespace [GroupDocs.Redaction.Options](../../../groupdocs.redaction.options)
* assembly [GroupDocs.Redaction](../../../)

<!-- NIET BEWERKEN: gegenereerd door xmldocmd voor GroupDocs.Redaction.dll -->
