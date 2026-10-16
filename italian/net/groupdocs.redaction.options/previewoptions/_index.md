---
title: "PreviewOptions"
second_title: "Riferimento API di GroupDocs.Redaction per .NET"
description: "Fornisce le opzioni per impostare i requisiti e i delegati di stream per la generazione dell'anteprima."
type: docs
weight: 400
url: /it/net/groupdocs.redaction.options/previewoptions/
---
## PreviewOptions class

Fornisce le opzioni per impostare i requisiti e i delegati di stream per la generazione dell'anteprima.

```csharp
public class PreviewOptions
```

## Costruttori

| Nome | Descrizione |
| --- | --- |
| [PreviewOptions](previewoptions#constructor)(CreatePageStream) | Inizializza una nuova istanza della classe PreviewOptions, facendo chiudere lo stream di output. |
| [PreviewOptions](previewoptions#constructor_1)(CreatePageStream, ReleasePageStream) | Inizializza una nuova istanza della classe PreviewOptions, facendo restituire lo stream di output al client per un uso successivo. |

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [CreatePageStream](../../groupdocs.redaction.options/previewoptions/createpagestream) { get; set; } | Ottiene o imposta un'istanza del delegato per la creazione dello stream di pagina. |
| [Height](../../groupdocs.redaction.options/previewoptions/height) { get; set; } | Ottiene o imposta l'altezza dell'anteprima della pagina. |
| [PageNumbers](../../groupdocs.redaction.options/previewoptions/pagenumbers) { get; set; } | Ottiene o imposta un array di numeri di pagina per generare l'anteprima. |
| [PreviewFormat](../../groupdocs.redaction.options/previewoptions/previewformat) { get; set; } | Ottiene o imposta il formato dell'immagine di anteprima. |
| [ReleasePageStream](../../groupdocs.redaction.options/previewoptions/releasepagestream) { get; set; } | Ottiene o imposta un'istanza del delegato di completamento dell'anteprima della pagina. |
| [Width](../../groupdocs.redaction.options/previewoptions/width) { get; set; } | Ottiene o imposta la larghezza dell'anteprima della pagina. |

### Esempi

Il seguente esempio dimostra come ottenere un'anteprima del documento utilizzando il delegato [`PreviewOptions`](../previewoptions) e [`CreatePageStream`](./createpagestream).

```csharp
    CreatePageStream createDelegate = delegate (int pageNumber)
    {
        var pagePath = System.IO.Path.Combine(@"C:\Temp", string.Format("page_{0}.png", pageNumber));
        return System.IO.File.Create(pagePath);
    };
    var previewOptions = new PreviewOptions(createDelegate);
    previewOptions.PreviewFormat = PreviewOptions.PreviewFormats.PNG;
    previewOptions.Height = 640;
    previewOptions.Width = 480;
    previewOptions.PageNumbers = new int[] { 1 };
    using (var redactor = new Redactor("C:\Temp\SourceFile.pdf"))
    {
        redactor.GeneratePreview(previewOptions);
    }
```

Il seguente esempio dimostra come ottenere un'anteprima del documento utilizzando [`PreviewOptions`](../previewoptions) e entrambi i delegati.

```csharp
    CreatePageStream createDelegate = delegate (int pageNumber)
    {
        var pagePath = System.IO.Path.Combine(@"C:\Temp", string.Format("page_{0}.png", pageNumber));
        return System.IO.File.Create(pagePath);
    };
    ReleasePageStream releaseDelegate = delegate (int pageNumber, System.IO.Stream pageStream)
    {
        // eseguire qualsiasi operazione con Stream, contenente l'anteprima della pagina
        pageStream.Close();
    };
    var previewOptions = new PreviewOptions(createDelegate, releaseDelegate);
    previewOptions.PreviewFormat = PreviewOptions.PreviewFormats.PNG;
    previewOptions.Height = 640;
    previewOptions.Width = 480;
    previewOptions.PageNumbers = new int[] { 1 };
    using (var redactor = new Redactor("C:\Temp\SourceFile.pdf"))
    {
        redactor.GeneratePreview(previewOptions);
    }
```

### Vedi anche

* namespace [GroupDocs.Redaction.Options](../../groupdocs.redaction.options)
* assembly [GroupDocs.Redaction](../../)

<!-- NON MODIFICARE: generato da xmldocmd per GroupDocs.Redaction.dll -->
