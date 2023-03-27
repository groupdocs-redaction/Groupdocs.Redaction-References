---
title: AddAdvancedOption
second_title: Riferimento API GroupDocs.Redaction per .NET
description: È possibile utilizzare questo metodo per registrare unopzione di rasterizzazione avanzata da applicare.
type: docs
weight: 70
url: /it/net/groupdocs.redaction.options/rasterizationoptions/addadvancedoption/
---
## AddAdvancedOption(AdvancedRasterizationOptions) {#addadvancedoption}

È possibile utilizzare questo metodo per registrare un'opzione di rasterizzazione avanzata da applicare.

```csharp
public void AddAdvancedOption(AdvancedRasterizationOptions optionType)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| optionType | AdvancedRasterizationOptions | Fornisce informazioni sul tipo di effetto selezionato (scala di grigi, bordo, ecc.) |

### Esempi

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

### Guarda anche

* enum [AdvancedRasterizationOptions](../../advancedrasterizationoptions)
* class [RasterizationOptions](../../rasterizationoptions)
* spazio dei nomi [GroupDocs.Redaction.Options](../../rasterizationoptions)
* assemblea [GroupDocs.Redaction](../../../)

---

## AddAdvancedOption(AdvancedRasterizationOptions, Dictionary&lt;string, string&gt;) {#addadvancedoption_1}

È possibile utilizzare questo metodo per registrare un'opzione di rasterizzazione avanzata da applicare.

```csharp
public void AddAdvancedOption(AdvancedRasterizationOptions optionType, 
    Dictionary<string, string> parameters)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| optionType | AdvancedRasterizationOptions | Fornisce informazioni sul tipo di effetto selezionato (scala di grigi, bordo, ecc.) |
| parameters | Dictionary`2 | Parametri per l'effetto dato, come l'angolo di rotazione |

### Esempi

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

* enum [AdvancedRasterizationOptions](../../advancedrasterizationoptions)
* class [RasterizationOptions](../../rasterizationoptions)
* spazio dei nomi [GroupDocs.Redaction.Options](../../rasterizationoptions)
* assemblea [GroupDocs.Redaction](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Redaction.dll -->
