---
title: "RasterizationOptions"
second_title: "Riferimento API di GroupDocs.Redaction per .NET"
description: "Fornisce le opzioni per convertire i file in PDF."
type: docs
weight: 420
url: /it/net/groupdocs.redaction.options/rasterizationoptions/
---
## RasterizationOptions class

Fornisce le opzioni per convertire i file in PDF.

```csharp
public class RasterizationOptions
```

## Costruttori

| Nome | Descrizione |
| --- | --- |
| [RasterizationOptions](rasterizationoptions)() | Inizializza una nuova istanza. |

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [Compliance](../../groupdocs.redaction.options/rasterizationoptions/compliance) { get; set; } | Ottiene o imposta il livello di conformità PDF. |
| [Enabled](../../groupdocs.redaction.options/rasterizationoptions/enabled) { get; set; } | Ottiene o imposta un valore che indica se tutte le pagine del documento devono essere convertite in immagini e inserite in un unico file PDF. TRUE per impostazione predefinita, impostare FALSE per evitare la rasterizzazione. |
| [HasAdvancedOptions](../../groupdocs.redaction.options/rasterizationoptions/hasadvancedoptions) { get; } | Ottiene un indicatore, che è true se le opzioni avanzate di rasterizzazione sono impostate. |
| [PageCount](../../groupdocs.redaction.options/rasterizationoptions/pagecount) { get; set; } | Ottiene o imposta il numero di pagine da convertire in PDF. |
| [PageIndex](../../groupdocs.redaction.options/rasterizationoptions/pageindex) { get; set; } | Ottiene o imposta l'indice della prima pagina (basato su 0) da convertire in PDF. |

## Metodi

| Nome | Descrizione |
| --- | --- |
| [AddAdvancedOption](../../groupdocs.redaction.options/rasterizationoptions/addadvancedoption#addadvancedoption)(AdvancedRasterizationOptions) | È possibile utilizzare questo metodo per registrare un'opzione avanzata di rasterizzazione da applicare. |
| [AddAdvancedOption](../../groupdocs.redaction.options/rasterizationoptions/addadvancedoption#addadvancedoption_1)(AdvancedRasterizationOptions, Dictionary&lt;string, string&gt;) | È possibile utilizzare questo metodo per registrare un'opzione avanzata di rasterizzazione da applicare. |

### Osservazioni

**Learn more**

* More details about saving document as a rasterized PDF: [Save in rasterized PDF](https://docs.groupdocs.com/redaction/net/save-in-rasterized-pdf/)
* More details about rasterization options: [Select specific pages for rasterized PDF](https://docs.groupdocs.com/redaction/net/select-specific-pages-for-rasterized-pdf/)

### Esempi

Il seguente esempio dimostra come impostare le opzioni per il processo di rasterizzazione.

```csharp
    using (var redactor = new Redactor("SomePresentation.pptx"))
    {
        // censura dati sensibili nella prima diapositiva 
    
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

Il seguente esempio dimostra come applicare le opzioni di rasterizzazione avanzata con le impostazioni predefinite.

```csharp
    using (Redactor redactor = new Redactor(@"C:\sample.docx"))
    {
      // Salva il documento con le opzioni predefinite (converti le pagine in immagini, salva come PDF)
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

Il seguente esempio dimostra come applicare l'opzione di rasterizzazione avanzata del bordo con impostazioni personalizzate.

```csharp
    using (Redactor redactor = new Redactor(@"C:\sample.docx"))
    {
      // Salva il documento con un bordo personalizzato
      var so = new SaveOptions();
      so.Rasterization.Enabled = true;
      so.RedactedFileSuffix = "_scan";
      so.Rasterization.AddAdvancedOption(AdvancedRasterizationOptions.Border, new Dictionary<string, string>() { { "border", "10" } });
      redactor.Save(so);
    }
```

Il seguente esempio dimostra come applicare l'opzione di rasterizzazione avanzata del rumore con impostazioni personalizzate.

```csharp
    using (Redactor redactor = new Redactor(@"C:\sample.docx"))
    {
      // Salva il documento con il numero e le dimensioni personalizzate degli effetti di rumore
      var so = new SaveOptions();
      so.Rasterization.Enabled = true;
      so.RedactedFileSuffix = "_scan";
      so.Rasterization.AddAdvancedOption(AdvancedRasterizationOptions.Noise, 
          new Dictionary<string, string>() { { "maxSpots", "150" }, { "spotMaxSize", "15" } });
      redactor.Save(so);
    }
```

Il seguente esempio dimostra come applicare l'opzione di rasterizzazione avanzata tilt con impostazioni personalizzate.

```csharp
    using (Redactor redactor = new Redactor(@"C:\sample.docx"))
    {
      // Salva il documento con l'effetto tilt personalizzato
      var so = new SaveOptions();
      so.Rasterization.Enabled = true;
      so.RedactedFileSuffix = "_scan";
      so.Rasterization.AddAdvancedOption(AdvancedRasterizationOptions.Tilt, 
          new Dictionary<string, string>() { { { "minAngle", "85" }, { "randomAngleMax", "5" } });
      redactor.Save(so);
    }
```

### Vedi anche

* namespace [GroupDocs.Redaction.Options](../../groupdocs.redaction.options)
* assembly [GroupDocs.Redaction](../../)

<!-- NON MODIFICARE: generato da xmldocmd per GroupDocs.Redaction.dll -->
