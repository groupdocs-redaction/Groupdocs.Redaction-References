---
title: "Opslaan"
second_title: "GroupDocs.Redaction voor .NET API-referentie"
description: "Slaat het document op in een bestand met de volgende opties AddSuffix  true RasterizeToPDF  true."
type: docs
weight: 60
url: /nl/net/groupdocs.redaction/redactor/save/
---
## Save() {#save}

Slaat het document op in een bestand met de volgende opties: AddSuffix = true, RasterizeToPDF = true.

```csharp
public string Save()
```

### Retourwaarde

Pad naar geredigeerd document

### Zie ook

* class [Redactor](../../redactor)
* namespace [GroupDocs.Redaction](../../../groupdocs.redaction)
* assembly [GroupDocs.Redaction](../../../)

---

## Save(SaveOptions) {#save_1}

Slaat het document op in een bestand.

```csharp
public string Save(SaveOptions saveOptions)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| saveOptions | SaveOptions | Opties om een achtervoegsel toe te voegen of te rasteren |

### Retourwaarde

Pad naar geredigeerd document

### Voorbeelden

Het volgende voorbeeld laat zien hoe een document op te slaan met SaveOptions.

```csharp
    using (Redactor redactor = new Redactor(@"C:\sample.pdf"))
    {
       // Documentredactie komt hier
       // ...
    
       // Sla het document op met standaardopties (converteer pagina's naar afbeeldingen, sla op als PDF)
       redactor.Save();
    
       // Sla het document op in het oorspronkelijke formaat en overschrijf het originele bestand
       redactor.Save(new SaveOptions() { AddSuffix = false, RasterizeToPDF = false });
    
       // Sla het document op naar een \"*_Redacted.*\" bestand in het oorspronkelijke formaat
       redactor.Save(new SaveOptions() { AddSuffix = true, RasterizeToPDF = false });
    
       // Sla het document op naar \"*_AnyText.*\" (bijv. tijdstempel in plaats van \"AnyText\") in de bestandsnaam zonder rasterisatie
       redactor.Save(new SaveOptions(false, "AnyText"));
    }    
```

### Zie ook

* class [SaveOptions](../../../groupdocs.redaction.options/saveoptions)
* class [Redactor](../../redactor)
* namespace [GroupDocs.Redaction](../../../groupdocs.redaction)
* assembly [GroupDocs.Redaction](../../../)

---

## Save(Stream, SaveOptions) {#save_3}

Slaat het document op in de opgegeven stream.

```csharp
public void Save(Stream document, SaveOptions saveOptions)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| document | Stream | De doelstroom. |
| saveOptions | SaveOptions | De opslagopties die rasterisatie regelen, het achtervoegsel van de bestandsnaam en document-specifieke opslaginstellingen. |

### Zie ook

* class [SaveOptions](../../../groupdocs.redaction.options/saveoptions)
* class [Redactor](../../redactor)
* namespace [GroupDocs.Redaction](../../../groupdocs.redaction)
* assembly [GroupDocs.Redaction](../../../)

<!-- NIET BEWERKEN: gegenereerd door xmldocmd voor GroupDocs.Redaction.dll -->
