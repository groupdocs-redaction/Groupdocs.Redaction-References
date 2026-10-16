---
title: "RedactionDescription"
second_title: "GroupDocs.Redaction voor .NET API-referentie"
description: "Initialiseert een nieuw exemplaar van de RedactionDescription-klasse zonder vervangingsinformatie."
type: docs
weight: 10
url: /nl/net/groupdocs.redaction.redactions/redactiondescription/redactiondescription/
---
## RedactionDescription(RedactionType, RedactionActionType, string) {#constructor_1}

Initialiseert een nieuw exemplaar van de RedactionDescription-klasse zonder vervangingsinformatie.

```csharp
public RedactionDescription(RedactionType redactionType, RedactionActionType actionType, 
    string originalText)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| redactionType | RedactionType | Type van de gegevens die worden geredigeerd |
| actionType | RedactionActionType | Actie die op deze gegevens moet worden uitgevoerd |
| originalText | String | Gevonden tekst, opmerking of annotatie-inhoud |

### Zie ook

* enum [RedactionType](../../redactiontype)
* enum [RedactionActionType](../../redactionactiontype)
* class [RedactionDescription](../../redactiondescription)
* namespace [GroupDocs.Redaction.Redactions](../../../groupdocs.redaction.redactions)
* assembly [GroupDocs.Redaction](../../../)

---

## RedactionDescription(RedactionType, RedactionActionType, string, TextReplacement) {#constructor_2}

Initialiseert een nieuw exemplaar van de RedactionDescription-klasse met vervangingsinformatie.

```csharp
public RedactionDescription(RedactionType redactionType, RedactionActionType actionType, 
    string originalText, TextReplacement replacement)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| redactionType | RedactionType | Type van de gegevens die worden geredigeerd |
| actionType | RedactionActionType | Actie die op deze gegevens moet worden uitgevoerd |
| originalText | String | Gevonden tekst, opmerking of annotatie-inhoud |
| vervanging | TextReplacement | Vervangende tekst, gevonden tekst en de positie ervan binnen de oorspronkelijke tekenreeks |

### Zie ook

* enum [RedactionType](../../redactiontype)
* enum [RedactionActionType](../../redactionactiontype)
* class [TextReplacement](../../textreplacement)
* class [RedactionDescription](../../redactiondescription)
* namespace [GroupDocs.Redaction.Redactions](../../../groupdocs.redaction.redactions)
* assembly [GroupDocs.Redaction](../../../)

---

## RedactionDescription(RedactionType, RedactionActionType, RegionReplacementOptions, string) {#constructor}

Initialiseert een nieuw exemplaar van de RedactionDescription-klasse met vervangingsinformatie voor een afbeeldingsgebied.

```csharp
public RedactionDescription(RedactionType redactionType, RedactionActionType actionType, 
    RegionReplacementOptions imageAreaReplacement, string imageDetails)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| redactionType | RedactionType | Type van de gegevens die worden geredigeerd |
| actionType | RedactionActionType | Actie die op deze gegevens moet worden uitgevoerd |
| imageAreaReplacement | RegionReplacementOptions | Informatie over vervanging van afbeeldingsgebied |
| imageDetails | String | Tekstuele beschrijving van afbeelding, standaard is het String.Empty |

### Zie ook

* enum [RedactionType](../../redactiontype)
* enum [RedactionActionType](../../redactionactiontype)
* class [RegionReplacementOptions](../../regionreplacementoptions)
* class [RedactionDescription](../../redactiondescription)
* namespace [GroupDocs.Redaction.Redactions](../../../groupdocs.redaction.redactions)
* assembly [GroupDocs.Redaction](../../../)

<!-- NIET BEWERKEN: gegenereerd door xmldocmd voor GroupDocs.Redaction.dll -->
