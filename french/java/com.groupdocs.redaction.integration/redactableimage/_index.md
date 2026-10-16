---
title: "RedactableImage"
second_title: "Référence API de GroupDocs.Redaction pour Java"
description: "Fournit une façade pour toutes les opérations de suppression d'images raster."
type: docs
weight: 14
url: /fr/java/com.groupdocs.redaction.integration/redactableimage/
---
**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.groupdocs.redaction.integration.IImageFormatInstance](../../com.groupdocs.redaction.integration/iimageformatinstance), [com.groupdocs.redaction.integration.IMultipleAreaRedactable](../../com.groupdocs.redaction.integration/imultiplearearedactable)
```
public class RedactableImage implements IImageFormatInstance, IMultipleAreaRedactable
```

Fournit une façade pour toutes les opérations de suppression d'images raster.

## Constructeurs

| Constructeur | Description |
| --- | --- |
|  | [RedactableImage(IImageFormatInstance img)](#RedactableImage-com.groupdocs.redaction.integration.IImageFormatInstance-) | Crée une nouvelle instance en utilisant un objet, implémentant |
IImageFormatInstance
interface.
|
|  | [RedactableImage(IMultipleAreaRedactable img)](#RedactableImage-com.groupdocs.redaction.integration.IMultipleAreaRedactable-) | Crée une nouvelle instance en utilisant un objet, implémentant |
IMultipleAreaRedactable
interface.
|
## Méthodes

| Méthode | Description |
| --- | --- |
|  | [getRawStream()](#getRawStream--) | Récupère un flux contenant le contenu réel de l'image. |
|
|  | [editAreas(Rectangle[] rectangles, Color boxColor)](#editAreas-java.awt.Rectangle---java.awt.Color-) | Masque plusieurs zones d'image en même temps avec la même couleur. |
|
|  | [editArea(Point topLeft, RegionReplacementOptions options)](#editArea-java.awt.Point-com.groupdocs.redaction.redactions.RegionReplacementOptions-) | Remplace la zone à un point donné par un rectangle de couleur et de taille spécifiques. |
|
### RedactableImage(IImageFormatInstance img) {#RedactableImage-com.groupdocs.redaction.integration.IImageFormatInstance-}
```
public RedactableImage(IImageFormatInstance img)
```


Crée une nouvelle instance en utilisant un objet, implémentant
IImageFormatInstance
interface.


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | img | [IImageFormatInstance](../../com.groupdocs.redaction.integration/iimageformatinstance) | Une instance, implémentant l'interface IImageFormatInstance |
|

### RedactableImage(IMultipleAreaRedactable img) {#RedactableImage-com.groupdocs.redaction.integration.IMultipleAreaRedactable-}
```
public RedactableImage(IMultipleAreaRedactable img)
```


Crée une nouvelle instance en utilisant un objet, implémentant
IMultipleAreaRedactable
interface.


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | img | [IMultipleAreaRedactable](../../com.groupdocs.redaction.integration/imultiplearearedactable) | Une instance, implémentant l'interface IMultipleAreaRedactable |
|

### getRawStream() {#getRawStream--}
```
public final InputStream getRawStream()
```


Récupère un flux contenant le contenu réel de l'image.


**Returns:**
java.io.InputStream - Flux contenant les données d'image

### editAreas(Rectangle[] rectangles, Color boxColor) {#editAreas-java.awt.Rectangle---java.awt.Color-}
```
public final RedactionResult editAreas(Rectangle[] rectangles, Color boxColor)
```


Masque plusieurs zones d'image en même temps avec la même couleur.


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | rectangles | java.awt.Rectangle[] | Un tableau de zones rectangulaires |
|
|  | boxColor | java.awt.Color | Couleur pour remplir les zones |
|

**Returns:**
[RedactionResult](../../com.groupdocs.redaction/redactionresult) - Image areas redaction result

### editArea(Point topLeft, RegionReplacementOptions options) {#editArea-java.awt.Point-com.groupdocs.redaction.redactions.RegionReplacementOptions-}
```
public final RedactionResult editArea(Point topLeft, RegionReplacementOptions options)
```


Remplace la zone à un point donné par un rectangle de couleur et de taille spécifiques.


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | topLeft | java.awt.Point | Coordonnées du coin supérieur gauche de la zone remplie |
|
|  | options | [RegionReplacementOptions](../../com.groupdocs.redaction.redactions/regionreplacementoptions) | Paramètres de couleur et de taille |
|

**Returns:**
[RedactionResult](../../com.groupdocs.redaction/redactionresult) - Image area redaction result

