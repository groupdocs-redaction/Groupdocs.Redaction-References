---
title: "GroupDocs.Redaction.Options"
second_title: "Référence API de GroupDocs.Redaction pour .NET"
description: "L’espace de noms Options fournit des classes d’options de chargement et d’enregistrement."
type: docs
weight: 60
url: /fr/net/groupdocs.redaction.options/
---
L’espace de noms Options fournit des classes d’options de chargement et d’enregistrement.

## Classes

| Classe | Description |
| --- | --- |
| [CreatePageStream](./createpagestream) | Représente une méthode qui renvoie un flux pour écrire les données d'aperçu de page. |
| [LoadOptions](./loadoptions) | Fournit des options qui seront utilisées pour ouvrir un fichier. |
| [PreviewOptions](./previewoptions) | Fournit des options pour définir les exigences et les délégués de flux pour la génération d'aperçus. |
| [RasterizationOptions](./rasterizationoptions) | Fournit des options pour convertir des fichiers en PDF. |
| [RedactorSettings](./redactorsettings) | Représente les paramètres de rédaction, permettant de personnaliser le processus de rédaction. |
| [ReleasePageStream](./releasepagestream) | Représente une méthode qui libère le flux créé par le délégué [`CreatePageStream`](../groupdocs.redaction.options/createpagestream). |
| [SaveOptions](./saveoptions) | Fournit des options pour modifier le nom du fichier de sortie et/ou convertir le document en PDF basé sur des images (rasterisation). |
| [WordprocessingSaveOptions](./wordprocessingsaveoptions) | Fournit des options d'enregistrement pour les documents de traitement de texte. |
## Interfaces

| Interface | Description |
| --- | --- |
| [ILogger](./ilogger) | Définit l'interface d'un logger qui peut être utilisé pour consigner les événements et les erreurs lors du processus de rédaction. |
## Énumération

| Énumération | Description |
| --- | --- |
| [AdvancedRasterizationOptions](./advancedrasterizationoptions) | Énumération de drapeaux pour gérer les options avancées de rasterisation à appliquer. |
| [PdfComplianceLevel](./pdfcompliancelevel) | Représente une liste des niveaux de conformité PDF pris en charge. |
| [PreviewOptions.PreviewFormats](./previewoptions.previewformats) | Représente les formats d'aperçu pris en charge. |
| [WordProcessingComplianceLevel](./wordprocessingcompliancelevel) | Représente les niveaux de conformité OOXML pris en charge pour les documents de traitement de texte. Le niveau de conformité Strict ne peut être rétrogradé qu'en Transitional, pas en Ecma. |

<!-- NE PAS MODIFIER : généré par xmldocmd pour GroupDocs.Redaction.dll -->
