---
title: "IFixedFormatDocument"
second_title: "GroupDocs.Redaction voor .NET API-referentie"
description: "Definieert methoden die vereist zijn voor toegangsformaten met een vaste structuur, zoals PDF of presentaties."
type: docs
weight: 140
url: /nl/net/groupdocs.redaction.integration/ifixedformatdocument/
---
## IFixedFormatDocument interface

Definieert methoden die vereist zijn voor toegang tot formaten met een vaste structuur, zoals PDF of presentaties.

```csharp
public interface IFixedFormatDocument
```

## Methoden

| Naam | Beschrijving |
| --- | --- |
| [LoadImages](../../groupdocs.redaction.integration/ifixedformatdocument/loadimages)(RedactionFilter[]) | Laadt een array van raster‑afbeeldingsinstanties, die zich in het document bevinden, overeenkomend met de [`RedactionFilter`](../../groupdocs.redaction.redactions/redactionfilter)-set. |
| [RedactAnnotation](../../groupdocs.redaction.integration/ifixedformatdocument/redactannotation)(Regex, ReplacementOptions) | Vervangt de overeenkomende tekst in alle annotaties binnen het document met de opgegeven opties. |

### Opmerkingen

**Learn more**

* More details about applying redactions: [Redaction basics](https://docs.groupdocs.com/redaction/net/redaction-basics/)
* More details about PageAreaRedaction: [Use PageAreaRedaction](https://docs.groupdocs.com/redaction/net/use-page-area-redaction/)
* More details about implementing custom formats: [Create custom format handler](https://docs.groupdocs.com/redaction/net/create-custom-format-handler/)

### Zie ook

* namespace [GroupDocs.Redaction.Integration](../../groupdocs.redaction.integration)
* assembly [GroupDocs.Redaction](../../)

<!-- NIET BEWERKEN: gegenereerd door xmldocmd voor GroupDocs.Redaction.dll -->
