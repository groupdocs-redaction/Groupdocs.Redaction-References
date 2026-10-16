---
title: "IFixedFormatDocument"
second_title: "Référence API de GroupDocs.Redaction pour .NET"
description: "Définit les méthodes requises pour accéder aux formats à structure fixe tels que PDF ou les présentations."
type: docs
weight: 140
url: /fr/net/groupdocs.redaction.integration/ifixedformatdocument/
---
## IFixedFormatDocument interface

Définit les méthodes nécessaires pour accéder aux formats à structure fixe, tels que PDF ou les présentations.

```csharp
public interface IFixedFormatDocument
```

## Méthodes

| Nom | Description |
| --- | --- |
| [LoadImages](../../groupdocs.redaction.integration/ifixedformatdocument/loadimages)(RedactionFilter[]) | Charge un tableau d'instances d'images raster, contenues dans le document, correspondant à l'ensemble [`RedactionFilter`](../../groupdocs.redaction.redactions/redactionfilter) spécifié. |
| [RedactAnnotation](../../groupdocs.redaction.integration/ifixedformatdocument/redactannotation)(Regex, ReplacementOptions) | Remplace le texte correspondant dans toutes les annotations du document avec les options fournies. |

### Remarques

**Learn more**

* More details about applying redactions: [Redaction basics](https://docs.groupdocs.com/redaction/net/redaction-basics/)
* More details about PageAreaRedaction: [Use PageAreaRedaction](https://docs.groupdocs.com/redaction/net/use-page-area-redaction/)
* More details about implementing custom formats: [Create custom format handler](https://docs.groupdocs.com/redaction/net/create-custom-format-handler/)

### Voir aussi

* namespace [GroupDocs.Redaction.Integration](../../groupdocs.redaction.integration)
* assembly [GroupDocs.Redaction](../../)

<!-- NE PAS MODIFIER : généré par xmldocmd pour GroupDocs.Redaction.dll -->
