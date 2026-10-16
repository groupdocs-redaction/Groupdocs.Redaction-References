---
title: "DeleteAnnotationRedaction"
second_title: "GroupDocs.Redaction voor .NET API-referentie"
description: "Stelt een tekstredactie voor die annotaties verwijdert als de tekst overeenkomt met de opgegeven reguliere expressie, en optioneel alle annotaties verwijdert."
type: docs
weight: 580
url: /nl/net/groupdocs.redaction.redactions/deleteannotationredaction/
---
## DeleteAnnotationRedaction class

Stelt een tekstredactie voor die annotaties verwijdert als de tekst overeenkomt met een gegeven reguliere expressie (optioneel worden alle annotaties verwijderd).

```csharp
public class DeleteAnnotationRedaction : Redaction
```

## Constructors

| Naam | Beschrijving |
| --- | --- |
| [DeleteAnnotationRedaction](deleteannotationredaction#constructor)() | Initialiseert een nieuw exemplaar van de DeleteAnnotationRedaction-klasse, met instellingen om alle annotaties te verwijderen (alles overeenkomend). |
| [DeleteAnnotationRedaction](deleteannotationredaction#constructor_2)(Regex) | Initialiseert een nieuw exemplaar van de DeleteAnnotationRedaction-klasse, die annotaties verwijdert die overeenkomen met de opgegeven expressie. |
| [DeleteAnnotationRedaction](deleteannotationredaction#constructor_1)(string) | Initialiseert een nieuw exemplaar van de DeleteAnnotationRedaction-klasse, die annotaties verwijdert die overeenkomen met de opgegeven expressie. |

## Properties

| Naam | Beschrijving |
| --- | --- |
| override [Description](../../groupdocs.redaction.redactions/deleteannotationredaction/description) { get; } | Retourneert een string die de redactie en de parameters beschrijft. |
| [Expression](../../groupdocs.redaction.redactions/deleteannotationredaction/expression) { get; } | Haalt de reguliere expressie op die moet overeenkomen. |

## Methoden

| Naam | Beschrijving |
| --- | --- |
| override [ApplyTo](../../groupdocs.redaction.redactions/deleteannotationredaction/applyto)(DocumentFormatInstance) | Past de redactie toe op een gegeven format‑instantie. |

### Opmerkingen

**Learn more**

* More details about applying redactions: [Redaction basics](https://docs.groupdocs.com/redaction/net/redaction-basics/)
* More details about document annotation redactions: [Annotation redactions](https://docs.groupdocs.com/redaction/net/annotation-redactions/)

### Voorbeelden

Het volgende voorbeeld toont hoe alle annotaties die de woorden "use", "show" of "describe" bevatten uit een document te verwijderen (en de andere te behouden).

```csharp
using (Redactor redactor = new Redactor(@"D:\test.docx"))
{
   redactor.Apply(new DeleteAnnotationRedaction("(?im:(use|show|describe))"));
   redactor.Save()
}
```

### Zie ook

* class [Redaction](../../groupdocs.redaction/redaction)
* namespace [GroupDocs.Redaction.Redactions](../../groupdocs.redaction.redactions)
* assembly [GroupDocs.Redaction](../../)

<!-- NIET BEWERKEN: gegenereerd door xmldocmd voor GroupDocs.Redaction.dll -->
