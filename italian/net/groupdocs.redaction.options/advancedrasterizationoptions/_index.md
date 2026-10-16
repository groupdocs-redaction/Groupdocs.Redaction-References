---
title: "AdvancedRasterizationOptions"
second_title: "Riferimento API di GroupDocs.Redaction per .NET"
description: "Enumerazione di flag per gestire le opzioni avanzate di rasterizzazione da applicare."
type: docs
weight: 290
url: /it/net/groupdocs.redaction.options/advancedrasterizationoptions/
---
## AdvancedRasterizationOptions enumeration

Enumerazione di flag per gestire le opzioni avanzate di rasterizzazione da applicare.

```csharp
public enum AdvancedRasterizationOptions
```

### Valori

| Nome | Valore | Descrizione |
| --- | --- | --- |
| None | `0` | Nessuna opzione avanzata da applicare. |
| Tilt | `1` | Inclina l'immagine rasterizzata a un angolo casuale. |
| Noise | `2` | Aggiungi macchie casuali alle immagini delle pagine rasterizzate. |
| Border | `4` | Aggiungi una linea di bordo per imitare l'effetto di scansione della pagina. |
| Grayscale | `8` | Rendi le immagini delle pagine in scala di grigi per imitare una scansione in scala di grigi. |

### Esempi

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
