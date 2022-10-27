---
title: ReleasePageStream
second_title: Referencia de API de GroupDocs.Redaction para .NET
description: Representa un método que libera flujo creado porCreatePageStream./createpagestream delegar.
type: docs
weight: 360
url: /es/net/groupdocs.redaction.options/releasepagestream/
---
## ReleasePageStream delegate

Representa un método que libera flujo creado por[`CreatePageStream`](../createpagestream) delegar.

```csharp
public delegate void ReleasePageStream(int pageNumber, Stream pageStream);
```

| Parámetro | Escribe | Descripción |
| --- | --- | --- |
| pageNumber | Int32 | Número de página de la vista previa de la página generada |
| pageStream | Stream | Stream, que contiene la vista previa de la página generada |

### Ejemplos

El siguiente ejemplo demuestra cómo obtener una vista previa del documento usando[`PreviewOptions`](../previewoptions) y ambos delegados.

```csharp
    CreatePageStream createDelegate = delegate (int pageNumber)
    {
        var pagePath = System.IO.Path.Combine(@"C:\Temp", string.Format("page_{0}.png", pageNumber));
        return System.IO.File.Create(pagePath);
    };
    ReleasePageStream releaseDelegate = delegate (int pageNumber, System.IO.Stream pageStream)
    {
        // hacer cualquier cosa con Stream, que contiene una vista previa de la página
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

### Ver también

* espacio de nombres [GroupDocs.Redaction.Options](../../groupdocs.redaction.options)
* asamblea [GroupDocs.Redaction](../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Redaction.dll -->