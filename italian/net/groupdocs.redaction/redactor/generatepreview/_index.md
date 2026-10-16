---
title: "GeneratePreview"
second_title: "Riferimento API di GroupDocs.Redaction per .NET"
description: "Genera immagini di anteprima di pagine specifiche in un determinato formato immagine."
type: docs
weight: 40
url: /it/net/groupdocs.redaction/redactor/generatepreview/
---
## Redactor.GeneratePreview method

Genera immagini di anteprima di pagine specifiche in un determinato formato immagine.

```csharp
public void GeneratePreview(PreviewOptions previewOptions)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| previewOptions | PreviewOptions | Proprietà dell'immagine e impostazioni dell'intervallo di pagine |

### Esempi

Il seguente esempio dimostra come ottenere un'anteprima del documento usando [`PreviewOptions`](../../../groupdocs.redaction.options/previewoptions) e entrambi i delegati.

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

* class [PreviewOptions](../../../groupdocs.redaction.options/previewoptions)
* class [Redactor](../../redactor)
* namespace [GroupDocs.Redaction](../../../groupdocs.redaction)
* assembly [GroupDocs.Redaction](../../../)

<!-- NON MODIFICARE: generato da xmldocmd per GroupDocs.Redaction.dll -->
