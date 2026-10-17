---
title: "IRedactionCallback"
second_title: "GroupDocs.Redaction för .NET API-referens"
description: "Definierar metoder som krävs för att ta emot information om varje redigeringsändring och eventuellt förhindra den."
type: docs
weight: 620
url: /sv/net/groupdocs.redaction.redactions/iredactioncallback/
---
## IRedactionCallback interface

Definierar metoder som krävs för att ta emot information om varje redigeringsändring och eventuellt förhindra den.

```csharp
public interface IRedactionCallback
```

## Metoder

| Namn | Beskrivning |
| --- | --- |
| [AcceptRedaction](../../groupdocs.redaction.redactions/iredactioncallback/acceptredaction)(RedactionDescription) | Detta anrop utlöses precis innan någon redigering tillämpas på dokumentet och möjliggör att logga eller förbjuda det. |

### Anmärkningar

**Learn more**

* More details about implementing IRedactionCallback interface: [Use redaction callback](https://docs.groupdocs.com/redaction/net/use-redaction-callback/)

### Exempel

Följande exempel visar hur man implementerar detaljerad loggning för redigeringsprocessen.

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
        // du kan returnera "false" här för att förhindra en specifik förändring under redigeringsprocessen
        return true;
    }
}

...

// Tilldela en instans innan du använder Redactor
Redactor.RedactionCallback = new RedactionDump();
```

### Se även

* namespace [GroupDocs.Redaction.Redactions](../../groupdocs.redaction.redactions)
* assembly [GroupDocs.Redaction](../../)

<!-- GÅ INTE ATT REDIGERA: genererad av xmldocmd för GroupDocs.Redaction.dll -->
