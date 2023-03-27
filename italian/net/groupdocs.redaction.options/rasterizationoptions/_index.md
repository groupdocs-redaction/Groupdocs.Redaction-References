---
title: RasterizationOptions
second_title: Riferimento API GroupDocs.Redaction per .NET
description: Fornisce opzioni per convertire i file in PDF.
type: docs
weight: 350
url: /it/net/groupdocs.redaction.options/rasterizationoptions/
---
## RasterizationOptions class

Fornisce opzioni per convertire i file in PDF.

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
| [Enabled](../../groupdocs.redaction.options/rasterizationoptions/enabled) { get; set; } | Ottiene o imposta un valore che indica se tutte le pagine del documento devono essere convertite in immagini e inserite in un unico file PDF. TRUE per impostazione predefinita, impostato su FALSE per evitare la rasterizzazione. |
| [HasAdvancedOptions](../../groupdocs.redaction.options/rasterizationoptions/hasadvancedoptions) { get; } | Ottiene un indicatore, che è vero se sono impostate opzioni di rasterizzazione avanzate. |
| [PageCount](../../groupdocs.redaction.options/rasterizationoptions/pagecount) { get; set; } | Ottiene o imposta il numero di pagine da convertire in PDF. |
| [PageIndex](../../groupdocs.redaction.options/rasterizationoptions/pageindex) { get; set; } | Ottiene o imposta l'indice della prima pagina (in base 0) da convertire in PDF. |

## Metodi

| Nome | Descrizione |
| --- | --- |
| [AddAdvancedOption](../../groupdocs.redaction.options/rasterizationoptions/addadvancedoption#addadvancedoption)(AdvancedRasterizationOptions) | È possibile utilizzare questo metodo per registrare un'opzione di rasterizzazione avanzata da applicare. |
| [AddAdvancedOption](../../groupdocs.redaction.options/rasterizationoptions/addadvancedoption#addadvancedoption_1)(AdvancedRasterizationOptions, Dictionary&lt;string, string&gt;) | È possibile utilizzare questo metodo per registrare un'opzione di rasterizzazione avanzata da applicare. |

### Osservazioni

**Saperne di più**

* Ulteriori dettagli sul salvataggio del documento come PDF rasterizzato: [Salva in PDF rasterizzato](https://docs.groupdocs.com/redaction/net/save-in-rasterized-pdf/)
* Maggiori dettagli sulle opzioni di rasterizzazione: [Seleziona pagine specifiche per PDF rasterizzati](https://docs.groupdocs.com/redaction/net/select-specific-pages-for-rasterized-pdf/)

### Esempi

L'esempio seguente mostra come impostare le opzioni per il processo di rasterizzazione.

```csharp
    using (var redactor = new Redactor("SomePresentation.pptx"))
    {
        // oscura i dati sensibili nella prima diapositiva 
    
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

L'esempio seguente mostra come applicare le opzioni di rasterizzazione avanzate con le impostazioni predefinite.

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

L'esempio seguente mostra come applicare l'opzione di rasterizzazione avanzata del bordo con impostazioni personalizzate.

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

L'esempio seguente mostra come applicare l'opzione di rasterizzazione avanzata del rumore con impostazioni personalizzate.

```csharp
    using (Redactor redactor = new Redactor(@"C:\sample.docx"))
    {
      // Salva il documento con il numero e la dimensione personalizzati degli effetti di disturbo
      var so = new SaveOptions();
      so.Rasterization.Enabled = true;
      so.RedactedFileSuffix = "_scan";
      so.Rasterization.AddAdvancedOption(AdvancedRasterizationOptions.Noise, 
          new Dictionary<string, string>() { { "maxSpots", "150" }, { "spotMaxSize", "15" } });
      redactor.Save(so);
    }
```

L'esempio seguente mostra come applicare l'opzione di rasterizzazione avanzata tilt con impostazioni personalizzate.

```csharp
    using (Redactor redactor = new Redactor(@"C:\sample.docx"))
    {
      // Salva il documento con l'effetto di inclinazione personalizzato
      var so = new SaveOptions();
      so.Rasterization.Enabled = true;
      so.RedactedFileSuffix = "_scan";
      so.Rasterization.AddAdvancedOption(AdvancedRasterizationOptions.Tilt, 
          new Dictionary<string, string>() { { { "minAngle", "85" }, { "randomAngleMax", "5" } });
      redactor.Save(so);
    }
```

### Guarda anche

* spazio dei nomi [GroupDocs.Redaction.Options](../../groupdocs.redaction.options)
* assemblea [GroupDocs.Redaction](../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Redaction.dll -->
