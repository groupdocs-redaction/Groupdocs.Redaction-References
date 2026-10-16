---
title: "ImageAreaRedaction"
second_title: "Riferimento API di GroupDocs.Redaction per .NET"
description: "Rappresenta una redazione che inserisce un rettangolo colorato nell'area specificata di un documento immagine."
type: docs
weight: 630
url: /it/net/groupdocs.redaction.redactions/imagearearedaction/
---
## ImageAreaRedaction class

Rappresenta una redazione che inserisce un rettangolo colorato nell'area specificata di un documento immagine.

```csharp
public class ImageAreaRedaction : Redaction
```

## Costruttori

| Nome | Descrizione |
| --- | --- |
| [ImageAreaRedaction](imagearearedaction)(Point, RegionReplacementOptions) | Inizializza una nuova istanza della classe ImageAreaRedaction per la redazione di una dimensione di area specifica. |

## Proprietà

| Nome | Descrizione |
| --- | --- |
| override [Description](../../groupdocs.redaction.redactions/imagearearedaction/description) { get; } | Restituisce una stringa che descrive la redazione e i suoi parametri. |
| [Options](../../groupdocs.redaction.redactions/imagearearedaction/options) { get; } | Restituisce le opzioni [`RegionReplacementOptions`](../regionreplacementoptions) con parametri di colore e area. |
| [TopLeft](../../groupdocs.redaction.redactions/imagearearedaction/topleft) { get; } | Ottiene la posizione in alto a sinistra dell'area da rimuovere |

## Metodi

| Nome | Descrizione |
| --- | --- |
| override [ApplyTo](../../groupdocs.redaction.redactions/imagearearedaction/applyto)(DocumentFormatInstance) | Applica la redazione a una determinata istanza di formato. |

### Osservazioni

**Learn more**

* More details about applying redactions: [Redaction basics](https://docs.groupdocs.com/redaction/net/redaction-basics/)
* More details about image redactions: [Image redactions](https://docs.groupdocs.com/redaction/net/image-redactions/)

### Esempi

Il seguente esempio dimostra la sostituzione di un'area all'interno dell'immagine con un rettangolo di colore solido.

```csharp
    using (Redactor redactor = new Redactor("D:\\test.jpg"))
    {
       GroupDocs.Redaction.Options.Drawing.Point samplePoint = new GroupDocs.Redaction.Options.Drawing.Point(516, 311);
       GroupDocs.Redaction.Options.Drawing.Size sampleSize = new GroupDocs.Redaction.Options.Drawing.Size(170, 35);
       RedactorChangeLog result = redactor.Apply(new ImageAreaRedaction(samplePoint,
                     new RegionReplacementOptions(GroupDocs.Redaction.Options.Drawing.Color.Blue, sampleSize)));
       if (result.Status != RedactionStatus.Failed)
       {
          redactor.Save();
       };
    } 
```

### Vedi anche

* class [Redaction](../../groupdocs.redaction/redaction)
* namespace [GroupDocs.Redaction.Redactions](../../groupdocs.redaction.redactions)
* assembly [GroupDocs.Redaction](../../)

<!-- NON MODIFICARE: generato da xmldocmd per GroupDocs.Redaction.dll -->
