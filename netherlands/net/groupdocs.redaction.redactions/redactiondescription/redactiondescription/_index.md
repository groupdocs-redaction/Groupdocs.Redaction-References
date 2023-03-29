---
title: RedactionDescription
second_title: GroupDocs.Redaction voor .NET API-referentie
description: Initialiseert een nieuwe instantie van de klasse RedactionDescription zonder vervangende informatie.
type: docs
weight: 10
url: /nl/net/groupdocs.redaction.redactions/redactiondescription/redactiondescription/
---
## RedactionDescription(RedactionType, RedactionActionType, string) {#constructor_1}

Initialiseert een nieuwe instantie van de klasse RedactionDescription zonder vervangende informatie.

```csharp
public RedactionDescription(RedactionType redactionType, RedactionActionType actionType, 
    string originalText)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| redactionType | RedactionType | Type gegevens dat wordt geredigeerd |
| actionType | RedactionActionType | Op deze gegevens uit te voeren actie |
| originalText | String | Overeenkomende tekst, opmerking of annotatie |

### Zie ook

* enum [RedactionType](../../redactiontype)
* enum [RedactionActionType](../../redactionactiontype)
* class [RedactionDescription](../../redactiondescription)
* naamruimte [GroupDocs.Redaction.Redactions](../../redactiondescription)
* montage [GroupDocs.Redaction](../../../)

---

## RedactionDescription(RedactionType, RedactionActionType, string, TextReplacement) {#constructor_2}

Initialiseert een nieuwe instantie van de klasse RedactionDescription met vervangende informatie.

```csharp
public RedactionDescription(RedactionType redactionType, RedactionActionType actionType, 
    string originalText, TextReplacement replacement)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| redactionType | RedactionType | Type gegevens dat wordt geredigeerd |
| actionType | RedactionActionType | Op deze gegevens uit te voeren actie |
| originalText | String | Overeenkomende tekst, opmerking of annotatie |
| replacement | TextReplacement | Vervangende tekst, overeenkomende tekst en de positie ervan binnen de oorspronkelijke tekenreeks |

### Zie ook

* enum [RedactionType](../../redactiontype)
* enum [RedactionActionType](../../redactionactiontype)
* class [TextReplacement](../../textreplacement)
* class [RedactionDescription](../../redactiondescription)
* naamruimte [GroupDocs.Redaction.Redactions](../../redactiondescription)
* montage [GroupDocs.Redaction](../../../)

---

## RedactionDescription(RedactionType, RedactionActionType, RegionReplacementOptions, string) {#constructor}

Initialiseert een nieuwe instantie van de klasse RedactionDescription met informatie over het vervangen van het afbeeldingsgebied.

```csharp
public RedactionDescription(RedactionType redactionType, RedactionActionType actionType, 
    RegionReplacementOptions imageAreaReplacement, string imageDetails)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| redactionType | RedactionType | Type gegevens dat wordt geredigeerd |
| actionType | RedactionActionType | Op deze gegevens uit te voeren actie |
| imageAreaReplacement | RegionReplacementOptions | Informatie over vervanging van beeldgebied |
| imageDetails | String | Afbeelding tekstuele beschrijving, standaard is dit String.Empty |

### Zie ook

* enum [RedactionType](../../redactiontype)
* enum [RedactionActionType](../../redactionactiontype)
* class [RegionReplacementOptions](../../regionreplacementoptions)
* class [RedactionDescription](../../redactiondescription)
* naamruimte [GroupDocs.Redaction.Redactions](../../redactiondescription)
* montage [GroupDocs.Redaction](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Redaction.dll -->