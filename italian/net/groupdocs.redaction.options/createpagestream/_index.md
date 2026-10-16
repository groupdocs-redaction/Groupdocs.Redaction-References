---
title: "CreatePageStream"
second_title: "Riferimento API di GroupDocs.Redaction per .NET"
description: "Rappresenta un metodo che restituisce uno stream per scrivere i dati dell'anteprima della pagina."
type: docs
weight: 300
url: /it/net/groupdocs.redaction.options/createpagestream/
---
## CreatePageStream delegate

Rappresenta un metodo che restituisce uno stream per scrivere i dati dell'anteprima della pagina.

```csharp
public delegate Stream CreatePageStream(int pageNumber);
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| pageNumber | Int32 | Numero di pagina di una pagina per generare la miniatura |

### Valore di ritorno

Stream per scrivere l'anteprima della pagina

### Esempi

Il seguente esempio dimostra come ottenere un'anteprima del documento utilizzando il delegato [`PreviewOptions`](../previewoptions) e [`CreatePageStream`](../createpagestream).

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

### Vedi anche

* namespace [GroupDocs.Redaction.Options](../../groupdocs.redaction.options)
* assembly [GroupDocs.Redaction](../../)

<!-- NON MODIFICARE: generato da xmldocmd per GroupDocs.Redaction.dll -->
