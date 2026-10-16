---
title: "AddAdvancedOption"
second_title: "Riferimento API di GroupDocs.Redaction per .NET"
description: "È possibile utilizzare questo metodo per registrare un'opzione avanzata di rasterizzazione da applicare."
type: docs
weight: 70
url: /it/net/groupdocs.redaction.options/rasterizationoptions/addadvancedoption/
---
## AddAdvancedOption(AdvancedRasterizationOptions) {#addadvancedoption}

È possibile utilizzare questo metodo per registrare un'opzione avanzata di rasterizzazione da applicare.

```csharp
public void AddAdvancedOption(AdvancedRasterizationOptions optionType)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| optionType | AdvancedRasterizationOptions | Fornisce informazioni sul tipo di effetto selezionato (scala di grigi, bordo, ecc.) |

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

### Vedi anche

* enum [AdvancedRasterizationOptions](../../advancedrasterizationoptions)
* class [RasterizationOptions](../../rasterizationoptions)
* namespace [GroupDocs.Redaction.Options](../../../groupdocs.redaction.options)
* assembly [GroupDocs.Redaction](../../../)

---

## AddAdvancedOption(AdvancedRasterizationOptions, Dictionary&lt;string, string&gt;) {#addadvancedoption_1}

È possibile utilizzare questo metodo per registrare un'opzione avanzata di rasterizzazione da applicare.

```csharp
public void AddAdvancedOption(AdvancedRasterizationOptions optionType, 
    Dictionary<string, string> parameters)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| optionType | AdvancedRasterizationOptions | Fornisce informazioni sul tipo di effetto selezionato (scala di grigi, bordo, ecc.) |
| parameters | Dictionary`2 | Parametri per l'effetto specificato, come l'angolo di rotazione |

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

* enum [AdvancedRasterizationOptions](../../advancedrasterizationoptions)
* class [RasterizationOptions](../../rasterizationoptions)
* namespace [GroupDocs.Redaction.Options](../../../groupdocs.redaction.options)
* assembly [GroupDocs.Redaction](../../../)

<!-- NON MODIFICARE: generato da xmldocmd per GroupDocs.Redaction.dll -->
