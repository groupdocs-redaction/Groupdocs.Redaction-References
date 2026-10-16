---
title: "com.groupdocs.redaction.options"
second_title: "Référence API de GroupDocs.Redaction pour Java"
description: "Le package fournit des classes d'options de chargement et d'enregistrement."
type: docs
weight: 15
url: /fr/java/com.groupdocs.redaction.options/
---

Le package fournit des classes d'options de chargement et d'enregistrement.



## Classes

| Classe | Description |
| --- | --- |
| [LoadOptions](../com.groupdocs.redaction.options/loadoptions) | Fournit des options qui seront utilisées pour ouvrir un fichier. |
| [PreviewOptions](../com.groupdocs.redaction.options/previewoptions) | Fournit des options pour définir les exigences et les délégués de flux pour la génération d'aperçu. |
| [RasterizationOptions](../com.groupdocs.redaction.options/rasterizationoptions) | Fournit des options pour convertir des fichiers en PDF. |
| [RedactorSettings](../com.groupdocs.redaction.options/redactorsettings) | Représente les paramètres de rédaction, permettant de personnaliser le processus de rédaction. |
| [SaveOptions](../com.groupdocs.redaction.options/saveoptions) | Fournit des options pour modifier le nom du fichier de sortie et/ou convertir le document en PDF basé sur des images (rasterisation). |
| [WordprocessingSaveOptions](../com.groupdocs.redaction.options/wordprocessingsaveoptions) | Options d'enregistrement du traitement de texte. |

## Interfaces

| Interface | Description |
| --- | --- |
| [ICreatePageStream](../com.groupdocs.redaction.options/icreatepagestream) | Fournit une méthode qui renvoie un flux pour écrire les données d'aperçu de page. |
| [ILogger](../com.groupdocs.redaction.options/ilogger) | Définit l'interface d'un journaliseur qui peut être utilisé pour consigner les événements et les erreurs lors du processus de rédaction. |
| [IReleasePageStream](../com.groupdocs.redaction.options/ireleasepagestream) | Représente une méthode qui libère le flux créé par le délégué CreatePageStream. |

## Énumérations

| Énum | Description |
| --- | --- |
| [AdvancedRasterizationOptions](../com.groupdocs.redaction.options/advancedrasterizationoptions) | Une énumération pour gérer les options avancées de rasterisation à appliquer. |
| [PdfComplianceLevel](../com.groupdocs.redaction.options/pdfcompliancelevel) | Représente une liste des niveaux de conformité PDF pris en charge. |
| [PreviewFormats](../com.groupdocs.redaction.options/previewformats) | Représente les formats d'aperçu pris en charge. |
| [WordProcessingComplianceLevel](../com.groupdocs.redaction.options/wordprocessingcompliancelevel) | Niveaux de conformité OOXML pour les documents de traitement de texte. |
