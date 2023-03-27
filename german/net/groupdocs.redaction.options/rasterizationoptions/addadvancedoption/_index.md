---
title: AddAdvancedOption
second_title: GroupDocs.Redaction für .NET-API-Referenz
description: Sie können diese Methode verwenden um eine erweiterte Rasterungsoption für die Anwendung zu registrieren.
type: docs
weight: 70
url: /de/net/groupdocs.redaction.options/rasterizationoptions/addadvancedoption/
---
## AddAdvancedOption(AdvancedRasterizationOptions) {#addadvancedoption}

Sie können diese Methode verwenden, um eine erweiterte Rasterungsoption für die Anwendung zu registrieren.

```csharp
public void AddAdvancedOption(AdvancedRasterizationOptions optionType)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| optionType | AdvancedRasterizationOptions | Liefert Informationen über den ausgewählten Effekttyp (Graustufen, Rand usw.) |

### Beispiele

Das folgende Beispiel zeigt, wie die erweiterten Rasterungsoptionen mit Standardeinstellungen angewendet werden.

```csharp
    using (Redactor redactor = new Redactor(@"C:\sample.docx"))
    {
      // Dokument mit Standardoptionen speichern (Seiten in Bilder umwandeln, als PDF speichern)
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
* namensraum [GroupDocs.Redaction.Options](../../rasterizationoptions)
* Montage [GroupDocs.Redaction](../../../)

---

## AddAdvancedOption(AdvancedRasterizationOptions, Dictionary&lt;string, string&gt;) {#addadvancedoption_1}

Sie können diese Methode verwenden, um eine erweiterte Rasterungsoption für die Anwendung zu registrieren.

```csharp
public void AddAdvancedOption(AdvancedRasterizationOptions optionType, 
    Dictionary<string, string> parameters)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| optionType | AdvancedRasterizationOptions | Liefert Informationen über den ausgewählten Effekttyp (Graustufen, Rand usw.) |
| parameters | Dictionary`2 | Parameter für den jeweiligen Effekt, z. B. Drehwinkel |

### Beispiele

Das folgende Beispiel zeigt, wie die erweiterten Rasterungsoptionen mit Standardeinstellungen angewendet werden.

```csharp
    using (Redactor redactor = new Redactor(@"C:\sample.docx"))
    {
      // Dokument mit Standardoptionen speichern (Seiten in Bilder umwandeln, als PDF speichern)
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

Das folgende Beispiel zeigt, wie Sie die Option „Erweiterte Randrasterung“ mit benutzerdefinierten Einstellungen anwenden.

```csharp
    using (Redactor redactor = new Redactor(@"C:\sample.docx"))
    {
      // Speichern Sie das Dokument mit einem benutzerdefinierten Rahmen
      var so = new SaveOptions();
      so.Rasterization.Enabled = true;
      so.RedactedFileSuffix = "_scan";
      so.Rasterization.AddAdvancedOption(AdvancedRasterizationOptions.Border, new Dictionary<string, string>() { { "border", "10" } });
      redactor.Save(so);
    }
```

Das folgende Beispiel zeigt, wie Sie die erweiterte Rasterungsoption „Rauschen“ mit benutzerdefinierten Einstellungen anwenden.

```csharp
    using (Redactor redactor = new Redactor(@"C:\sample.docx"))
    {
      // Speichern Sie das Dokument mit der benutzerdefinierten Anzahl und Größe von Rauscheffekten
      var so = new SaveOptions();
      so.Rasterization.Enabled = true;
      so.RedactedFileSuffix = "_scan";
      so.Rasterization.AddAdvancedOption(AdvancedRasterizationOptions.Noise, 
          new Dictionary<string, string>() { { "maxSpots", "150" }, { "spotMaxSize", "15" } });
      redactor.Save(so);
    }
```

Das folgende Beispiel zeigt, wie Sie die erweiterte Rasterungsoption Neigung mit benutzerdefinierten Einstellungen anwenden.

```csharp
    using (Redactor redactor = new Redactor(@"C:\sample.docx"))
    {
      // Speichern Sie das Dokument mit dem benutzerdefinierten Neigungseffekt
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
* namensraum [GroupDocs.Redaction.Options](../../rasterizationoptions)
* Montage [GroupDocs.Redaction](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Redaction.dll -->
