---
title: "PreviewOptions"
second_title: "GroupDocs.Redaction för Java API-referens"
description: "Tillhandahåller alternativ för att ange krav och strömdelegater för förhandsgranskningsgenerering."
type: docs
weight: 11
url: /sv/java/com.groupdocs.redaction.options/previewoptions/
---
**Inheritance:**
java.lang.Object
```
public class PreviewOptions
```

Tillhandahåller alternativ för att ange krav och strömdelegater för förhandsgranskningsgenerering.

## Konstruktörer

| Konstruktor | Beskrivning |
| --- | --- |
|  | [PreviewOptions(ICreatePageStream createPageStream)](#PreviewOptions-com.groupdocs.redaction.options.ICreatePageStream-) | Initierar en ny instans av klassen PreviewOptions, vilket får utdataflödet att stängas. |
|
|  | [PreviewOptions(ICreatePageStream createPageStream, IReleasePageStream releasePageStream)](#PreviewOptions-com.groupdocs.redaction.options.ICreatePageStream-com.groupdocs.redaction.options.IReleasePageStream-) | Initierar en ny instans av klassen PreviewOptions, vilket får utdataflödet att returneras till klienten för vidare användning. |
|
## Metoder

| Metod | Beskrivning |
| --- | --- |
|  | [getWidth()](#getWidth--) | Hämtar eller anger sidförhandsgranskningsbredd. |
|
|  | [setWidth(int value)](#setWidth-int-) | Hämtar eller anger sidförhandsgranskningsbredd. |
|
|  | [getHeight()](#getHeight--) | Hämtar eller anger sidförhandsgranskningshöjd. |
|
|  | [setHeight(int value)](#setHeight-int-) | Hämtar eller anger sidförhandsgranskningshöjd. |
|
|  | [getPageNumbers()](#getPageNumbers--) | Hämtar eller anger en array med sidnummer för att generera förhandsgranskning. |
|
|  | [setPageNumbers(int[] value)](#setPageNumbers-int---) | Hämtar eller anger en array med sidnummer för att generera förhandsgranskning. |
|
|  | [getPreviewFormat()](#getPreviewFormat--) | Hämtar eller anger format för förhandsgranskningsbild. |
|
|  | [setPreviewFormat(PreviewFormats value)](#setPreviewFormat-com.groupdocs.redaction.options.PreviewFormats-) | Hämtar eller anger format för förhandsgranskningsbild. |
|
|  | [getCreatePageStream()](#getCreatePageStream--) | Hämtar eller anger en instans av delegat för skapande av sidström. |
|
|  | [setCreatePageStream(ICreatePageStream value)](#setCreatePageStream-com.groupdocs.redaction.options.ICreatePageStream-) | Hämtar eller anger en instans av delegat för skapande av sidström. |
|
|  | [getReleasePageStream()](#getReleasePageStream--) | Hämtar eller anger en instans av delegat för slutförande av sidförhandsgranskning. |
|
|  | [setReleasePageStream(IReleasePageStream value)](#setReleasePageStream-com.groupdocs.redaction.options.IReleasePageStream-) | Hämtar eller anger en instans av delegat för slutförande av sidförhandsgranskning. |
|
### PreviewOptions(ICreatePageStream createPageStream) {#PreviewOptions-com.groupdocs.redaction.options.ICreatePageStream-}
```
public PreviewOptions(ICreatePageStream createPageStream)
```


Initierar en ny instans av klassen PreviewOptions, vilket får utdataflödet att stängas.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | createPageStream | [ICreatePageStream](../../com.groupdocs.redaction.options/icreatepagestream) | Skapar en ström för en specifik sidförhandsgranskning |
|

### PreviewOptions(ICreatePageStream createPageStream, IReleasePageStream releasePageStream) {#PreviewOptions-com.groupdocs.redaction.options.ICreatePageStream-com.groupdocs.redaction.options.IReleasePageStream-}
```
public PreviewOptions(ICreatePageStream createPageStream, IReleasePageStream releasePageStream)
```


Initierar en ny instans av klassen PreviewOptions, vilket får utdataflödet att returneras till klienten för vidare användning.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | createPageStream | [ICreatePageStream](../../com.groupdocs.redaction.options/icreatepagestream) | Skapar en ström för en specifik sidförhandsgranskning |
|
|  | releasePageStream | [IReleasePageStream](../../com.groupdocs.redaction.options/ireleasepagestream) | Meddelar att sidförhandsgranskningens generering är klar och hämtar utdataström |
|

### getWidth() {#getWidth--}
```
public final int getWidth()
```


Hämtar eller anger sidförhandsgranskningsbredd.


**Returns:**
int - Sidförhandsgranskningsbredd.

### setWidth(int value) {#setWidth-int-}
```
public final void setWidth(int value)
```


Hämtar eller anger sidförhandsgranskningsbredd.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | värde | int | Sidförhandsgranskningsbredd. |
|

### getHeight() {#getHeight--}
```
public final int getHeight()
```


Hämtar eller anger sidförhandsgranskningshöjd.


**Returns:**
int - Sidförhandsgranskningshöjd.

### setHeight(int value) {#setHeight-int-}
```
public final void setHeight(int value)
```


Hämtar eller anger sidförhandsgranskningshöjd.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | värde | int | Sidförhandsgranskningshöjd. |
|

### getPageNumbers() {#getPageNumbers--}
```
public final int[] getPageNumbers()
```


Hämtar eller anger en array med sidnummer för att generera förhandsgranskning.


**Returns:**
int[] - En array med sidnummer för att generera förhandsgranskning.

### setPageNumbers(int[] value) {#setPageNumbers-int---}
```
public final void setPageNumbers(int[] value)
```


Hämtar eller anger en array med sidnummer för att generera förhandsgranskning.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | värde | int[] | En array med sidnummer för att generera förhandsgranskning. |
|

### getPreviewFormat() {#getPreviewFormat--}
```
public final PreviewFormats getPreviewFormat()
```


Hämtar eller anger format för förhandsgranskningsbild.


**Returns:**
[PreviewFormats](../../com.groupdocs.redaction.options/previewformats) - Preview image format.

### setPreviewFormat(PreviewFormats value) {#setPreviewFormat-com.groupdocs.redaction.options.PreviewFormats-}
```
public final void setPreviewFormat(PreviewFormats value)
```


Hämtar eller anger format för förhandsgranskningsbild.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | value | [PreviewFormats](../../com.groupdocs.redaction.options/previewformats) | Format för förhandsgranskningsbild. |
|

### getCreatePageStream() {#getCreatePageStream--}
```
public final ICreatePageStream getCreatePageStream()
```


Hämtar eller anger en instans av delegat för skapande av sidström.


**Returns:**
[ICreatePageStream](../../com.groupdocs.redaction.options/icreatepagestream) - An instance of page stream creation delegate.

### setCreatePageStream(ICreatePageStream value) {#setCreatePageStream-com.groupdocs.redaction.options.ICreatePageStream-}
```
public final void setCreatePageStream(ICreatePageStream value)
```


Hämtar eller anger en instans av delegat för skapande av sidström.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | value | [ICreatePageStream](../../com.groupdocs.redaction.options/icreatepagestream) | En instans av delegat för skapande av sidström. |
|

### getReleasePageStream() {#getReleasePageStream--}
```
public final IReleasePageStream getReleasePageStream()
```


Hämtar eller anger en instans av delegat för slutförande av sidförhandsgranskning.


**Returns:**
[IReleasePageStream](../../com.groupdocs.redaction.options/ireleasepagestream) - An instance of page preview completion delegate.

### setReleasePageStream(IReleasePageStream value) {#setReleasePageStream-com.groupdocs.redaction.options.IReleasePageStream-}
```
public final void setReleasePageStream(IReleasePageStream value)
```


Hämtar eller anger en instans av delegat för slutförande av sidförhandsgranskning.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | value | [IReleasePageStream](../../com.groupdocs.redaction.options/ireleasepagestream) | En instans av delegat för slutförande av sidförhandsgranskning. |
|

