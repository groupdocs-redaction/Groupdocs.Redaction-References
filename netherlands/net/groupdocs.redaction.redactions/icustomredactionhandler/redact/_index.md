---
title: "Redigeren"
second_title: "GroupDocs.Redaction voor .NET API-referentie"
description: "Past aangepaste redactie toe op specifieke documentinhoud. Momenteel wordt dit alleen ondersteund voor PDF PageAreaRedactiongroupdocs.redaction.redactions/pagearearedaction. Gebruikers kunnen hun eigen redactielogica definiëren, zoals AIbased redaction, die geavanceerder kan zijn dan eenvoudige patternbased methoden."
type: docs
weight: 10
url: /nl/net/groupdocs.redaction.redactions/icustomredactionhandler/redact/
---
## ICustomRedactionHandler.Redact method

Past aangepaste redactie toe op specifieke documentinhoud. Momenteel wordt dit alleen ondersteund voor PDF [`PageAreaRedaction`](../../pagearearedaction). Gebruikers kunnen hun eigen redactielogica definiëren, zoals AI-based redaction, die geavanceerder kan zijn dan eenvoudige pattern-based methoden.

```csharp
public CustomRedactionResult Redact(CustomRedactionContext context)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| context | CustomRedactionContext | Bevat de documentinhoud die moet worden geredigeerd, samen met gerelateerde metadata. |

### Retourwaarde

Een [`CustomRedactionResult`](../../customredactionresult) die aangeeft of de redactie moet worden toegepast en de gewijzigde inhoud.

### Zie ook

* class [CustomRedactionResult](../../customredactionresult)
* class [CustomRedactionContext](../../customredactioncontext)
* interface [ICustomRedactionHandler](../../icustomredactionhandler)
* namespace [GroupDocs.Redaction.Redactions](../../../groupdocs.redaction.redactions)
* assembly [GroupDocs.Redaction](../../../)

<!-- NIET BEWERKEN: gegenereerd door xmldocmd voor GroupDocs.Redaction.dll -->
