---
title: AddAdvancedOption
second_title: Referencia de API de GroupDocs.Redaction para .NET
description: Puede usar este método para registrar una opción de rasterización avanzada para aplicar.
type: docs
weight: 70
url: /es/net/groupdocs.redaction.options/rasterizationoptions/addadvancedoption/
---
## AddAdvancedOption(AdvancedRasterizationOptions) {#addadvancedoption}

Puede usar este método para registrar una opción de rasterización avanzada para aplicar.

```csharp
public void AddAdvancedOption(AdvancedRasterizationOptions optionType)
```

| Parámetro | Escribe | Descripción |
| --- | --- | --- |
| optionType | AdvancedRasterizationOptions | Proporciona información sobre el tipo de efecto seleccionado (escala de grises, borde, etc.) |

### Ejemplos

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

### Ver también

* enum [AdvancedRasterizationOptions](../../advancedrasterizationoptions)
* class [RasterizationOptions](../../rasterizationoptions)
* espacio de nombres [GroupDocs.Redaction.Options](../../rasterizationoptions)
* asamblea [GroupDocs.Redaction](../../../)

---

## AddAdvancedOption(AdvancedRasterizationOptions, Dictionary&lt;string, string&gt;) {#addadvancedoption_1}

Puede usar este método para registrar una opción de rasterización avanzada para aplicar.

```csharp
public void AddAdvancedOption(AdvancedRasterizationOptions optionType, 
    Dictionary<string, string> parameters)
```

| Parámetro | Escribe | Descripción |
| --- | --- | --- |
| optionType | AdvancedRasterizationOptions | Proporciona información sobre el tipo de efecto seleccionado (escala de grises, borde, etc.) |
| parameters | Dictionary`2 | Parámetros para el efecto dado, como el ángulo de rotación |

### Ejemplos

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

* enum [AdvancedRasterizationOptions](../../advancedrasterizationoptions)
* class [RasterizationOptions](../../rasterizationoptions)
* espacio de nombres [GroupDocs.Redaction.Options](../../rasterizationoptions)
* asamblea [GroupDocs.Redaction](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Redaction.dll -->
