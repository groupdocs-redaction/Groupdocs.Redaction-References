---
title: "com.groupdocs.redaction.redactions"
second_title: "GroupDocs.Redaction for Java API-referentie"
description: "Het pakket biedt klassen voor verschillende soorten redactie."
type: docs
weight: 16
url: /nl/java/com.groupdocs.redaction.redactions/
---

Het pakket biedt klassen voor verschillende soorten redactie.



## Klassen

| Klasse | Beschrijving |
| --- | --- |
| [AnnotationRedaction](../com.groupdocs.redaction.redactions/annotationredaction) | Stelt een redactiestrategie voor die annotatietekst (commentaren, enz.) vervangt die overeenkomt met een gegeven reguliere expressie. |
| [CellColumnRedaction](../com.groupdocs.redaction.redactions/cellcolumnredaction) | Stelt een tekstredactie voor die tekst in spreadsheetdocumenten (CSV, Excel, enz.) vervangt. |
| [CellFilter](../com.groupdocs.redaction.redactions/cellfilter) | Biedt een optie om de reikwijdte van een CellColumnRedaction te beperken tot een werkblad en een kolom. |
| [CustomRedactionContext](../com.groupdocs.redaction.redactions/customredactioncontext) | Biedt invoergegevens voor [ICustomRedactionHandler](../com.groupdocs.redaction.redactions/icustomredactionhandler). |
| [CustomRedactionResult](../com.groupdocs.redaction.redactions/customredactionresult) | Stelt een resultaat voor dat wordt geretourneerd door [ICustomRedactionHandler](../com.groupdocs.redaction.redactions/icustomredactionhandler). |
| [DeleteAnnotationRedaction](../com.groupdocs.redaction.redactions/deleteannotationredaction) | Stelt een tekstredactie voor die annotaties verwijdert als de tekst overeenkomt met een gegeven reguliere expressie (optioneel worden alle annotaties verwijderd). |
| [EraseMetadataRedaction](../com.groupdocs.redaction.redactions/erasemetadataredaction) | Stelt een metadataredactie voor die alle metadata of metadata die overeenkomt met specifieke MetadataFilters uit het document wist. |
| [ExactPhraseRedaction](../com.groupdocs.redaction.redactions/exactphraseredaction) | Stelt een tekstredactie voor die exacte zinnen in de documenttekst vervangt, standaard zonder hoofdlettergevoeligheid. |
| [ImageAreaRedaction](../com.groupdocs.redaction.redactions/imagearearedaction) | Stelt een redactiestrategie voor die een gekleurde rechthoek plaatst in een opgegeven gebied van een beelddocument. |
| [MetadataFilters](../com.groupdocs.redaction.redactions/metadatafilters) | Stelt een lijst voor van de meest voorkomende typen documentmetadata. |
| [MetadataRedaction](../com.groupdocs.redaction.redactions/metadataredaction) | Vertegenwoordigt een abstracte basisklasse voor documentmetadata-redacties. |
| [MetadataSearchRedaction](../com.groupdocs.redaction.redactions/metadatasearchredaction) | Vertegenwoordigt een metadata-redactie die metadata doorzoekt en redacteert met behulp van reguliere expressies, waarbij sleutels en/of waarden worden gematcht. |
| [PageAreaFilter](../com.groupdocs.redaction.redactions/pageareafilter) | Vertegenwoordigt een redactiefilter dat een gebied binnen een pagina van een document instelt om redacties toe te passen. |
| [PageAreaRedaction](../com.groupdocs.redaction.redactions/pagearearedaction) | Vertegenwoordigt een complexe tekstuele redactie die tekst, afbeeldingen en annotaties in een gebied van de pagina beïnvloedt. |
| [PageRangeFilter](../com.groupdocs.redaction.redactions/pagerangefilter) | Vertegenwoordigt een redactiefilter dat een paginabereik binnen een document instelt om redacties toe te passen. |
| [RedactionDescription](../com.groupdocs.redaction.redactions/redactiondescription) | Vertegenwoordigt informatie over een enkele wijzigingsactie die tijdens het redactieproces wordt uitgevoerd. |
| [RedactionFilter](../com.groupdocs.redaction.redactions/redactionfilter) | Vertegenwoordigt een redactiefilter dat de reikwijdte binnen een document instelt om redacties toe te passen. |
| [RedactionType](../com.groupdocs.redaction.redactions/redactiontype) | Vertegenwoordigt een type documentgegevens die door redacties worden beïnvloed. |
| [RegexRedaction](../com.groupdocs.redaction.redactions/regexredaction) | Vertegenwoordigt een tekstredactie die tekst in het document doorzoekt en vervangt door de opgegeven reguliere expressie te matchen. |
| [RegionReplacementOptions](../com.groupdocs.redaction.redactions/regionreplacementoptions) | Vertegenwoordigt kleur- en gebiedsparameters voor het vervangen van een afbeeldingsgebied. |
| [RemovePageRedaction](../com.groupdocs.redaction.redactions/removepageredaction) | Vertegenwoordigt een redactie die een pagina (dia, werkblad, enz.) uit een document verwijdert. |
| [ReplacementOptions](../com.groupdocs.redaction.redactions/replacementoptions) | Vertegenwoordigt opties voor het vervangen van gematchte tekst. |
| [TextRedaction](../com.groupdocs.redaction.redactions/textredaction) | Vertegenwoordigt een abstracte basisklasse voor documenttekst-redacties. |
| [TextReplacement](../com.groupdocs.redaction.redactions/textreplacement) | Vertegenwoordigt informatie over een tekstuele vervanging. |

## Interfaces

| Interface | Beschrijving |
| --- | --- |
| [ICustomRedactionHandler](../com.groupdocs.redaction.redactions/icustomredactionhandler) | Definieert een aangepaste redactiecallback. |
| [IRedactionCallback](../com.groupdocs.redaction.redactions/iredactioncallback) | Definieert methoden die vereist zijn om informatie over elke redactiewijziging te ontvangen en deze eventueel te voorkomen. |

## Enumeraties

| Enumeratie | Beschrijving |
| --- | --- |
| [PageSeekOrigin](../com.groupdocs.redaction.redactions/pageseekorigin) | Biedt de velden die referentiepunten in een document voor navigatie vertegenwoordigen. |
| [RedactionActionType](../com.groupdocs.redaction.redactions/redactionactiontype) | Vertegenwoordigt acties die kunnen worden ondernomen om redacties uit te voeren. |
| [ReplacementType](../com.groupdocs.redaction.redactions/replacementtype) | Vertegenwoordigt een type vervanging voor de gematchte tekst. |
