---
title: "RasterizationOptions"
second_title: "GroupDocs.Redaction für .NET API-Referenz"
description: "Stellt Optionen zum Konvertieren von Dateien in PDF bereit."
type: docs
weight: 420
url: /de/net/groupdocs.redaction.options/rasterizationoptions/
---
## RasterizationOptions class

Stellt Optionen zum Konvertieren von Dateien in PDF bereit.

```csharp
public class RasterizationOptions
```

## Konstruktoren

| Name | Beschreibung |
| --- | --- |
| [RasterizationOptions](rasterizationoptions)() | Initialisiert eine neue Instanz. |

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [Compliance](../../groupdocs.redaction.options/rasterizationoptions/compliance) { get; set; } | Liest oder setzt das PDF-Konformitätsniveau. |
| [Enabled](../../groupdocs.redaction.options/rasterizationoptions/enabled) { get; set; } | Liest oder setzt einen Wert, der angibt, ob alle Seiten im Dokument in Bilder konvertiert und in einer einzigen PDF-Datei zusammengefasst werden sollen. Standardmäßig TRUE, auf FALSE setzen, um die Rasterung zu vermeiden. |
| [HasAdvancedOptions](../../groupdocs.redaction.options/rasterizationoptions/hasadvancedoptions) { get; } | Liest einen Indikator, der true ist, wenn erweiterte Rasterungsoptionen festgelegt sind. |
| [PageCount](../../groupdocs.redaction.options/rasterizationoptions/pagecount) { get; set; } | Liest oder setzt die Anzahl der Seiten, die in PDF konvertiert werden sollen. |
| [PageIndex](../../groupdocs.redaction.options/rasterizationoptions/pageindex) { get; set; } | Liest oder setzt den Index der ersten Seite (0-basiert), die in PDF konvertiert werden soll. |

## Methoden

| Name | Beschreibung |
| --- | --- |
| [AddAdvancedOption](../../groupdocs.redaction.options/rasterizationoptions/addadvancedoption#addadvancedoption)(AdvancedRasterizationOptions) | Sie können diese Methode verwenden, um eine anzuwendende erweiterte Rasterungsoption zu registrieren. |
| [AddAdvancedOption](../../groupdocs.redaction.options/rasterizationoptions/addadvancedoption#addadvancedoption_1)(AdvancedRasterizationOptions, Dictionary&lt;string, string&gt;) | Sie können diese Methode verwenden, um eine anzuwendende erweiterte Rasterungsoption zu registrieren. |

### Hinweise

**Learn more**

* More details about saving document as a rasterized PDF: [Save in rasterized PDF](https://docs.groupdocs.com/redaction/net/save-in-rasterized-pdf/)
* More details about rasterization options: [Select specific pages for rasterized PDF](https://docs.groupdocs.com/redaction/net/select-specific-pages-for-rasterized-pdf/)

### Beispiele

Das folgende Beispiel zeigt, wie Optionen für den Rasterungsprozess festgelegt werden.

```csharp
    using (var redactor = new Redactor("SomePresentation.pptx"))
    {
        // sensiblen Daten auf der ersten Folie redigieren 
    
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

* namespace [GroupDocs.Redaction.Options](../../groupdocs.redaction.options)
* assembly [GroupDocs.Redaction](../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Redaction.dll -->
