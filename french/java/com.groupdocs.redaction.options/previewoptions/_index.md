---
title: "PreviewOptions"
second_title: "Référence API de GroupDocs.Redaction pour Java"
description: "Fournit des options pour définir les exigences et les délégués de flux pour la génération d'aperçu."
type: docs
weight: 11
url: /fr/java/com.groupdocs.redaction.options/previewoptions/
---
**Inheritance:**
java.lang.Object
```
public class PreviewOptions
```

Fournit des options pour définir les exigences et les délégués de flux pour la génération d'aperçu.

## Constructeurs

| Constructeur | Description |
| --- | --- |
|  | [PreviewOptions(ICreatePageStream createPageStream)](#PreviewOptions-com.groupdocs.redaction.options.ICreatePageStream-) | Initialise une nouvelle instance de la classe PreviewOptions, entraînant la fermeture du flux de sortie. |
|
|  | [PreviewOptions(ICreatePageStream createPageStream, IReleasePageStream releasePageStream)](#PreviewOptions-com.groupdocs.redaction.options.ICreatePageStream-com.groupdocs.redaction.options.IReleasePageStream-) | Initialise une nouvelle instance de la classe PreviewOptions, entraînant le retour du flux de sortie au client pour une utilisation ultérieure. |
|
## Méthodes

| Méthode | Description |
| --- | --- |
|  | [getWidth()](#getWidth--) | Obtient ou définit la largeur de l'aperçu de page. |
|
|  | [setWidth(int value)](#setWidth-int-) | Obtient ou définit la largeur de l'aperçu de page. |
|
|  | [getHeight()](#getHeight--) | Obtient ou définit la hauteur de l'aperçu de page. |
|
|  | [setHeight(int value)](#setHeight-int-) | Obtient ou définit la hauteur de l'aperçu de page. |
|
|  | [getPageNumbers()](#getPageNumbers--) | Obtient ou définit un tableau de numéros de page pour générer l'aperçu. |
|
|  | [setPageNumbers(int[] value)](#setPageNumbers-int---) | Obtient ou définit un tableau de numéros de page pour générer l'aperçu. |
|
|  | [getPreviewFormat()](#getPreviewFormat--) | Obtient ou définit le format de l'image d'aperçu. |
|
|  | [setPreviewFormat(PreviewFormats value)](#setPreviewFormat-com.groupdocs.redaction.options.PreviewFormats-) | Obtient ou définit le format de l'image d'aperçu. |
|
|  | [getCreatePageStream()](#getCreatePageStream--) | Obtient ou définit une instance du délégué de création de flux de page. |
|
|  | [setCreatePageStream(ICreatePageStream value)](#setCreatePageStream-com.groupdocs.redaction.options.ICreatePageStream-) | Obtient ou définit une instance du délégué de création de flux de page. |
|
|  | [getReleasePageStream()](#getReleasePageStream--) | Obtient ou définit une instance du délégué de fin d'aperçu de page. |
|
|  | [setReleasePageStream(IReleasePageStream value)](#setReleasePageStream-com.groupdocs.redaction.options.IReleasePageStream-) | Obtient ou définit une instance du délégué de fin d'aperçu de page. |
|
### PreviewOptions(ICreatePageStream createPageStream) {#PreviewOptions-com.groupdocs.redaction.options.ICreatePageStream-}
```
public PreviewOptions(ICreatePageStream createPageStream)
```


Initialise une nouvelle instance de la classe PreviewOptions, entraînant la fermeture du flux de sortie.


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | createPageStream | [ICreatePageStream](../../com.groupdocs.redaction.options/icreatepagestream) | Crée un flux pour un aperçu de page spécifique |
|

### PreviewOptions(ICreatePageStream createPageStream, IReleasePageStream releasePageStream) {#PreviewOptions-com.groupdocs.redaction.options.ICreatePageStream-com.groupdocs.redaction.options.IReleasePageStream-}
```
public PreviewOptions(ICreatePageStream createPageStream, IReleasePageStream releasePageStream)
```


Initialise une nouvelle instance de la classe PreviewOptions, entraînant le retour du flux de sortie au client pour une utilisation ultérieure.


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | createPageStream | [ICreatePageStream](../../com.groupdocs.redaction.options/icreatepagestream) | Crée un flux pour un aperçu de page spécifique |
|
|  | releasePageStream | [IReleasePageStream](../../com.groupdocs.redaction.options/ireleasepagestream) | Notifie que la génération de l'aperçu de page est terminée et récupère le flux de sortie |
|

### getWidth() {#getWidth--}
```
public final int getWidth()
```


Obtient ou définit la largeur de l'aperçu de page.


**Returns:**
int - Largeur de l'aperçu de page.

### setWidth(int value) {#setWidth-int-}
```
public final void setWidth(int value)
```


Obtient ou définit la largeur de l'aperçu de page.


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | valeur | int | Largeur de l'aperçu de page. |
|

### getHeight() {#getHeight--}
```
public final int getHeight()
```


Obtient ou définit la hauteur de l'aperçu de page.


**Returns:**
int - Hauteur de l'aperçu de page.

### setHeight(int value) {#setHeight-int-}
```
public final void setHeight(int value)
```


Obtient ou définit la hauteur de l'aperçu de page.


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | valeur | int | Hauteur de l'aperçu de page. |
|

### getPageNumbers() {#getPageNumbers--}
```
public final int[] getPageNumbers()
```


Obtient ou définit un tableau de numéros de page pour générer l'aperçu.


**Returns:**
int[] - Un tableau de numéros de page pour générer l'aperçu.

### setPageNumbers(int[] value) {#setPageNumbers-int---}
```
public final void setPageNumbers(int[] value)
```


Obtient ou définit un tableau de numéros de page pour générer l'aperçu.


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | valeur | int[] | Un tableau de numéros de page pour générer l'aperçu. |
|

### getPreviewFormat() {#getPreviewFormat--}
```
public final PreviewFormats getPreviewFormat()
```


Obtient ou définit le format de l'image d'aperçu.


**Returns:**
[PreviewFormats](../../com.groupdocs.redaction.options/previewformats) - Preview image format.

### setPreviewFormat(PreviewFormats value) {#setPreviewFormat-com.groupdocs.redaction.options.PreviewFormats-}
```
public final void setPreviewFormat(PreviewFormats value)
```


Obtient ou définit le format de l'image d'aperçu.


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | value | [PreviewFormats](../../com.groupdocs.redaction.options/previewformats) | Format de l'image d'aperçu. |
|

### getCreatePageStream() {#getCreatePageStream--}
```
public final ICreatePageStream getCreatePageStream()
```


Obtient ou définit une instance du délégué de création de flux de page.


**Returns:**
[ICreatePageStream](../../com.groupdocs.redaction.options/icreatepagestream) - An instance of page stream creation delegate.

### setCreatePageStream(ICreatePageStream value) {#setCreatePageStream-com.groupdocs.redaction.options.ICreatePageStream-}
```
public final void setCreatePageStream(ICreatePageStream value)
```


Obtient ou définit une instance du délégué de création de flux de page.


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | value | [ICreatePageStream](../../com.groupdocs.redaction.options/icreatepagestream) | Une instance du délégué de création de flux de page. |
|

### getReleasePageStream() {#getReleasePageStream--}
```
public final IReleasePageStream getReleasePageStream()
```


Obtient ou définit une instance du délégué de fin d'aperçu de page.


**Returns:**
[IReleasePageStream](../../com.groupdocs.redaction.options/ireleasepagestream) - An instance of page preview completion delegate.

### setReleasePageStream(IReleasePageStream value) {#setReleasePageStream-com.groupdocs.redaction.options.IReleasePageStream-}
```
public final void setReleasePageStream(IReleasePageStream value)
```


Obtient ou définit une instance du délégué de fin d'aperçu de page.


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | value | [IReleasePageStream](../../com.groupdocs.redaction.options/ireleasepagestream) | Une instance du délégué de fin d'aperçu de page. |
|

