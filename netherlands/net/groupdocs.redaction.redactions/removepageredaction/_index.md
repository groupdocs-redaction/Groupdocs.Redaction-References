---
title: "RemovePageRedaction"
second_title: "GroupDocs.Redaction voor .NET API-referentie"
description: "Stelt een redactie voor die een pagina, dia, werkblad enz. uit een document verwijdert."
type: docs
weight: 770
url: /nl/net/groupdocs.redaction.redactions/removepageredaction/
---
## RemovePageRedaction class

Stelt een redactie voor die een pagina (dia, werkblad, enz.) uit een document verwijdert.

```csharp
public class RemovePageRedaction : Redaction
```

## Constructors

| Naam | Beschrijving |
| --- | --- |
| [RemovePageRedaction](removepageredaction)(PageSeekOrigin, int, int) | Initialiseert een nieuw exemplaar van de RemovePageRedaction-klasse. |

## Properties

| Naam | Beschrijving |
| --- | --- |
| [Count](../../groupdocs.redaction.redactions/removepageredaction/count) { get; } | Haalt het aantal te verwijderen pagina's op. |
| virtual [Description](../../groupdocs.redaction/redaction/description) { get; } | Retourneert een string die de redactie en de parameters beschrijft. |
| [Index](../../groupdocs.redaction.redactions/removepageredaction/index) { get; } | Haalt de startpositie-index op (0-gebaseerd). |
| [Origin](../../groupdocs.redaction.redactions/removepageredaction/origin) { get; } | Haalt de zoekreferentiepositie op, het begin of het einde van een document. |

## Methoden

| Naam | Beschrijving |
| --- | --- |
| override [ApplyTo](../../groupdocs.redaction.redactions/removepageredaction/applyto)(DocumentFormatInstance) | Past de redactie toe op een gegeven format‑instantie. |

### Opmerkingen

**Learn more**

* More details about applying redactions: [Redaction basics](https://docs.groupdocs.com/redaction/net/redaction-basics/)
* More details about removing pages: [Remove page redaction](https://docs.groupdocs.com/redaction/net/remove-page-redaction/)

### Voorbeelden

Het volgende voorbeeld toont hoe de laatste pagina van het document te verwijderen.

```csharp
using (Redactor redactor = new Redactor(@"C:\test.pdf"))
{
   redactor.Apply(new RemovePageRedaction(PageSeekOrigin.End, 0, 1));
   redactor.Save()
}
```

### Zie ook

* class [Redaction](../../groupdocs.redaction/redaction)
* namespace [GroupDocs.Redaction.Redactions](../../groupdocs.redaction.redactions)
* assembly [GroupDocs.Redaction](../../)

<!-- NIET BEWERKEN: gegenereerd door xmldocmd voor GroupDocs.Redaction.dll -->
