---
title: "Punto"
second_title: "Riferimento API di GroupDocs.Redaction per .NET"
description: "Identifica una compensazione in pixel su una pagina o immagine, solitamente l'angolo in alto a sinistra di un'area di redazione."
type: docs
weight: 340
url: /it/net/groupdocs.redaction.options.drawing/point/
---
## Point structure

Identifica uno spostamento di pixel su una pagina o immagine, solitamente l'angolo in alto a sinistra di un'area di redazione.

```csharp
public struct Point : IEquatable<Point>
```

## Costruttori

| Nome | Descrizione |
| --- | --- |
| [Point](point)(int, int) | Crea un punto per l'origine della regione di redazione. |

## Proprietà

| Nome | Descrizione |
| --- | --- |
| static [Empty](../../groupdocs.redaction.options.drawing/point/empty) { get; } | Un punto all'origine (0, 0). |
| [X](../../groupdocs.redaction.options.drawing/point/x) { get; } | Compensazione orizzontale dal bordo sinistro, in pixel. |
| [Y](../../groupdocs.redaction.options.drawing/point/y) { get; } | Compensazione verticale dal bordo superiore, in pixel. |

## Metodi

| Nome | Descrizione |
| --- | --- |
| override [Equals](../../groupdocs.redaction.options.drawing/point/equals#equals_1)(object) | Confronta questo punto con un altro oggetto. |
| [Equals](../../groupdocs.redaction.options.drawing/point/equals#equals)(Point) | Confronta le coordinate con un altro punto. |
| override [GetHashCode](../../groupdocs.redaction.options.drawing/point/gethashcode)() | Restituisce un codice hash derivato dalle coordinate. |
| override [ToString](../../groupdocs.redaction.options.drawing/point/tostring)() | Restituisce le coordinate in forma leggibile. |

### Vedi anche

* namespace [GroupDocs.Redaction.Options.Drawing](../../groupdocs.redaction.options.drawing)
* assembly [GroupDocs.Redaction](../../)

<!-- NON MODIFICARE: generato da xmldocmd per GroupDocs.Redaction.dll -->
