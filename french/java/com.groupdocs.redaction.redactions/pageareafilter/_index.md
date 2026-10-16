---
title: "PageAreaFilter"
second_title: "Référence API de GroupDocs.Redaction pour Java"
description: "Représente un filtre de rédaction définissant une zone au sein d’une page d’un document pour appliquer la rédaction."
type: docs
weight: 22
url: /fr/java/com.groupdocs.redaction.redactions/pageareafilter/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.redaction.redactions.RedactionFilter](../../com.groupdocs.redaction.redactions/redactionfilter)
```
public class PageAreaFilter extends RedactionFilter
```

Représente un filtre de rédaction, définissant une zone au sein d'une page d'un document où appliquer la rédaction.

*** ** * ** ***


**Learn more**

* More details about applying redactions: [Redaction basics](../https://docs.groupdocs.com/redaction/java/redaction-basics/)
* More details about redaction filters: [Use PDF redaction filters](../https://docs.groupdocs.com/redaction/java/use-pdf-redaction-filters/)

<br />


## Constructeurs

| Constructeur | Description |
| --- | --- |
|  | [PageAreaFilter(Point topLeft, Dimension size)](#PageAreaFilter-java.awt.Point-java.awt.Dimension-) | Initialise une nouvelle instance de la classe PageAreaFilter pour rédiger une zone spécifique. |
|
## Méthodes

| Méthode | Description |
| --- | --- |
|  | [getRectangle()](#getRectangle--) | Obtient le rectangle (position en haut à gauche et taille de la zone) sur une page. |
|
|  | [isInTheArea(Rectangle rectangle)](#isInTheArea-java.awt.Rectangle-) | Vérifie si cette zone de filtre intersecte le rectangle donné. |
|
### PageAreaFilter(Point topLeft, Dimension size) {#PageAreaFilter-java.awt.Point-java.awt.Dimension-}
```
public PageAreaFilter(Point topLeft, Dimension size)
```


Initialise une nouvelle instance de la classe PageAreaFilter pour rédiger une zone spécifique.


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | topLeft | java.awt.Point | Coordonnées de la zone en haut à gauche |
|
|  | taille | java.awt.Dimension | Taille et couleur de la zone |
|

### getRectangle() {#getRectangle--}
```
public final Rectangle getRectangle()
```


Obtient le rectangle (position en haut à gauche et taille de la zone) sur une page.


**Returns:**
java.awt.Rectangle - Le rectangle (position en haut à gauche et taille de la zone) sur une page.

### isInTheArea(Rectangle rectangle) {#isInTheArea-java.awt.Rectangle-}
```
public final boolean isInTheArea(Rectangle rectangle)
```


Vérifie si cette zone de filtre intersecte le rectangle donné.


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | rectangle | java.awt.Rectangle | Rectangle à vérifier |
|

**Returns:**
boolean - true, si cette zone de filtre intersecte

