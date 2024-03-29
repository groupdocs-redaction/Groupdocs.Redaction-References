---
title: RegionReplacementOptions
second_title: Referencia de API de GroupDocs.Redaction para .NET
description: Representa los parámetros de color y área para el reemplazo de la región de la imagen. VerImageAreaRedaction./imagearearedaction .
type: docs
weight: 600
url: /es/net/groupdocs.redaction.redactions/regionreplacementoptions/
---
## RegionReplacementOptions class

Representa los parámetros de color y área para el reemplazo de la región de la imagen. Ver[`ImageAreaRedaction`](../imagearearedaction) .

```csharp
public class RegionReplacementOptions
```

## Constructores

| Nombre | Descripción |
| --- | --- |
| [RegionReplacementOptions](regionreplacementoptions#constructor_1)(Color, Size) | Inicializa una nueva instancia de la clase RegionReplacementOptions. |
| [RegionReplacementOptions](regionreplacementoptions#constructor)(Color, Font, string) | Inicializa una nueva instancia de la clase RegionReplacementOptions cuyo tamaño coincide con el texto dado. |

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [FillColor](../../groupdocs.redaction.redactions/regionreplacementoptions/fillcolor) { get; set; } | Obtiene o establece el color para rellenar el área redactada. |
| [Size](../../groupdocs.redaction.redactions/regionreplacementoptions/size) { get; set; } | Obtiene o establece el rectángulo con y altura. |

### Observaciones

**Aprende más**

* Más detalles sobre las redacciones de imágenes: [Redacciones de imágenes](https://docs.groupdocs.com/redaction/net/image-redactions/)

### Ejemplos

El siguiente ejemplo muestra cómo reemplazar un área dentro de la imagen con un rectángulo de color sólido.

```csharp
    using (Redactor redactor = new Redactor("D:\\test.jpg"))
    {
       System.Drawing.Point samplePoint = new System.Drawing.Point(516, 311);
       System.Drawing.Size sampleSize = new System.Drawing.Size(170, 35);
       RedactorChangeLog result = redactor.Apply(new ImageAreaRedaction(samplePoint,
                     new RegionReplacementOptions(System.Drawing.Color.Blue, sampleSize)));
       if (result.Status != RedactionStatus.Failed)
       {
          redactor.Save();
       };
    } 
```

### Ver también

* espacio de nombres [GroupDocs.Redaction.Redactions](../../groupdocs.redaction.redactions)
* asamblea [GroupDocs.Redaction](../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Redaction.dll -->
