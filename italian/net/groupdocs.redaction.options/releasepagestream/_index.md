---
title: "ReleasePageStream"
second_title: "Riferimento API di GroupDocs.Redaction per .NET"
description: "Rappresenta un metodo che rilascia lo stream creato dal delegato CreatePageStream./createpagestream."
type: docs
weight: 440
url: /it/net/groupdocs.redaction.options/releasepagestream/
---
## ReleasePageStream delegate

Rappresenta un metodo che rilascia lo stream creato dal delegato [`CreatePageStream`](../createpagestream).

```csharp
public delegate void ReleasePageStream(int pageNumber, Stream pageStream);
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| pageNumber | Int32 | Numero di pagina dell'anteprima della pagina generata |
| pageStream | Stream | Stream, contenente l'anteprima della pagina generata |

### Esempi

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
