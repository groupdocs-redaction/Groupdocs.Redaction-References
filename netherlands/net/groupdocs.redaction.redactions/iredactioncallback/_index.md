---
title: "IRedactionCallback"
second_title: "GroupDocs.Redaction voor .NET API-referentie"
description: "Definieert methoden die vereist zijn om informatie over elke redactiewijziging te ontvangen en deze eventueel te voorkomen."
type: docs
weight: 620
url: /nl/net/groupdocs.redaction.redactions/iredactioncallback/
---
## IRedactionCallback interface

Definieert methoden die vereist zijn om informatie over elke redactiewijziging te ontvangen en deze eventueel te voorkomen.

```csharp
public interface IRedactionCallback
```

## Methoden

| Naam | Beschrijving |
| --- | --- |
| [AcceptRedaction](../../groupdocs.redaction.redactions/iredactioncallback/acceptredaction)(RedactionDescription) | Deze oproep wordt geactiveerd vlak vóór het toepassen van enige redactie op het document en maakt het mogelijk om dit te loggen of te verbieden. |

### Opmerkingen

**Learn more**

* More details about implementing IRedactionCallback interface: [Use redaction callback](https://docs.groupdocs.com/redaction/net/use-redaction-callback/)

### Voorbeelden

Het volgende voorbeeld toont hoe je gedetailleerde logging voor het redactieproces kunt implementeren.

```csharp
public class RedactionDump : IRedactionCallback
{
    public RedactionDump()
    {
    }

    public bool AcceptRedaction(RedactionDescription description)
    {
        Console.Write("{0} redaction, {1} action, item {2}. ", description.RedactionType, description.ActionType, description.OriginalText);
        if (description.Replacement != null)
        {
            Console.Write("Text {0} is replaced with {1}. ", description.Replacement.OriginalText, description.Replacement.Replacement);
        }
        Console.WriteLine();
        // je kunt hier "false" retourneren om een specifieke wijziging tijdens het redactieproces te voorkomen
        return true;
    }
}

...

// Wijs een instantie toe voordat je Redactor gebruikt
Redactor.RedactionCallback = new RedactionDump();
```

### Zie ook

* namespace [GroupDocs.Redaction.Redactions](../../groupdocs.redaction.redactions)
* assembly [GroupDocs.Redaction](../../)

<!-- NIET BEWERKEN: gegenereerd door xmldocmd voor GroupDocs.Redaction.dll -->
