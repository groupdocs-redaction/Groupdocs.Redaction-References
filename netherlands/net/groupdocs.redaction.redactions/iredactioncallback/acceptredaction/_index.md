---
title: "AcceptRedaction"
second_title: "GroupDocs.Redaction voor .NET API-referentie"
description: "Deze oproep wordt geactiveerd vlak vóór het toepassen van enige redactie op het document en maakt het mogelijk om dit te loggen of te verbieden."
type: docs
weight: 10
url: /nl/net/groupdocs.redaction.redactions/iredactioncallback/acceptredaction/
---
## IRedactionCallback.AcceptRedaction method

Deze oproep wordt geactiveerd vlak vóór het toepassen van enige redactie op het document en maakt het mogelijk om dit te loggen of te verbieden.

```csharp
public bool AcceptRedaction(RedactionDescription description)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| beschrijving | RedactionDescription | Bevat informatie over een specifiek overeenkomsttype, criteria, tekst en positie |

### Retourwaarde

Retourneer true om een specifieke overeenkomstredactie te accepteren of false om deze af te wijzen

### Zie ook

* class [RedactionDescription](../../redactiondescription)
* interface [IRedactionCallback](../../iredactioncallback)
* namespace [GroupDocs.Redaction.Redactions](../../../groupdocs.redaction.redactions)
* assembly [GroupDocs.Redaction](../../../)

<!-- NIET BEWERKEN: gegenereerd door xmldocmd voor GroupDocs.Redaction.dll -->
