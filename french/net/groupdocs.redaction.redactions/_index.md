---
title: "GroupDocs.Redaction.Redactions"
second_title: "Référence API de GroupDocs.Redaction pour .NET"
description: "L’espace de noms Redactions fournit des classes pour différents types de masquages."
type: docs
weight: 80
url: /fr/net/groupdocs.redaction.redactions/
---
L’espace de noms Redactions fournit des classes pour différents types de masquages.

## Classes

| Classe | Description |
| --- | --- |
| [AnnotationRedaction](./annotationredaction) | Représente une rédaction qui remplace le texte d'annotation (commentaires, etc.) correspondant à une expression régulière donnée. |
| [CellColumnRedaction](./cellcolumnredaction) | Représente une rédaction de texte qui remplace le texte dans des documents de feuille de calcul (CSV, Excel, etc.). |
| [CellFilter](./cellfilter) | Fournit une option pour limiter la portée d'une [`CellColumnRedaction`](../groupdocs.redaction.redactions/cellcolumnredaction) à une feuille de calcul et à une colonne. |
| [CustomRedactionContext](./customredactioncontext) | Fournit un contexte pour le traitement de rédaction personnalisé. |
| [CustomRedactionResult](./customredactionresult) | Représente le résultat d'une opération de rédaction personnalisée. |
| [DeleteAnnotationRedaction](./deleteannotationredaction) | Représente une rédaction de texte qui supprime les annotations si le texte correspond à une expression régulière donnée (supprime éventuellement toutes les annotations). |
| [EraseMetadataRedaction](./erasemetadataredaction) | Représente une rédaction de métadonnées qui efface toutes les métadonnées ou les métadonnées correspondant à des MetadataFilters spécifiques du document. |
| [ExactPhraseRedaction](./exactphraseredaction) | Représente une rédaction de texte qui remplace une phrase exacte dans le texte du document, insensible à la casse par défaut. |
| [ImageAreaRedaction](./imagearearedaction) | Représente une rédaction qui place un rectangle coloré dans la zone donnée d'un document image. |
| [MetadataRedaction](./metadataredaction) | Représente une classe abstraite de base pour les rédactions de métadonnées de document. |
| [MetadataSearchRedaction](./metadatasearchredaction) | Représente une rédaction de métadonnées qui recherche et rédige les métadonnées à l'aide d'expressions régulières, en faisant correspondre les clés et/ou les valeurs. |
| [PageAreaFilter](./pageareafilter) | Représente un filtre de rédaction, définissant une zone au sein d'une page d'un document pour appliquer la rédaction. |
| [PageAreaRedaction](./pagearearedaction) | Représente une rédaction textuelle complexe qui affecte le texte, les images et les annotations dans une zone de la page. |
| [PageRangeFilter](./pagerangefilter) | Représente un filtre de rédaction, définissant une plage de pages à l'intérieur d'un document pour appliquer la rédaction. |
| [RedactionDescription](./redactiondescription) | Représente une information sur une action de modification unique effectuée pendant le processus de rédaction. |
| [RedactionFilter](./redactionfilter) | Représente un filtre de rédaction, définissant la portée à l'intérieur d'un document pour appliquer les rédactions. |
| [RegexRedaction](./regexredaction) | Représente une rédaction de texte qui recherche et remplace le texte dans le document en faisant correspondre l'expression régulière fournie. |
| [RegionReplacementOptions](./regionreplacementoptions) | Représente les paramètres de couleur et de zone pour le remplacement d'une région d'image. Voir [`ImageAreaRedaction`](../groupdocs.redaction.redactions/imagearearedaction). |
| [RemovePageRedaction](./removepageredaction) | Représente une rédaction qui supprime une page (diapositive, feuille de calcul, etc.) d'un document. |
| [ReplacementOptions](./replacementoptions) | Représente les options pour le remplacement du texte correspondant. |
| [TextRedaction](./textredaction) | Représente une classe abstraite de base pour les rédactions de texte de document. |
| [TextReplacement](./textreplacement) | Représente une information de remplacement textuel. |
## Interfaces

| Interface | Description |
| --- | --- |
| [ICustomRedactionHandler](./icustomredactionhandler) | Fournit une interface pour implémenter une logique de rédaction personnalisée. |
| [IRedactionCallback](./iredactioncallback) | Définit les méthodes requises pour recevoir des informations sur chaque modification de rédaction et éventuellement l'empêcher. |
## Énumération

| Énumération | Description |
| --- | --- |
| [MetadataFilters](./metadatafilters) | Représente une liste des types de métadonnées de document les plus courants. |
| [PageSeekOrigin](./pageseekorigin) | Fournit les champs qui représentent des points de référence dans un document pour la recherche. |
| [RedactionActionType](./redactionactiontype) | Représente les actions qui peuvent être effectuées pour réaliser une rédaction. |
| [RedactionType](./redactiontype) | Représente un type de données du document, affecté par la rédaction. |
| [ReplacementType](./replacementtype) | Représente un type de remplacement pour le texte correspondant. |

<!-- NE PAS MODIFIER : généré par xmldocmd pour GroupDocs.Redaction.dll -->
