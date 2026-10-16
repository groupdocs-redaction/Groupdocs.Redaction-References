---
title: "IRedactionCallback"
second_title: "Référence API de GroupDocs.Redaction pour .NET"
description: "Définit les méthodes requises pour recevoir des informations sur chaque modification de rédaction et éventuellement l'empêcher."
type: docs
weight: 620
url: /fr/net/groupdocs.redaction.redactions/iredactioncallback/
---
## IRedactionCallback interface

Définit les méthodes requises pour recevoir des informations sur chaque modification de rédaction et éventuellement l'empêcher.

```csharp
public interface IRedactionCallback
```

## Méthodes

| Nom | Description |
| --- | --- |
| [AcceptRedaction](../../groupdocs.redaction.redactions/iredactioncallback/acceptredaction)(RedactionDescription) | Cet appel est déclenché juste avant l'application de toute rédaction au document et permet de l'enregistrer ou de l'interdire. |

### Remarques

**Learn more**

* More details about implementing IRedactionCallback interface: [Use redaction callback](https://docs.groupdocs.com/redaction/net/use-redaction-callback/)

### Exemples

L'exemple suivant montre comment mettre en œuvre une journalisation détaillée du processus de rédaction.

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
        // vous pouvez retourner "false" ici pour empêcher une modification particulière pendant le processus de rédaction.
        return true;
    }
}

...

// Attribuez une instance avant d'utiliser Redactor
Redactor.RedactionCallback = new RedactionDump();
```

### Voir aussi

* namespace [GroupDocs.Redaction.Redactions](../../groupdocs.redaction.redactions)
* assembly [GroupDocs.Redaction](../../)

<!-- NE PAS MODIFIER : généré par xmldocmd pour GroupDocs.Redaction.dll -->
