---
title: "com.groupdocs.redaction.redactions"
second_title: "Référence API de GroupDocs.Redaction pour Java"
description: "Le package fournit des classes pour différents types de caviardages."
type: docs
weight: 16
url: /fr/java/com.groupdocs.redaction.redactions/
---

Le package fournit des classes pour différents types de caviardages.



## Classes

| Classe | Description |
| --- | --- |
| [AnnotationRedaction](../com.groupdocs.redaction.redactions/annotationredaction) | Représente une rédaction qui remplace le texte d'annotation (commentaires, etc.) correspondant à une expression régulière donnée. |
| [CellColumnRedaction](../com.groupdocs.redaction.redactions/cellcolumnredaction) | Représente une rédaction de texte qui remplace le texte dans des documents de feuille de calcul (CSV, Excel, etc.). |
| [CellFilter](../com.groupdocs.redaction.redactions/cellfilter) | Fournit une option pour limiter la portée d'une CellColumnRedaction à une feuille de calcul et à une colonne. |
| [CustomRedactionContext](../com.groupdocs.redaction.redactions/customredactioncontext) | Fournit les données d'entrée pour [ICustomRedactionHandler](../com.groupdocs.redaction.redactions/icustomredactionhandler). |
| [CustomRedactionResult](../com.groupdocs.redaction.redactions/customredactionresult) | Représente un résultat renvoyé par [ICustomRedactionHandler](../com.groupdocs.redaction.redactions/icustomredactionhandler). |
| [DeleteAnnotationRedaction](../com.groupdocs.redaction.redactions/deleteannotationredaction) | Représente une rédaction de texte qui supprime les annotations si le texte correspond à une expression régulière donnée (supprime éventuellement toutes les annotations). |
| [EraseMetadataRedaction](../com.groupdocs.redaction.redactions/erasemetadataredaction) | Représente une rédaction de métadonnées qui efface toutes les métadonnées ou les métadonnées correspondant à des filtres MetadataFilters spécifiques du document. |
| [ExactPhraseRedaction](../com.groupdocs.redaction.redactions/exactphraseredaction) | Représente une rédaction de texte qui remplace une phrase exacte dans le texte du document, insensible à la casse par défaut. |
| [ImageAreaRedaction](../com.groupdocs.redaction.redactions/imagearearedaction) | Représente une rédaction qui place un rectangle coloré dans une zone donnée d'un document image. |
| [MetadataFilters](../com.groupdocs.redaction.redactions/metadatafilters) | Représente une liste des types de métadonnées de document les plus courants. |
| [MetadataRedaction](../com.groupdocs.redaction.redactions/metadataredaction) | Représente une classe abstraite de base pour les rédactions de métadonnées de document. |
| [MetadataSearchRedaction](../com.groupdocs.redaction.redactions/metadatasearchredaction) | Représente une rédaction de métadonnées qui recherche et rédige les métadonnées à l'aide d'expressions régulières, en faisant correspondre les clés et/ou les valeurs. |
| [PageAreaFilter](../com.groupdocs.redaction.redactions/pageareafilter) | Représente un filtre de rédaction, définissant une zone au sein d'une page d'un document où appliquer la rédaction. |
| [PageAreaRedaction](../com.groupdocs.redaction.redactions/pagearearedaction) | Représente une rédaction textuelle complexe qui affecte le texte, les images et les annotations dans une zone de la page. |
| [PageRangeFilter](../com.groupdocs.redaction.redactions/pagerangefilter) | Représente un filtre de rédaction, définissant une plage de pages à l'intérieur d'un document pour appliquer la rédaction. |
| [RedactionDescription](../com.groupdocs.redaction.redactions/redactiondescription) | Représente les informations d'une action de modification unique effectuée pendant le processus de rédaction. |
| [RedactionFilter](../com.groupdocs.redaction.redactions/redactionfilter) | Représente un filtre de rédaction, définissant la portée à l'intérieur d'un document pour appliquer les rédactions. |
| [RedactionType](../com.groupdocs.redaction.redactions/redactiontype) | Représente un type de données de document, affecté par la rédaction. |
| [RegexRedaction](../com.groupdocs.redaction.redactions/regexredaction) | Représente une rédaction de texte qui recherche et remplace le texte dans le document en faisant correspondre l'expression régulière fournie. |
| [RegionReplacementOptions](../com.groupdocs.redaction.redactions/regionreplacementoptions) | Représente les paramètres de couleur et de zone pour le remplacement d'une région d'image. |
| [RemovePageRedaction](../com.groupdocs.redaction.redactions/removepageredaction) | Représente une rédaction qui supprime une page (diapositive, feuille de calcul, etc.) d'un document. |
| [ReplacementOptions](../com.groupdocs.redaction.redactions/replacementoptions) | Représente les options pour le remplacement du texte correspondant. |
| [TextRedaction](../com.groupdocs.redaction.redactions/textredaction) | Représente une classe abstraite de base pour les rédactions de texte de document. |
| [TextReplacement](../com.groupdocs.redaction.redactions/textreplacement) | Représente une information de remplacement textuel. |

## Interfaces

| Interface | Description |
| --- | --- |
| [ICustomRedactionHandler](../com.groupdocs.redaction.redactions/icustomredactionhandler) | Définit un rappel de rédaction personnalisé. |
| [IRedactionCallback](../com.groupdocs.redaction.redactions/iredactioncallback) | Définit les méthodes requises pour recevoir des informations sur chaque modification de rédaction et, éventuellement, l'empêcher. |

## Énumérations

| Énum | Description |
| --- | --- |
| [PageSeekOrigin](../com.groupdocs.redaction.redactions/pageseekorigin) | Fournit les champs qui représentent des points de référence dans un document pour la recherche. |
| [RedactionActionType](../com.groupdocs.redaction.redactions/redactionactiontype) | Représente les actions qui peuvent être effectuées pour réaliser la rédaction. |
| [ReplacementType](../com.groupdocs.redaction.redactions/replacementtype) | Représente un type de remplacement pour le texte correspondant. |
