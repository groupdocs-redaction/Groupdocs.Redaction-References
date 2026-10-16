---
title: "PreviewOptions"
second_title: "GroupDocs.Redaction for Java API-referentie"
description: "Biedt opties om vereisten en streamdelegaten in te stellen voor het genereren van een preview."
type: docs
weight: 11
url: /nl/java/com.groupdocs.redaction.options/previewoptions/
---
**Inheritance:**
java.lang.Object
```
public class PreviewOptions
```

Biedt opties om vereisten en streamdelegaten in te stellen voor het genereren van een preview.

## Constructors

| Constructor | Beschrijving |
| --- | --- |
|  | [PreviewOptions(ICreatePageStream createPageStream)](#PreviewOptions-com.groupdocs.redaction.options.ICreatePageStream-) | Initialiseert een nieuw exemplaar van de PreviewOptions-klasse, waardoor de uitvoerstroom wordt gesloten. |
|
|  | [PreviewOptions(ICreatePageStream createPageStream, IReleasePageStream releasePageStream)](#PreviewOptions-com.groupdocs.redaction.options.ICreatePageStream-com.groupdocs.redaction.options.IReleasePageStream-) | Initialiseert een nieuw exemplaar van de PreviewOptions-klasse, waardoor de uitvoerstroom wordt teruggegeven aan de client voor verder gebruik. |
|
## Methoden

| Methode | Beschrijving |
| --- | --- |
|  | [getWidth()](#getWidth--) | Haalt of stelt de breedte van de paginavoorbeeld in. |
|
|  | [setWidth(int value)](#setWidth-int-) | Haalt of stelt de breedte van de paginavoorbeeld in. |
|
|  | [getHeight()](#getHeight--) | Haalt of stelt de hoogte van de paginavoorbeeld in. |
|
|  | [setHeight(int value)](#setHeight-int-) | Haalt of stelt de hoogte van de paginavoorbeeld in. |
|
|  | [getPageNumbers()](#getPageNumbers--) | Haalt of stelt een array met paginanummers in om een voorbeeld te genereren. |
|
|  | [setPageNumbers(int[] value)](#setPageNumbers-int---) | Haalt of stelt een array met paginanummers in om een voorbeeld te genereren. |
|
|  | [getPreviewFormat()](#getPreviewFormat--) | Haalt of stelt het formaat van de voorbeeldafbeelding in. |
|
|  | [setPreviewFormat(PreviewFormats value)](#setPreviewFormat-com.groupdocs.redaction.options.PreviewFormats-) | Haalt of stelt het formaat van de voorbeeldafbeelding in. |
|
|  | [getCreatePageStream()](#getCreatePageStream--) | Haalt of stelt een instantie van de paginastroomcreatie‑delegate in. |
|
|  | [setCreatePageStream(ICreatePageStream value)](#setCreatePageStream-com.groupdocs.redaction.options.ICreatePageStream-) | Haalt of stelt een instantie van de paginastroomcreatie‑delegate in. |
|
|  | [getReleasePageStream()](#getReleasePageStream--) | Haalt of stelt een instantie van de paginavoorbeeldvoltooiings‑delegate in. |
|
|  | [setReleasePageStream(IReleasePageStream value)](#setReleasePageStream-com.groupdocs.redaction.options.IReleasePageStream-) | Haalt of stelt een instantie van de paginavoorbeeldvoltooiings‑delegate in. |
|
### PreviewOptions(ICreatePageStream createPageStream) {#PreviewOptions-com.groupdocs.redaction.options.ICreatePageStream-}
```
public PreviewOptions(ICreatePageStream createPageStream)
```


Initialiseert een nieuw exemplaar van de PreviewOptions-klasse, waardoor de uitvoerstroom wordt gesloten.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | createPageStream | [ICreatePageStream](../../com.groupdocs.redaction.options/icreatepagestream) | Maakt een stroom voor een specifiek paginavoorbeeld. |
|

### PreviewOptions(ICreatePageStream createPageStream, IReleasePageStream releasePageStream) {#PreviewOptions-com.groupdocs.redaction.options.ICreatePageStream-com.groupdocs.redaction.options.IReleasePageStream-}
```
public PreviewOptions(ICreatePageStream createPageStream, IReleasePageStream releasePageStream)
```


Initialiseert een nieuw exemplaar van de PreviewOptions-klasse, waardoor de uitvoerstroom wordt teruggegeven aan de client voor verder gebruik.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | createPageStream | [ICreatePageStream](../../com.groupdocs.redaction.options/icreatepagestream) | Maakt een stroom voor een specifiek paginavoorbeeld. |
|
|  | releasePageStream | [IReleasePageStream](../../com.groupdocs.redaction.options/ireleasepagestream) | Meldt dat de generatie van het paginavoorbeeld voltooid is en haalt de uitvoerstroom op. |
|

### getWidth() {#getWidth--}
```
public final int getWidth()
```


Haalt of stelt de breedte van de paginavoorbeeld in.


**Returns:**
int - Paginavoorbeeldbreedte.

### setWidth(int value) {#setWidth-int-}
```
public final void setWidth(int value)
```


Haalt of stelt de breedte van de paginavoorbeeld in.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | waarde | int | Paginavoorbeeldbreedte. |
|

### getHeight() {#getHeight--}
```
public final int getHeight()
```


Haalt of stelt de hoogte van de paginavoorbeeld in.


**Returns:**
int - Paginavoorbeeldhoogte.

### setHeight(int value) {#setHeight-int-}
```
public final void setHeight(int value)
```


Haalt of stelt de hoogte van de paginavoorbeeld in.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | waarde | int | Paginavoorbeeldhoogte. |
|

### getPageNumbers() {#getPageNumbers--}
```
public final int[] getPageNumbers()
```


Haalt of stelt een array met paginanummers in om een voorbeeld te genereren.


**Returns:**
int[] - Een array met paginanummers om een voorbeeld te genereren.

### setPageNumbers(int[] value) {#setPageNumbers-int---}
```
public final void setPageNumbers(int[] value)
```


Haalt of stelt een array met paginanummers in om een voorbeeld te genereren.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | waarde | int[] | Een array met paginanummers om een voorbeeld te genereren. |
|

### getPreviewFormat() {#getPreviewFormat--}
```
public final PreviewFormats getPreviewFormat()
```


Haalt of stelt het formaat van de voorbeeldafbeelding in.


**Returns:**
[PreviewFormats](../../com.groupdocs.redaction.options/previewformats) - Preview image format.

### setPreviewFormat(PreviewFormats value) {#setPreviewFormat-com.groupdocs.redaction.options.PreviewFormats-}
```
public final void setPreviewFormat(PreviewFormats value)
```


Haalt of stelt het formaat van de voorbeeldafbeelding in.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | value | [PreviewFormats](../../com.groupdocs.redaction.options/previewformats) | Voorbeeldafbeeldingsformaat. |
|

### getCreatePageStream() {#getCreatePageStream--}
```
public final ICreatePageStream getCreatePageStream()
```


Haalt of stelt een instantie van de paginastroomcreatie‑delegate in.


**Returns:**
[ICreatePageStream](../../com.groupdocs.redaction.options/icreatepagestream) - An instance of page stream creation delegate.

### setCreatePageStream(ICreatePageStream value) {#setCreatePageStream-com.groupdocs.redaction.options.ICreatePageStream-}
```
public final void setCreatePageStream(ICreatePageStream value)
```


Haalt of stelt een instantie van de paginastroomcreatie‑delegate in.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | value | [ICreatePageStream](../../com.groupdocs.redaction.options/icreatepagestream) | Een instantie van de paginastroomcreatie‑delegate. |
|

### getReleasePageStream() {#getReleasePageStream--}
```
public final IReleasePageStream getReleasePageStream()
```


Haalt of stelt een instantie van de paginavoorbeeldvoltooiings‑delegate in.


**Returns:**
[IReleasePageStream](../../com.groupdocs.redaction.options/ireleasepagestream) - An instance of page preview completion delegate.

### setReleasePageStream(IReleasePageStream value) {#setReleasePageStream-com.groupdocs.redaction.options.IReleasePageStream-}
```
public final void setReleasePageStream(IReleasePageStream value)
```


Haalt of stelt een instantie van de paginavoorbeeldvoltooiings‑delegate in.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | value | [IReleasePageStream](../../com.groupdocs.redaction.options/ireleasepagestream) | Een instantie van de paginavoorbeeldvoltooiings‑delegate. |
|

