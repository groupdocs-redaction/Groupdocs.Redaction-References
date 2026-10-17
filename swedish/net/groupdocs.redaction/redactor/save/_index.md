---
title: "Save"
second_title: "GroupDocs.Redaction för .NET API-referens"
description: "Sparar dokumentet till en fil med följande alternativ AddSuffix  true RasterizeToPDF  true."
type: docs
weight: 60
url: /sv/net/groupdocs.redaction/redactor/save/
---
## Save() {#save}

Sparar dokumentet till en fil med följande alternativ: AddSuffix = true, RasterizeToPDF = true.

```csharp
public string Save()
```

### Returvärde

Sökväg till redigerat dokument

### Se även

* class [Redactor](../../redactor)
* namespace [GroupDocs.Redaction](../../../groupdocs.redaction)
* assembly [GroupDocs.Redaction](../../../)

---

## Save(SaveOptions) {#save_1}

Sparar dokumentet till en fil.

```csharp
public string Save(SaveOptions saveOptions)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| saveOptions | SaveOptions | Alternativ för att lägga till suffix eller rasterisera |

### Returvärde

Sökväg till redigerat dokument

### Exempel

Följande exempel visar hur man sparar ett dokument med SaveOptions.

```csharp
    using (Redactor redactor = new Redactor(@"C:\sample.pdf"))
    {
       // Dokumentredigering sker här
       // ...
    
       // Spara dokumentet med standardalternativ (konvertera sidor till bilder, spara som PDF)
       redactor.Save();
    
       // Spara dokumentet i originalformat och skriv över originalfilen
       redactor.Save(new SaveOptions() { AddSuffix = false, RasterizeToPDF = false });
    
       // Spara dokumentet till filen "*_Redacted.*" i originalformat
       redactor.Save(new SaveOptions() { AddSuffix = true, RasterizeToPDF = false });
    
       // Spara dokumentet till "*_AnyText.*" (t.ex. tidsstämpel istället för "AnyText") i filnamnet utan rasterisering
       redactor.Save(new SaveOptions(false, "AnyText"));
    }    
```

### Se även

* class [SaveOptions](../../../groupdocs.redaction.options/saveoptions)
* class [Redactor](../../redactor)
* namespace [GroupDocs.Redaction](../../../groupdocs.redaction)
* assembly [GroupDocs.Redaction](../../../)

---

## Save(Stream, SaveOptions) {#save_3}

Sparar dokumentet till den angivna strömmen.

```csharp
public void Save(Stream document, SaveOptions saveOptions)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| dokument | Stream | Målsströmmen. |
| saveOptions | SaveOptions | Sparaalternativen som styr rasterisering, suffix för utdatafilens namn och dokumentspecifika sparinställningar. |

### Se även

* class [SaveOptions](../../../groupdocs.redaction.options/saveoptions)
* class [Redactor](../../redactor)
* namespace [GroupDocs.Redaction](../../../groupdocs.redaction)
* assembly [GroupDocs.Redaction](../../../)

<!-- GÅ INTE ATT REDIGERA: genererad av xmldocmd för GroupDocs.Redaction.dll -->
