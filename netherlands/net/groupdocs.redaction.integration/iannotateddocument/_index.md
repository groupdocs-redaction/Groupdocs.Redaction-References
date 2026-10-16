---
title: "IAnnotatedDocument"
second_title: "GroupDocs.Redaction voor .NET API-referentie"
description: "Definieert methoden die vereist zijn voor toegang tot annotaties zoals opmerkingen. Moet worden geïmplementeerd door DocumentFormatInstance./documentformatinstancederived klasse om annotatie‑redacties uit te voeren."
type: docs
weight: 120
url: /nl/net/groupdocs.redaction.integration/iannotateddocument/
---
## IAnnotatedDocument interface

Definieert methoden die vereist zijn voor toegang tot annotaties, zoals opmerkingen. Moet worden geïmplementeerd door [`DocumentFormatInstance`](../documentformatinstance)-afgeleide klasse om annotatie‑redacties uit te voeren.

```csharp
public interface IAnnotatedDocument
```

## Methoden

| Naam | Beschrijving |
| --- | --- |
| [DeleteAnnotations](../../groupdocs.redaction.integration/iannotateddocument/deleteannotations)(Regex) | Verwijdert alle annotaties die overeenkomen met een reguliere expressie binnen het document. |
| [RedactAnnotation](../../groupdocs.redaction.integration/iannotateddocument/redactannotation)(Regex, string) | Vervangt de overeenkomende tekst in alle annotaties binnen het document. |

### Opmerkingen

**Learn more**

* More details about applying redactions: [Redaction basics](https://docs.groupdocs.com/redaction/net/redaction-basics/)
* More details about document annotation redactions: [Annotation redactions](https://docs.groupdocs.com/redaction/net/annotation-redactions/)
* More details about implementing custom formats: [Create custom format handler](https://docs.groupdocs.com/redaction/net/create-custom-format-handler/)

### Zie ook

* namespace [GroupDocs.Redaction.Integration](../../groupdocs.redaction.integration)
* assembly [GroupDocs.Redaction](../../)

<!-- NIET BEWERKEN: gegenereerd door xmldocmd voor GroupDocs.Redaction.dll -->
