---
title: RasterizationOptions
second_title: GroupDocs.Redaction für .NET-API-Referenz
description: Bietet Optionen zum Konvertieren von Dateien in PDF.
type: docs
weight: 350
url: /de/net/groupdocs.redaction.options/rasterizationoptions/
---
## RasterizationOptions class

Bietet Optionen zum Konvertieren von Dateien in PDF.

```csharp
public class RasterizationOptions
```

## Konstrukteure

| Name | Beschreibung |
| --- | --- |
| [RasterizationOptions](rasterizationoptions)() | Initialisiert eine neue Instanz. |

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [Compliance](../../groupdocs.redaction.options/rasterizationoptions/compliance) { get; set; } | Ruft die PDF-Konformitätsstufe ab oder legt sie fest. |
| [Enabled](../../groupdocs.redaction.options/rasterizationoptions/enabled) { get; set; } | Ruft einen Wert ab oder legt einen Wert fest, der angibt, ob alle Seiten im Dokument in Bilder konvertiert und in eine einzige PDF-Datei eingefügt werden müssen. Standardmäßig TRUE, auf FALSE gesetzt, um eine Rasterung zu vermeiden. |
| [HasAdvancedOptions](../../groupdocs.redaction.options/rasterizationoptions/hasadvancedoptions) { get; } | Ruft einen Indikator ab, der wahr ist, wenn erweiterte Rasterisierungsoptionen eingestellt sind. |
| [PageCount](../../groupdocs.redaction.options/rasterizationoptions/pagecount) { get; set; } | Ermittelt oder setzt die Anzahl der Seiten, die in PDF konvertiert werden sollen. |
| [PageIndex](../../groupdocs.redaction.options/rasterizationoptions/pageindex) { get; set; } | Ruft den Index der ersten Seite (0-basiert) ab oder legt ihn fest, die in PDF konvertiert werden soll. |

## Methoden

| Name | Beschreibung |
| --- | --- |
| [AddAdvancedOption](../../groupdocs.redaction.options/rasterizationoptions/addadvancedoption#addadvancedoption)(AdvancedRasterizationOptions) | Sie können diese Methode verwenden, um eine erweiterte Rasterungsoption für die Anwendung zu registrieren. |
| [AddAdvancedOption](../../groupdocs.redaction.options/rasterizationoptions/addadvancedoption#addadvancedoption_1)(AdvancedRasterizationOptions, Dictionary&lt;string, string&gt;) | Sie können diese Methode verwenden, um eine erweiterte Rasterungsoption für die Anwendung zu registrieren. |

### Bemerkungen

**Erfahren Sie mehr**

* Weitere Details zum Speichern des Dokuments als gerastertes PDF: [Als gerastertes PDF speichern](https://docs.groupdocs.com/redaction/net/save-in-rasterized-pdf/)
* Weitere Details zu Rasterungsoptionen: [Wählen Sie bestimmte Seiten für gerastertes PDF aus](https://docs.groupdocs.com/redaction/net/select-specific-pages-for-rasterized-pdf/)

### Beispiele

Das folgende Beispiel zeigt, wie Sie Optionen für den Rasterungsprozess festlegen.

```csharp
    using (var redactor = new Redactor("SomePresentation.pptx"))
    {
        // vertrauliche Daten auf der ersten Folie schwärzen 
    
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

* namensraum [GroupDocs.Redaction.Options](../../groupdocs.redaction.options)
* Montage [GroupDocs.Redaction](../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Redaction.dll -->
