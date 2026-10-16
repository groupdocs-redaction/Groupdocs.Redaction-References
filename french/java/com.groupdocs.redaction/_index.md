---
title: "com.groupdocs.redaction"
second_title: "Référence API de GroupDocs.Redaction pour Java"
description: "Le package fournit des classes pour supprimer les informations sensibles des documents aux formats PDF, image raster et documents Office."
type: docs
weight: 10
url: /fr/java/com.groupdocs.redaction/
---

Le package fournit des classes pour caviarder les informations sensibles des documents aux formats PDF, image raster et Office.

Les principales classes de ce package sont :

<br />

* [Redactor](../../com.groupdocs.redaction/redactor) is the entry point for redaction process.
* [Redaction](../../com.groupdocs.redaction/redaction) is abstract base class for all types of document redactions.
* [RedactionPolicy](../../com.groupdocs.redaction/redactionpolicy) is pre-configured in XML set of redaction rules.
* [RedactorChangeLog](../../com.groupdocs.redaction/redactorchangelog) provides information about redaction process results.

<br />




## Classes

| Classe | Description |
| --- | --- |
| [DocumentInfo](../com.groupdocs.redaction/documentinfo) | Représente une information sur le document. |
| [FileType](../com.groupdocs.redaction/filetype) | Représente un type de fichier. |
| [PageInfo](../com.groupdocs.redaction/pageinfo) | Représente une brève information de page. |
| [Redaction](../com.groupdocs.redaction/redaction) | Représente une classe abstraite de base pour tous les types de rédaction. |
| [RedactionPolicy](../com.groupdocs.redaction/redactionpolicy) | Représente une politique de désinfection, contenant un ensemble de rédactions spécifiques à appliquer. |
| [RedactionResult](../com.groupdocs.redaction/redactionresult) | Représente un résultat de l'opération de rédaction. |
| [Redactor](../com.groupdocs.redaction/redactor) | Représente la classe principale qui contrôle le processus de rédaction de documents, permettant d'ouvrir, de rédiger et d'enregistrer les documents. |
| [RedactorChangeLog](../com.groupdocs.redaction/redactorchangelog) | Représente les résultats d'une liste de rédactions, transmis à la méthode Apply() de la classe Redactor. |
| [RedactorLogEntry](../com.groupdocs.redaction/redactorlogentry) | Représente les résultats de l'application de la rédaction. |

## Interfaces

| Interface | Description |
| --- | --- |
| [IDocumentInfo](../com.groupdocs.redaction/idocumentinfo) | Définit les méthodes requises pour obtenir les informations de base du document. |

## Énumérations

| Énum | Description |
| --- | --- |
| [RedactionStatus](../com.groupdocs.redaction/redactionstatus) | Représente un statut d'achèvement de la rédaction. |
