---
title: "groupdocs.redaction.redactions"
second_title: "Références API de GroupDocs.Redaction pour Python via .NET"
description: "Types sous groupdocs.redaction.redactions."
type: docs
url: /fr/python-net/groupdocs.redaction.redactions/
is_root: false
weight: 60
---


Types sous `groupdocs.redaction.redactions`.

### Classes
| Classe | Description |
| :- | :- |
| [`AnnotationRedaction`](/redaction/python-net/groupdocs.redaction.redactions/annotationredaction/) | Représente un caviardage qui remplace le texte des annotations (commentaires, etc.) correspondant à une expression régulière donnée. |
| [`CellColumnRedaction`](/redaction/python-net/groupdocs.redaction.redactions/cellcolumnredaction/) | Représente un caviardage de texte qui remplace le texte dans un document de feuille de calcul (CSV, Excel, etc.). |
| [`CellFilter`](/redaction/python-net/groupdocs.redaction.redactions/cellfilter/) | Fournit une option pour limiter la portée d'un [`CellColumnRedaction`](/redaction/python-net/groupdocs.redaction.redactions/cellcolumnredaction/) à une feuille de calcul et à une colonne. |
| [`CustomRedactionContext`](/redaction/python-net/groupdocs.redaction.redactions/customredactioncontext/) | Fournit le contexte pour le traitement personnalisé du caviardage. |
| [`CustomRedactionResult`](/redaction/python-net/groupdocs.redaction.redactions/customredactionresult/) | Représente le résultat d'une opération de caviardage personnalisée. |
| [`DeleteAnnotationRedaction`](/redaction/python-net/groupdocs.redaction.redactions/deleteannotationredaction/) | Représente un caviardage de texte qui supprime les annotations si le texte correspond à une expression régulière donnée (supprime éventuellement toutes les annotations). |
| [`EraseMetadataRedaction`](/redaction/python-net/groupdocs.redaction.redactions/erasemetadataredaction/) | Représente un caviardage de métadonnées qui efface toutes les métadonnées ou les métadonnées correspondant à des filtres MetadataFilters spécifiques du document. |
| [`ExactPhraseRedaction`](/redaction/python-net/groupdocs.redaction.redactions/exactphraseredaction/) | Représente un caviardage de texte qui remplace une phrase exacte dans le texte du document, insensible à la casse par défaut. |
| [`ICustomRedactionHandler`](/redaction/python-net/groupdocs.redaction.redactions/icustomredactionhandler/) | Fournit une interface pour implémenter une logique de caviardage personnalisée. |
| [`IRedactionCallback`](/redaction/python-net/groupdocs.redaction.redactions/iredactioncallback/) | Définit les méthodes requises pour recevoir des informations sur chaque modification de rédaction et, éventuellement, l'empêcher. |
| [`ImageAreaRedaction`](/redaction/python-net/groupdocs.redaction.redactions/imagearearedaction/) | Représente une rédaction qui place un rectangle coloré dans une zone donnée d'un document image. |
| [`MetadataRedaction`](/redaction/python-net/groupdocs.redaction.redactions/metadataredaction/) | Représente une classe abstraite de base pour les rédactions de métadonnées de document. |
| [`MetadataSearchRedaction`](/redaction/python-net/groupdocs.redaction.redactions/metadatasearchredaction/) | Représente une rédaction de métadonnées qui recherche et censure les métadonnées en utilisant des expressions régulières, en faisant correspondre les clés et/ou les valeurs. |
| [`PageAreaFilter`](/redaction/python-net/groupdocs.redaction.redactions/pageareafilter/) | Représente un filtre de rédaction, définissant une zone à l'intérieur d'une page d'un document pour appliquer la rédaction. |
| [`PageAreaRedaction`](/redaction/python-net/groupdocs.redaction.redactions/pagearearedaction/) | Représente une rédaction textuelle complexe qui affecte le texte, les images et les annotations dans une zone de la page. |
| [`PageRangeFilter`](/redaction/python-net/groupdocs.redaction.redactions/pagerangefilter/) | Représente un filtre de rédaction, définissant une plage de pages à l'intérieur d'un document pour appliquer la rédaction. |
| [`RedactionDescription`](/redaction/python-net/groupdocs.redaction.redactions/redactiondescription/) | Représente une information sur une action de modification unique effectuée pendant le processus de rédaction. |
| [`RegexRedaction`](/redaction/python-net/groupdocs.redaction.redactions/regexredaction/) | Représente une rédaction de texte qui recherche et remplace le texte dans le document en faisant correspondre l'expression régulière fournie. |
| [`RegionReplacementOptions`](/redaction/python-net/groupdocs.redaction.redactions/regionreplacementoptions/) | Représente les paramètres de couleur et de zone pour le remplacement d'une région d'image. |
| [`RemovePageRedaction`](/redaction/python-net/groupdocs.redaction.redactions/removepageredaction/) | Représente une rédaction qui supprime une page (diapositive, feuille de calcul, etc.) d'un document. |
| [`ReplacementOptions`](/redaction/python-net/groupdocs.redaction.redactions/replacementoptions/) | Représente les options pour le remplacement du texte correspondant. |
| [`TextRedaction`](/redaction/python-net/groupdocs.redaction.redactions/textredaction/) | Représente une classe abstraite de base pour les rédactions de texte de document. |
| [`TextReplacement`](/redaction/python-net/groupdocs.redaction.redactions/textreplacement/) | Représente une information de remplacement textuel. |

### Énumérations
| Énum | Description |
| :- | :- |
| [`MetadataFilters`](/redaction/python-net/groupdocs.redaction.redactions/metadatafilters/) |  |
| [`PageSeekOrigin`](/redaction/python-net/groupdocs.redaction.redactions/pageseekorigin/) |  |
| [`RedactionActionType`](/redaction/python-net/groupdocs.redaction.redactions/redactionactiontype/) |  |
| [`RedactionFilter`](/redaction/python-net/groupdocs.redaction.redactions/redactionfilter/) | Représente un filtre de rédaction, définissant la portée à l'intérieur d'un document pour appliquer les rédactions. |
| [`RedactionType`](/redaction/python-net/groupdocs.redaction.redactions/redactiontype/) |  |
| [`ReplacementType`](/redaction/python-net/groupdocs.redaction.redactions/replacementtype/) |  |
