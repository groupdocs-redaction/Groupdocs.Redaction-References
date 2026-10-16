---
title: "AddAdvancedOption"
second_title: "GroupDocs.Redaction für .NET API-Referenz"
description: "Sie können diese Methode verwenden, um eine anzuwendende erweiterte Rasterungsoption zu registrieren."
type: docs
weight: 70
url: /de/net/groupdocs.redaction.options/rasterizationoptions/addadvancedoption/
---
## AddAdvancedOption(AdvancedRasterizationOptions) {#addadvancedoption}

Sie können diese Methode verwenden, um eine anzuwendende erweiterte Rasterungsoption zu registrieren.

```csharp
public void AddAdvancedOption(AdvancedRasterizationOptions optionType)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| optionType | AdvancedRasterizationOptions | Stellt Informationen über den ausgewählten Effekttyp bereit (Graustufen, Rahmen usw.) |

### Beispiele

Das folgende Beispiel zeigt, wie die erweiterten Rasterisierungsoptionen mit den Standardeinstellungen angewendet werden.

```csharp
    using (Redactor redactor = new Redactor(@"C:\sample.docx"))
    {
      // Dokument mit Standardoptionen speichern (Seiten in Bilder konvertieren, als PDF speichern)
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

### Siehe auch

* enum [AdvancedRasterizationOptions](../../advancedrasterizationoptions)
* class [RasterizationOptions](../../rasterizationoptions)
* namespace [GroupDocs.Redaction.Options](../../../groupdocs.redaction.options)
* assembly [GroupDocs.Redaction](../../../)

---

## AddAdvancedOption(AdvancedRasterizationOptions, Dictionary&lt;string, string&gt;) {#addadvancedoption_1}

Sie können diese Methode verwenden, um eine anzuwendende erweiterte Rasterungsoption zu registrieren.

```csharp
public void AddAdvancedOption(AdvancedRasterizationOptions optionType, 
    Dictionary<string, string> parameters)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| optionType | AdvancedRasterizationOptions | Stellt Informationen über den ausgewählten Effekttyp bereit (Graustufen, Rahmen usw.) |
| parameters | Dictionary`2 | Parameter für den angegebenen Effekt, wie z. B. Rotationswinkel |

### Beispiele

Das folgende Beispiel zeigt, wie die erweiterten Rasterisierungsoptionen mit den Standardeinstellungen angewendet werden.

```csharp
    using (Redactor redactor = new Redactor(@"C:\sample.docx"))
    {
      // Dokument mit Standardoptionen speichern (Seiten in Bilder konvertieren, als PDF speichern)
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

Das folgende Beispiel zeigt, wie die erweiterte Rasterisierungsoption für den Rand mit benutzerdefinierten Einstellungen angewendet wird.

```csharp
    using (Redactor redactor = new Redactor(@"C:\sample.docx"))
    {
      // Speichere das Dokument mit einem benutzerdefinierten Rand
      var so = new SaveOptions();
      so.Rasterization.Enabled = true;
      so.RedactedFileSuffix = "_scan";
      so.Rasterization.AddAdvancedOption(AdvancedRasterizationOptions.Border, new Dictionary<string, string>() { { "border", "10" } });
      redactor.Save(so);
    }
```

Das folgende Beispiel zeigt, wie die erweiterte Rasterisierungsoption für Rauschen mit benutzerdefinierten Einstellungen angewendet wird.

```csharp
    using (Redactor redactor = new Redactor(@"C:\sample.docx"))
    {
      // Speichern Sie das Dokument mit der benutzerdefinierten Anzahl und Größe der Rauscheffekte
      var so = new SaveOptions();
      so.Rasterization.Enabled = true;
      so.RedactedFileSuffix = "_scan";
      so.Rasterization.AddAdvancedOption(AdvancedRasterizationOptions.Noise, 
          new Dictionary<string, string>() { { "maxSpots", "150" }, { "spotMaxSize", "15" } });
      redactor.Save(so);
    }
```

Das folgende Beispiel zeigt, wie die erweiterte Rasterisierungsoption „Tilt“ mit benutzerdefinierten Einstellungen angewendet wird.

```csharp
    using (Redactor redactor = new Redactor(@"C:\sample.docx"))
    {
      // Speichern Sie das Dokument mit dem benutzerdefinierten Tilt-Effekt
      var so = new SaveOptions();
      so.Rasterization.Enabled = true;
      so.RedactedFileSuffix = "_scan";
      so.Rasterization.AddAdvancedOption(AdvancedRasterizationOptions.Tilt, 
          new Dictionary<string, string>() { { { "minAngle", "85" }, { "randomAngleMax", "5" } });
      redactor.Save(so);
    }
```

### Siehe auch

* enum [AdvancedRasterizationOptions](../../advancedrasterizationoptions)
* class [RasterizationOptions](../../rasterizationoptions)
* namespace [GroupDocs.Redaction.Options](../../../groupdocs.redaction.options)
* assembly [GroupDocs.Redaction](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Redaction.dll -->
