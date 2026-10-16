---
title: "IAnnotatedDocument"
second_title: "Référence API de GroupDocs.Redaction pour .NET"
description: "Définit les méthodes requises pour accéder aux annotations telles que les commentaires. Doit être implémenté par la classe DocumentFormatInstance./documentformatinstancederived pour effectuer les redactions d'annotation."
type: docs
weight: 120
url: /fr/net/groupdocs.redaction.integration/iannotateddocument/
---
## IAnnotatedDocument interface

Définit les méthodes requises pour accéder aux annotations, telles que les commentaires. Doit être implémenté par la classe [`DocumentFormatInstance`](../documentformatinstance)-derived pour effectuer les redactions d'annotation.

```csharp
public interface IAnnotatedDocument
```

## Méthodes

| Nom | Description |
| --- | --- |
| [DeleteAnnotations](../../groupdocs.redaction.integration/iannotateddocument/deleteannotations)(Regex) | Supprime toutes les annotations correspondant à l'expression régulière dans le document. |
| [RedactAnnotation](../../groupdocs.redaction.integration/iannotateddocument/redactannotation)(Regex, string) | Remplace le texte correspondant dans toutes les annotations du document. |

### Remarques

**Learn more**

* More details about applying redactions: [Redaction basics](https://docs.groupdocs.com/redaction/net/redaction-basics/)
* More details about document annotation redactions: [Annotation redactions](https://docs.groupdocs.com/redaction/net/annotation-redactions/)
* More details about implementing custom formats: [Create custom format handler](https://docs.groupdocs.com/redaction/net/create-custom-format-handler/)

### Voir aussi

* namespace [GroupDocs.Redaction.Integration](../../groupdocs.redaction.integration)
* assembly [GroupDocs.Redaction](../../)

<!-- NE PAS MODIFIER : généré par xmldocmd pour GroupDocs.Redaction.dll -->
