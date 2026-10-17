---
title: "LoadOptions"
second_title: "GroupDocs.Redaction för .NET API-referens"
description: "Tillhandahåller alternativ som kommer att användas för att öppna en fil."
type: docs
weight: 380
url: /sv/net/groupdocs.redaction.options/loadoptions/
---
## LoadOptions class

Tillhandahåller alternativ som kommer att användas för att öppna en fil.

```csharp
public class LoadOptions
```

## Konstruktörer

| Namn | Beskrivning |
| --- | --- |
| [LoadOptions](loadoptions#constructor)() | Initierar en ny instans av LoadOptions-klassen. |
| [LoadOptions](loadoptions#constructor_1)(bool) | Initierar en ny instans av LoadOptions-klassen med angivet förrasteriseringsflagga. |
| [LoadOptions](loadoptions#constructor_2)(FileType) | Initierar en ny instans av LoadOptions-klassen med den angivna filtypen. |
| [LoadOptions](loadoptions#constructor_3)(string) | Initierar en ny instans av LoadOptions-klassen med angivet lösenord. |
| [LoadOptions](loadoptions#constructor_4)(string, bool) | Initierar en ny instans av LoadOptions-klassen med angivet lösenord. |

## Egenskaper

| Namn | Beskrivning |
| --- | --- |
| [FileType](../../groupdocs.redaction.options/loadoptions/filetype) { get; set; } | Hämtar eller anger filtypen att öppna. |
| [Password](../../groupdocs.redaction.options/loadoptions/password) { get; set; } | Hämtar eller anger ett lösenord för lösenordsskyddade dokument. |
| [PreRasterize](../../groupdocs.redaction.options/loadoptions/prerasterize) { get; set; } | Hämtar eller anger ett värde som indikerar om filen ska för-rasteriseras. |

### Anmärkningar

**Learn more**

* [Loading documents](https://docs.groupdocs.com/redaction/net/loading-documents/)
* [Load from local disk](https://docs.groupdocs.com/redaction/net/load-from-local-disc/)
* [Load from stream](https://docs.groupdocs.com/redaction/net/load-from-stream/)
* [Load password-protected document](https://docs.groupdocs.com/redaction/net/load-password-protected-file/)

### Exempel

Följande exempel visar hur man öppnar ett lösenordsskyddat dokument.

```csharp
LoadOptions loadOptions = new LoadOptions("mysecretpassword");
using (var redactor = new Redactor("PasswordProtected.pdf", loadOptions))
{
    // arbeta med dokument
}
```

### Se även

* namespace [GroupDocs.Redaction.Options](../../groupdocs.redaction.options)
* assembly [GroupDocs.Redaction](../../)

<!-- GÅ INTE ATT REDIGERA: genererad av xmldocmd för GroupDocs.Redaction.dll -->
