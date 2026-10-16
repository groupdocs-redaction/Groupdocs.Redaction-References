---
title: "MetadataFilters"
second_title: "Référence API de GroupDocs.Redaction pour Java"
description: "Représente une liste des types de métadonnées de document les plus courants."
type: docs
weight: 19
url: /fr/java/com.groupdocs.redaction.redactions/metadatafilters/
---
**Inheritance:**
java.lang.Object
```
public final class MetadataFilters
```

Représente une liste des types de métadonnées de document les plus courants.

## Constructeurs

| Constructeur | Description |
| --- | --- |
| [MetadataFilters()](#MetadataFilters--) |  |
## Champs

| Champ | Description |
| --- | --- |
|  | [None](#None) | Paramètre de filtre vide, ne correspond à aucun élément de métadonnées. |
|
|  | [Author](#Author) | Auteur du document. |
|
|  | [Category](#Category) | Catégorie du document. |
|
|  | [Comments](#Comments) | Commentaire du document. |
|
|  | [Company](#Company) | Entreprise de l'Auteur. |
|
|  | [ContentStatus](#ContentStatus) | Statut du contenu. |
|
|  | [CreatedTime](#CreatedTime) | Heure de création. |
|
|  | [HyperlinkBase](#HyperlinkBase) | Base du lien hypertexte. |
|
|  | [LastPrinted](#LastPrinted) | Date et heure de la dernière impression. |
|
|  | [LastSavedBy](#LastSavedBy) | Dernière sauvegarde par l'utilisateur. |
|
|  | [LastSavedTime](#LastSavedTime) | Date et heure de la dernière sauvegarde. |
|
|  | [NameOfApplication](#NameOfApplication) | Nom de l'application où le document a été créé. |
|
|  | [Manager](#Manager) | Nom du responsable de l'Auteur. |
|
|  | [RevisionNumber](#RevisionNumber) | Numéro de révision. |
|
|  | [Subject](#Subject) | Sujet du document. |
|
|  | [Template](#Template) | Nom du modèle de document. |
|
|  | [Title](#Title) | Titre du document. |
|
|  | [TotalEditingTime](#TotalEditingTime) | Temps total d'édition. |
|
|  | [Version](#Version) | Version du document. |
|
|  | [Description](#Description) | Description du document. |
|
|  | [Keywords](#Keywords) | Mots-clés du document. |
|
|  | [ContentType](#ContentType) | Type de contenu. |
|
|  | [All](#All) | Tous les types des éléments de métadonnées. |
|
## Méthodes

| Méthode | Description |
| --- | --- |
|  | [getNames()](#getNames--) | Obtient un ensemble avec tous les types de filtres déclarés. |
|
|  | [getValueByName(String valueName)](#getValueByName-java.lang.String-) | Obtient la valeur de MetadataFiler par son nom. |
|
|  | [parse(String values)](#parse-java.lang.String-) | Analyse une chaîne de valeurs de MetadataFilers séparées par des virgules en un entier. |
|
|  | [toString(int value)](#toString-int-) | Enregistre un entier sous forme de chaîne de valeurs de MetadataFilers séparées par des virgules. |
|
### MetadataFilters() {#MetadataFilters--}
```
public MetadataFilters()
```


### None {#None}
```
public static final int None
```


Paramètre de filtre vide, ne correspond à aucun élément de métadonnées.


### Author {#Author}
```
public static final int Author
```


Auteur du document.


### Category {#Category}
```
public static final int Category
```


Catégorie du document.


### Comments {#Comments}
```
public static final int Comments
```


Commentaire du document.


### Company {#Company}
```
public static final int Company
```


Entreprise de l'Auteur.


### ContentStatus {#ContentStatus}
```
public static final int ContentStatus
```


Statut du contenu.


### CreatedTime {#CreatedTime}
```
public static final int CreatedTime
```


Heure de création.


### HyperlinkBase {#HyperlinkBase}
```
public static final int HyperlinkBase
```


Base du lien hypertexte.


### LastPrinted {#LastPrinted}
```
public static final int LastPrinted
```


Date et heure de la dernière impression.


### LastSavedBy {#LastSavedBy}
```
public static final int LastSavedBy
```


Dernière sauvegarde par l'utilisateur.


### LastSavedTime {#LastSavedTime}
```
public static final int LastSavedTime
```


Date et heure de la dernière sauvegarde.


### NameOfApplication {#NameOfApplication}
```
public static final int NameOfApplication
```


Nom de l'application où le document a été créé.


### Manager {#Manager}
```
public static final int Manager
```


Nom du responsable de l'Auteur.


### RevisionNumber {#RevisionNumber}
```
public static final int RevisionNumber
```


Numéro de révision.


### Subject {#Subject}
```
public static final int Subject
```


Sujet du document.


### Template {#Template}
```
public static final int Template
```


Nom du modèle de document.


### Title {#Title}
```
public static final int Title
```


Titre du document.


### TotalEditingTime {#TotalEditingTime}
```
public static final int TotalEditingTime
```


Temps total d'édition.


### Version {#Version}
```
public static final int Version
```


Version du document.


### Description {#Description}
```
public static final int Description
```


Description du document.


### Keywords {#Keywords}
```
public static final int Keywords
```


Mots-clés du document.


### ContentType {#ContentType}
```
public static final int ContentType
```


Type de contenu.


### All {#All}
```
public static final int All
```


Tous les types des éléments de métadonnées.


### getNames() {#getNames--}
```
public static Set<String> getNames()
```


Obtient un ensemble avec tous les types de filtres déclarés.


**Returns:**
java.util.Set<java.lang.String> - Un ensemble contenant tous les types de filtres déclarés.

### getValueByName(String valueName) {#getValueByName-java.lang.String-}
```
public static int getValueByName(String valueName)
```


Obtient la valeur de MetadataFiler par son nom.


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | valueName | java.lang.String | Nom du MetadataFilter. |
|

**Returns:**
int - Valeur du MetadataFiler.

### parse(String values) {#parse-java.lang.String-}
```
public static int parse(String values)
```


Analyse une chaîne de valeurs de MetadataFilers séparées par des virgules en un entier.


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | values | java.lang.String | Une chaîne de valeurs de MetadataFilers séparées par des virgules. |
|

**Returns:**
int - Valeur des MetadataFilers.

### toString(int value) {#toString-int-}
```
public static String toString(int value)
```


Enregistre un entier sous forme de chaîne de valeurs de MetadataFilers séparées par des virgules.


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | valeur | int | Valeur du MetadataFiler. |
|

**Returns:**
java.lang.String - Une chaîne de valeurs de MetadataFiler séparées par des virgules.

