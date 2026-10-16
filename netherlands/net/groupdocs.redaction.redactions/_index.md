---
title: "GroupDocs.Redaction.Redactions"
second_title: "GroupDocs.Redaction voor .NET API-referentie"
description: "De Redactions namespace biedt klassen voor verschillende soorten redigeringen."
type: docs
weight: 80
url: /nl/net/groupdocs.redaction.redactions/
---
De Redactions namespace biedt klassen voor verschillende soorten redigeringen.

## Klassen

| Klasse | Beschrijving |
| --- | --- |
| [AnnotationRedaction](./annotationredaction) | Stelt een redactie voor die annotatietekst (commentaren, enz.) vervangt die overeenkomt met een gegeven reguliere expressie. |
| [CellColumnRedaction](./cellcolumnredaction) | Stelt een tekstredactie voor die tekst in spreadsheet‑documenten (CSV, Excel, enz.) vervangt. |
| [CellFilter](./cellfilter) | Biedt een optie om de reikwijdte van een [`CellColumnRedaction`](../groupdocs.redaction.redactions/cellcolumnredaction) te beperken tot een werkblad en een kolom. |
| [CustomRedactionContext](./customredactioncontext) | Biedt context voor aangepaste redactieverwerking. |
| [CustomRedactionResult](./customredactionresult) | Stelt het resultaat van een aangepaste redactiebewerking voor. |
| [DeleteAnnotationRedaction](./deleteannotationredaction) | Stelt een tekstredactie voor die annotaties verwijdert als de tekst overeenkomt met een gegeven reguliere expressie (optioneel worden alle annotaties verwijderd). |
| [EraseMetadataRedaction](./erasemetadataredaction) | Stelt een metadata‑redactie voor die alle metadata of metadata die overeenkomen met specifieke MetadataFilters uit het document verwijdert. |
| [ExactPhraseRedaction](./exactphraseredaction) | Stelt een tekstredactie voor die exacte zinnen in de tekst van het document vervangt, standaard hoofdletterongevoelig. |
| [ImageAreaRedaction](./imagearearedaction) | Stelt een redactie voor die een gekleurde rechthoek plaatst in een opgegeven gebied van een afbeeldingsdocument. |
| [MetadataRedaction](./metadataredaction) | Stelt een basis abstracte klasse voor documentmetadata‑redacties voor. |
| [MetadataSearchRedaction](./metadatasearchredaction) | Stelt een metadata‑redactie voor die metadata zoekt en redigeert met behulp van reguliere expressies, waarbij sleutels en/of waarden overeenkomen. |
| [PageAreaFilter](./pageareafilter) | Stelt een redactiefilter voor, waarbij een gebied binnen een pagina van een document wordt ingesteld om redacties toe te passen. |
| [PageAreaRedaction](./pagearearedaction) | Stelt een complexe tekstuele redactie voor die tekst, afbeeldingen en annotaties in een gebied van de pagina beïnvloedt. |
| [PageRangeFilter](./pagerangefilter) | Stelt een redactiefilter voor, waarbij een paginabereik binnen een document wordt ingesteld om redacties toe te passen. |
| [RedactionDescription](./redactiondescription) | Stelt een enkele wijzigingsactie‑informatie voor die tijdens het redactieproces wordt uitgevoerd. |
| [RedactionFilter](./redactionfilter) | Stelt een redactiefilter voor, waarbij een scope binnen een document wordt ingesteld om redacties toe te passen. |
| [RegexRedaction](./regexredaction) | Stelt een tekstredactie voor die tekst in het document zoekt en vervangt door overeenstemming met de opgegeven reguliere expressie. |
| [RegionReplacementOptions](./regionreplacementoptions) | Stelt kleur‑ en gebiedsparameters voor vervanging van een afbeeldingsgebied voor. Zie [`ImageAreaRedaction`](../groupdocs.redaction.redactions/imagearearedaction). |
| [RemovePageRedaction](./removepageredaction) | Stelt een redactie voor die een pagina (dia, werkblad, enz.) uit een document verwijdert. |
| [ReplacementOptions](./replacementoptions) | Stelt opties voor vervanging van overeenkomende tekst voor. |
| [TextRedaction](./textredaction) | Stelt een basis abstracte klasse voor documenttekst‑redacties voor. |
| [TextReplacement](./textreplacement) | Stelt informatie over een tekstuele vervanging voor. |
## Interfaces

| Interface | Beschrijving |
| --- | --- |
| [ICustomRedactionHandler](./icustomredactionhandler) | Biedt een interface voor het implementeren van aangepaste redactielogica. |
| [IRedactionCallback](./iredactioncallback) | Definieert methoden die vereist zijn om informatie over elke redactiewijziging te ontvangen en deze eventueel te voorkomen. |
## Enumeratie

| Enumeratie | Beschrijving |
| --- | --- |
| [MetadataFilters](./metadatafilters) | Stelt een lijst voor van de meest voorkomende typen documentmetadata. |
| [PageSeekOrigin](./pageseekorigin) | Biedt de velden die referentiepunten in een document voor zoeken vertegenwoordigen. |
| [RedactionActionType](./redactionactiontype) | Stelt acties voor die kunnen worden ondernomen om redacties uit te voeren. |
| [RedactionType](./redactiontype) | Stelt een type gegevens van een document voor, dat door redacties wordt beïnvloed. |
| [ReplacementType](./replacementtype) | Stelt een type vervanging voor de overeenkomende tekst voor. |

<!-- NIET BEWERKEN: gegenereerd door xmldocmd voor GroupDocs.Redaction.dll -->
