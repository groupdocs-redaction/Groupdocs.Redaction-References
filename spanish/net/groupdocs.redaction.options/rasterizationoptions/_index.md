---
title: RasterizationOptions
second_title: Referencia de API de GroupDocs.Redaction para .NET
description: Proporciona opciones para convertir archivos a PDF.
type: docs
weight: 350
url: /es/net/groupdocs.redaction.options/rasterizationoptions/
---
## RasterizationOptions class

Proporciona opciones para convertir archivos a PDF.

```csharp
public class RasterizationOptions
```

## Constructores

| Nombre | Descripción |
| --- | --- |
| [RasterizationOptions](rasterizationoptions)() | Inicializa una nueva instancia. |

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [Compliance](../../groupdocs.redaction.options/rasterizationoptions/compliance) { get; set; } | Obtiene o establece el nivel de cumplimiento de PDF. |
| [Enabled](../../groupdocs.redaction.options/rasterizationoptions/enabled) { get; set; } | Obtiene o establece un valor que indica si todas las páginas del documento deben convertirse en imágenes y colocarse en un solo archivo PDF. VERDADERO de forma predeterminada, establecido en FALSO para evitar la rasterización. |
| [HasAdvancedOptions](../../groupdocs.redaction.options/rasterizationoptions/hasadvancedoptions) { get; } | Obtiene un indicador, que es verdadero si se establecen opciones de rasterización avanzadas. |
| [PageCount](../../groupdocs.redaction.options/rasterizationoptions/pagecount) { get; set; } | Obtiene o establece el número de páginas que se convertirán a PDF. |
| [PageIndex](../../groupdocs.redaction.options/rasterizationoptions/pageindex) { get; set; } | Obtiene o establece el índice de la primera página (basado en 0) para convertir a PDF. |

## Métodos

| Nombre | Descripción |
| --- | --- |
| [AddAdvancedOption](../../groupdocs.redaction.options/rasterizationoptions/addadvancedoption#addadvancedoption)(AdvancedRasterizationOptions) | Puede usar este método para registrar una opción de rasterización avanzada para aplicar. |
| [AddAdvancedOption](../../groupdocs.redaction.options/rasterizationoptions/addadvancedoption#addadvancedoption_1)(AdvancedRasterizationOptions, Dictionary&lt;string, string&gt;) | Puede usar este método para registrar una opción de rasterización avanzada para aplicar. |

### Observaciones

**Aprende más**

* Más detalles sobre cómo guardar un documento como PDF rasterizado: [Guardar en PDF rasterizado](https://docs.groupdocs.com/redaction/net/save-in-rasterized-pdf/)
* Más detalles sobre las opciones de rasterización: [Seleccionar páginas específicas para PDF rasterizado](https://docs.groupdocs.com/redaction/net/select-specific-pages-for-rasterized-pdf/)

### Ejemplos

El siguiente ejemplo demuestra cómo establecer opciones para el proceso de rasterización.

```csharp
    using (var redactor = new Redactor("SomePresentation.pptx"))
    {
        // redactar datos confidenciales en la primera diapositiva 
    
        var rasterizationOptions = new RasterizationOptions();
        rasterizationOptions.PageIndex = 0;
        rasterizationOptions.PageCount = 1;
        rasterizationOptions.Compliance = PdfComplianceLevel.PdfA1a;
        using (var stream = File.Open(Path.Combine(@"C:\Temp", "PresentationFirstSlide.pdf")))
        {
            redactor.Save(stream, rasterizationOptions);
        }
    }      
```

El siguiente ejemplo demuestra cómo aplicar las opciones de rasterización avanzadas con la configuración predeterminada.

```csharp
    using (Redactor redactor = new Redactor(@"C:\sample.docx"))
    {
      // Guardar el documento con las opciones predeterminadas (convertir páginas en imágenes, guardar como PDF)
      var so = new SaveOptions();
      so.Rasterization.Enabled = true;
      so.RedactedFileSuffix = "_scan";
      so.Rasterization.AddAdvancedOption(AdvancedRasterizationOptions.Border);
      so.Rasterization.AddAdvancedOption(AdvancedRasterizationOptions.Noise);
      so.Rasterization.AddAdvancedOption(AdvancedRasterizationOptions.Grayscale);
      so.Rasterization.AddAdvancedOption(AdvancedRasterizationOptions.Tilt);
      redactor.Save(so);
    }
```

El siguiente ejemplo muestra cómo aplicar la opción de rasterización avanzada de bordes con configuraciones personalizadas.

```csharp
    using (Redactor redactor = new Redactor(@"C:\sample.docx"))
    {
      // Guarda el documento con un borde personalizado
      var so = new SaveOptions();
      so.Rasterization.Enabled = true;
      so.RedactedFileSuffix = "_scan";
      so.Rasterization.AddAdvancedOption(AdvancedRasterizationOptions.Border, new Dictionary<string, string>() { { "border", "10" } });
      redactor.Save(so);
    }
```

El siguiente ejemplo muestra cómo aplicar la opción de rasterización avanzada de ruido con configuraciones personalizadas.

```csharp
    using (Redactor redactor = new Redactor(@"C:\sample.docx"))
    {
      // Guarde el documento con el número personalizado y el tamaño de los efectos de ruido
      var so = new SaveOptions();
      so.Rasterization.Enabled = true;
      so.RedactedFileSuffix = "_scan";
      so.Rasterization.AddAdvancedOption(AdvancedRasterizationOptions.Noise, 
          new Dictionary<string, string>() { { "maxSpots", "150" }, { "spotMaxSize", "15" } });
      redactor.Save(so);
    }
```

El siguiente ejemplo muestra cómo aplicar la opción de rasterización avanzada de inclinación con configuraciones personalizadas.

```csharp
    using (Redactor redactor = new Redactor(@"C:\sample.docx"))
    {
      // Guarda el documento con el efecto de inclinación personalizado
      var so = new SaveOptions();
      so.Rasterization.Enabled = true;
      so.RedactedFileSuffix = "_scan";
      so.Rasterization.AddAdvancedOption(AdvancedRasterizationOptions.Tilt, 
          new Dictionary<string, string>() { { { "minAngle", "85" }, { "randomAngleMax", "5" } });
      redactor.Save(so);
    }
```

### Ver también

* espacio de nombres [GroupDocs.Redaction.Options](../../groupdocs.redaction.options)
* asamblea [GroupDocs.Redaction](../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Redaction.dll -->
