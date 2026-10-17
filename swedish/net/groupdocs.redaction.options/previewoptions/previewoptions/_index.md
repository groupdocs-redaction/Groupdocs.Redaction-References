---
title: "PreviewOptions"
second_title: "GroupDocs.Redaction för .NET API-referens"
description: "Initierar en ny instans av PreviewOptions-klassen vilket får utmatningsströmmen att stängas."
type: docs
weight: 10
url: /sv/net/groupdocs.redaction.options/previewoptions/previewoptions/
---
## PreviewOptions(CreatePageStream) {#constructor}

Initierar en ny instans av PreviewOptions-klassen, vilket får utdataströmmen att stängas.

```csharp
public PreviewOptions(CreatePageStream createPageStream)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| createPageStream | CreatePageStream | Skapar en ström för en specifik sidförhandsgranskning |

### Se även

* delegate [CreatePageStream](../../createpagestream)
* class [PreviewOptions](../../previewoptions)
* namespace [GroupDocs.Redaction.Options](../../../groupdocs.redaction.options)
* assembly [GroupDocs.Redaction](../../../)

---

## PreviewOptions(CreatePageStream, ReleasePageStream) {#constructor_1}

Initierar en ny instans av PreviewOptions-klassen, vilket får utdataströmmen att returneras till klienten för vidare användning.

```csharp
public PreviewOptions(CreatePageStream createPageStream, ReleasePageStream releasePageStream)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| createPageStream | CreatePageStream | Skapar en ström för en specifik sidförhandsgranskning |
| releasePageStream | ReleasePageStream | Meddelar att genereringen av sidförhandsgranskning är klar och hämtar utdataström |

### Se även

* delegate [CreatePageStream](../../createpagestream)
* delegate [ReleasePageStream](../../releasepagestream)
* class [PreviewOptions](../../previewoptions)
* namespace [GroupDocs.Redaction.Options](../../../groupdocs.redaction.options)
* assembly [GroupDocs.Redaction](../../../)

<!-- GÅ INTE ATT REDIGERA: genererad av xmldocmd för GroupDocs.Redaction.dll -->
