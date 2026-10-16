---
title: "Rettangolo"
second_title: "Riferimento API di GroupDocs.Redaction per .NET"
description: "Descrive un'area rettangolare su una pagina o immagine, ad esempio i limiti del testo OCR o una casella di redazione."
type: docs
weight: 350
url: /it/net/groupdocs.redaction.options.drawing/rectangle/
---
## Rectangle structure

Descrive un'area rettangolare su una pagina o immagine, ad esempio i limiti del testo OCR o una casella di redazione.

```csharp
public struct Rectangle : IEquatable<Rectangle>
```

## Costruttori

| Nome | Descrizione |
| --- | --- |
| [Rectangle](rectangle#constructor)(Point, Size) | Crea un rettangolo a partire da un punto in alto a sinistra e dalla dimensione della regione. |
| [Rectangle](rectangle#constructor_1)(int, int, int, int) | Crea un rettangolo a partire dalle coordinate degli angoli e dalle dimensioni. |

## Proprietà

| Nome | Descrizione |
| --- | --- |
| static [Empty](../../groupdocs.redaction.options.drawing/rectangle/empty) { get; } | Un rettangolo con larghezza e altezza zero all'origine. |
| [Height](../../groupdocs.redaction.options.drawing/rectangle/height) { get; set; } | Altezza dell'area, in pixel. |
| [IsEmpty](../../groupdocs.redaction.options.drawing/rectangle/isempty) { get; } | Ottiene un valore che indica se il rettangolo è vuoto. |
| [Location](../../groupdocs.redaction.options.drawing/rectangle/location) { get; } | Angolo in alto a sinistra del rettangolo. |
| [Size](../../groupdocs.redaction.options.drawing/rectangle/size) { get; } | Larghezza e altezza del rettangolo. |
| [Width](../../groupdocs.redaction.options.drawing/rectangle/width) { get; set; } | Larghezza dell'area, in pixel. |
| [X](../../groupdocs.redaction.options.drawing/rectangle/x) { get; set; } | Posizione orizzontale dell'angolo in alto a sinistra, in pixel. |
| [Y](../../groupdocs.redaction.options.drawing/rectangle/y) { get; set; } | Posizione verticale dell'angolo in alto a sinistra, in pixel. |

## Metodi

| Nome | Descrizione |
| --- | --- |
| override [Equals](../../groupdocs.redaction.options.drawing/rectangle/equals#equals_1)(object) | Confronta questo rettangolo con un altro oggetto. |
| [Equals](../../groupdocs.redaction.options.drawing/rectangle/equals#equals)(Rectangle) | Confronta i limiti con un altro rettangolo. |
| override [GetHashCode](../../groupdocs.redaction.options.drawing/rectangle/gethashcode)() | Restituisce un codice hash derivato da posizione e dimensione. |
| override [ToString](../../groupdocs.redaction.options.drawing/rectangle/tostring)() | Restituisce i limiti in una forma leggibile. |

### Vedi anche

* namespace [GroupDocs.Redaction.Options.Drawing](../../groupdocs.redaction.options.drawing)
* assembly [GroupDocs.Redaction](../../)

<!-- NON MODIFICARE: generato da xmldocmd per GroupDocs.Redaction.dll -->
