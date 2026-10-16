---
title: "RegionReplacementOptions"
second_title: "Riferimento API di GroupDocs.Redaction per .NET"
description: "Rappresenta i parametri di colore e area per la sostituzione di regioni immagine. Vedi ImageAreaRedaction./imagearearedaction."
type: docs
weight: 760
url: /it/net/groupdocs.redaction.redactions/regionreplacementoptions/
---
## RegionReplacementOptions class

Rappresenta i parametri di colore e area per la sostituzione di regioni immagine. Vedi [`ImageAreaRedaction`](../imagearearedaction).

```csharp
public class RegionReplacementOptions
```

## Costruttori

| Nome | Descrizione |
| --- | --- |
| [RegionReplacementOptions](regionreplacementoptions#constructor_1)(Color, Size) | Inizializza una nuova istanza della classe RegionReplacementOptions. |
| [RegionReplacementOptions](regionreplacementoptions#constructor)(Color, Font, string) | Inizializza una nuova istanza della classe RegionReplacementOptions la cui dimensione corrisponde al testo fornito. |

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [FillColor](../../groupdocs.redaction.redactions/regionreplacementoptions/fillcolor) { get; set; } | Ottiene o imposta il colore per riempire l'area redatta. |
| [Size](../../groupdocs.redaction.redactions/regionreplacementoptions/size) { get; set; } | Ottiene o imposta il rettangolo con larghezza e altezza. |

### Osservazioni

**Learn more**

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

* namespace [GroupDocs.Redaction.Redactions](../../groupdocs.redaction.redactions)
* assembly [GroupDocs.Redaction](../../)

<!-- NON MODIFICARE: generato da xmldocmd per GroupDocs.Redaction.dll -->
