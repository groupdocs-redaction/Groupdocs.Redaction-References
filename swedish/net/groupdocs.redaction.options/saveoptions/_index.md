---
title: "SaveOptions"
second_title: "GroupDocs.Redaction för .NET API-referens"
description: "Tillhandahåller alternativ för att ändra ett utdatafilnamn och/eller konvertera dokumentet till bildbaserad PDF-rasterisering."
type: docs
weight: 450
url: /sv/net/groupdocs.redaction.options/saveoptions/
---
## SaveOptions class

Tillhandahåller alternativ för att ändra ett utdatafilnamn och/eller konvertera dokumentet till bildbaserad PDF (rasterisering).

```csharp
public class SaveOptions
```

## Konstruktörer

| Namn | Beskrivning |
| --- | --- |
| [SaveOptions](saveoptions#constructor)() | Initierar en ny instans med standardvärden: rasterisera till PDF - falskt, lägg till suffix - falskt. |
| [SaveOptions](saveoptions#constructor_1)(bool, string) | Initierar en ny instans med angivna parametrar. |

## Egenskaper

| Namn | Beskrivning |
| --- | --- |
| [AddSuffix](../../groupdocs.redaction.options/saveoptions/addsuffix) { get; set; } | Hämtar eller anger ett värde som indikerar om filnamnet måste ändras innan sparning. Falskt som standard. |
| [Rasterization](../../groupdocs.redaction.options/saveoptions/rasterization) { get; } | Hämtar rasteriseringsinställningarna. |
| [RasterizeToPDF](../../groupdocs.redaction.options/saveoptions/rasterizetopdf) { get; set; } | Hämtar eller anger ett värde som indikerar om alla sidor i dokumentet ska konverteras till bilder och placeras i en enda PDF-fil. |
| [RedactedFileSuffix](../../groupdocs.redaction.options/saveoptions/redactedfilesuffix) { get; set; } | Hämtar eller anger ett anpassat suffix för utdatafilens namn. Om det inte anges används konstanten [`SaveSuffix`](./savesuffix). |
| [WordprocessingSaveOptions](../../groupdocs.redaction.options/saveoptions/wordprocessingsaveoptions) { get; } | Hämtar sparalternativen som är specifika för ordbehandlingsdokument. |

## Fält

| Namn | Beskrivning |
| --- | --- |
| const [SaveSuffix](../../groupdocs.redaction.options/saveoptions/savesuffix) | Representerar standardvärdet för suffix, som är "Redacted". |

### Anmärkningar

**Learn more**

* [Save with default options](https://docs.groupdocs.com/redaction/net/save-with-default-options/)
* [Save in rasterized PDF](https://docs.groupdocs.com/redaction/net/save-in-rasterized-pdf/)
* [Select specific pages for rasterized PDF](https://docs.groupdocs.com/redaction/net/select-specific-pages-for-rasterized-pdf/)
* [Save in original format](https://docs.groupdocs.com/redaction/net/save-in-original-format/)
* [Save overwriting original file](https://docs.groupdocs.com/redaction/net/save-overwriting-original-file/)
* [Save to stream](https://docs.groupdocs.com/redaction/net/save-to-stream/)

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

* namespace [GroupDocs.Redaction.Options](../../groupdocs.redaction.options)
* assembly [GroupDocs.Redaction](../../)

<!-- GÅ INTE ATT REDIGERA: genererad av xmldocmd för GroupDocs.Redaction.dll -->
