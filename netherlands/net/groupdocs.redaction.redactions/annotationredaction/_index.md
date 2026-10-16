---
title: "AnnotationRedaction"
second_title: "GroupDocs.Redaction voor .NET API-referentie"
description: "Stelt een redactie voor die annotatietekst, opmerkingen enz. vervangt die overeenkomt met een opgegeven reguliere expressie."
type: docs
weight: 530
url: /nl/net/groupdocs.redaction.redactions/annotationredaction/
---
## AnnotationRedaction class

Stelt een redactie voor die annotatietekst (commentaren, enz.) vervangt die overeenkomt met een gegeven reguliere expressie.

```csharp
public class AnnotationRedaction : Redaction
```

## Constructors

| Naam | Beschrijving |
| --- | --- |
| [AnnotationRedaction](annotationredaction#constructor_1)(Regex, string) | Initialiseert een nieuw exemplaar van de klasse AnnotationRedaction. |
| [AnnotationRedaction](annotationredaction#constructor)(string, string) | Initialiseert een nieuw exemplaar van de klasse AnnotationRedaction. |

## Properties

| Naam | Beschrijving |
| --- | --- |
| override [Description](../../groupdocs.redaction.redactions/annotationredaction/description) { get; } | Retourneert een string die de redactie en de parameters beschrijft. |
| [Expression](../../groupdocs.redaction.redactions/annotationredaction/expression) { get; } | Haalt de reguliere expressie op die moet overeenkomen. |
| [Replacement](../../groupdocs.redaction.redactions/annotationredaction/replacement) { get; } | Haalt een tekstvervanging op voor overeenkomende tekst. |

## Methoden

| Naam | Beschrijving |
| --- | --- |
| override [ApplyTo](../../groupdocs.redaction.redactions/annotationredaction/applyto)(DocumentFormatInstance) | Past de redactie toe op een gegeven format‑instantie. |

### Opmerkingen

**Learn more**

* More details about applying redactions: [Redaction basics](https://docs.groupdocs.com/redaction/net/redaction-basics/)
* More details about document annotation redactions: [Annotation redactions](https://docs.groupdocs.com/redaction/net/annotation-redactions/)

### Voorbeelden

Het volgende voorbeeld toont hoe de naam "John" te vervangen door "[redacted]" in alle annotaties.

```csharp
using (Redactor redactor = new Redactor(@"C:\test.pdf"))
{
   redactor.Apply(new AnnotationRedaction("(?im:john)", "[redacted]"));
   redactor.Save()
}
```

### Zie ook

* class [Redaction](../../groupdocs.redaction/redaction)
* namespace [GroupDocs.Redaction.Redactions](../../groupdocs.redaction.redactions)
* assembly [GroupDocs.Redaction](../../)

<!-- NIET BEWERKEN: gegenereerd door xmldocmd voor GroupDocs.Redaction.dll -->
