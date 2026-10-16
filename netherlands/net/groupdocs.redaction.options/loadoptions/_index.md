---
title: "LoadOptions"
second_title: "GroupDocs.Redaction voor .NET API-referentie"
description: "Biedt opties die worden gebruikt om een bestand te openen."
type: docs
weight: 380
url: /nl/net/groupdocs.redaction.options/loadoptions/
---
## LoadOptions class

Biedt opties die worden gebruikt om een bestand te openen.

```csharp
public class LoadOptions
```

## Constructors

| Naam | Beschrijving |
| --- | --- |
| [LoadOptions](loadoptions#constructor)() | Initialiseert een nieuw exemplaar van de LoadOptions-klasse. |
| [LoadOptions](loadoptions#constructor_1)(bool) | Initialiseert een nieuw exemplaar van de LoadOptions-klasse met de opgegeven pre-rasterisatievlag. |
| [LoadOptions](loadoptions#constructor_2)(FileType) | Initialiseert een nieuw exemplaar van de LoadOptions-klasse met het opgegeven bestandstype. |
| [LoadOptions](loadoptions#constructor_3)(string) | Initialiseert een nieuw exemplaar van de LoadOptions-klasse met een opgegeven wachtwoord. |
| [LoadOptions](loadoptions#constructor_4)(string, bool) | Initialiseert een nieuw exemplaar van de LoadOptions-klasse met een opgegeven wachtwoord. |

## Properties

| Naam | Beschrijving |
| --- | --- |
| [FileType](../../groupdocs.redaction.options/loadoptions/filetype) { get; set; } | Haalt op of stelt het type van het te openen bestand in. |
| [Password](../../groupdocs.redaction.options/loadoptions/password) { get; set; } | Haalt op of stelt een wachtwoord in voor met wachtwoord beveiligde documenten. |
| [PreRasterize](../../groupdocs.redaction.options/loadoptions/prerasterize) { get; set; } | Haalt op of stelt een waarde in die aangeeft of het bestand vooraf moet worden gerasterd. |

### Opmerkingen

**Learn more**

* [Loading documents](https://docs.groupdocs.com/redaction/net/loading-documents/)
* [Load from local disk](https://docs.groupdocs.com/redaction/net/load-from-local-disc/)
* [Load from stream](https://docs.groupdocs.com/redaction/net/load-from-stream/)
* [Load password-protected document](https://docs.groupdocs.com/redaction/net/load-password-protected-file/)

### Voorbeelden

Het volgende voorbeeld laat zien hoe een met wachtwoord beveiligd document te openen.

```csharp
LoadOptions loadOptions = new LoadOptions("mysecretpassword");
using (var redactor = new Redactor("PasswordProtected.pdf", loadOptions))
{
    // werken met document
}
```

### Zie ook

* namespace [GroupDocs.Redaction.Options](../../groupdocs.redaction.options)
* assembly [GroupDocs.Redaction](../../)

<!-- NIET BEWERKEN: gegenereerd door xmldocmd voor GroupDocs.Redaction.dll -->
