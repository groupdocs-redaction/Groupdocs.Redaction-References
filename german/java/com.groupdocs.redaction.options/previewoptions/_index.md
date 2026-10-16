---
title: "PreviewOptions"
second_title: "GroupDocs.Redaction for Java API-Referenz"
description: "Stellt Optionen bereit, um Anforderungen und Stream-Delegaten für die Vorschauerstellung festzulegen."
type: docs
weight: 11
url: /de/java/com.groupdocs.redaction.options/previewoptions/
---
**Inheritance:**
java.lang.Object
```
public class PreviewOptions
```

Stellt Optionen bereit, um Anforderungen und Stream-Delegaten für die Vorschauerstellung festzulegen.

## Konstruktoren

| Konstruktor | Beschreibung |
| --- | --- |
|  | [PreviewOptions(ICreatePageStream createPageStream)](#PreviewOptions-com.groupdocs.redaction.options.ICreatePageStream-) | Initialisiert eine neue Instanz der Klasse PreviewOptions, wodurch der Ausgabestream geschlossen wird. |
|
|  | [PreviewOptions(ICreatePageStream createPageStream, IReleasePageStream releasePageStream)](#PreviewOptions-com.groupdocs.redaction.options.ICreatePageStream-com.groupdocs.redaction.options.IReleasePageStream-) | Initialisiert eine neue Instanz der Klasse PreviewOptions, wodurch der Ausgabestream dem Client zur weiteren Verwendung zurückgegeben wird. |
|
## Methoden

| Methode | Beschreibung |
| --- | --- |
|  | [getWidth()](#getWidth--) | Liest oder setzt die Breite der Seitenvorschau. |
|
|  | [setWidth(int value)](#setWidth-int-) | Liest oder setzt die Breite der Seitenvorschau. |
|
|  | [getHeight()](#getHeight--) | Liest oder setzt die Höhe der Seitenvorschau. |
|
|  | [setHeight(int value)](#setHeight-int-) | Liest oder setzt die Höhe der Seitenvorschau. |
|
|  | [getPageNumbers()](#getPageNumbers--) | Liest oder setzt ein Array von Seitenzahlen, für die eine Vorschau erzeugt werden soll. |
|
|  | [setPageNumbers(int[] value)](#setPageNumbers-int---) | Liest oder setzt ein Array von Seitenzahlen, für die eine Vorschau erzeugt werden soll. |
|
|  | [getPreviewFormat()](#getPreviewFormat--) | Liest oder setzt das Bildformat der Vorschau. |
|
|  | [setPreviewFormat(PreviewFormats value)](#setPreviewFormat-com.groupdocs.redaction.options.PreviewFormats-) | Liest oder setzt das Bildformat der Vorschau. |
|
|  | [getCreatePageStream()](#getCreatePageStream--) | Liest oder setzt eine Instanz des Delegaten zur Erstellung des Seitenstreams. |
|
|  | [setCreatePageStream(ICreatePageStream value)](#setCreatePageStream-com.groupdocs.redaction.options.ICreatePageStream-) | Liest oder setzt eine Instanz des Delegaten zur Erstellung des Seitenstreams. |
|
|  | [getReleasePageStream()](#getReleasePageStream--) | Liest oder setzt eine Instanz des Delegaten für den Abschluss der Seitenvorschau. |
|
|  | [setReleasePageStream(IReleasePageStream value)](#setReleasePageStream-com.groupdocs.redaction.options.IReleasePageStream-) | Liest oder setzt eine Instanz des Delegaten für den Abschluss der Seitenvorschau. |
|
### PreviewOptions(ICreatePageStream createPageStream) {#PreviewOptions-com.groupdocs.redaction.options.ICreatePageStream-}
```
public PreviewOptions(ICreatePageStream createPageStream)
```


Initialisiert eine neue Instanz der Klasse PreviewOptions, wodurch der Ausgabestream geschlossen wird.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | createPageStream | [ICreatePageStream](../../com.groupdocs.redaction.options/icreatepagestream) | Erstellt einen Stream für eine bestimmte Seitenvorschau |
|

### PreviewOptions(ICreatePageStream createPageStream, IReleasePageStream releasePageStream) {#PreviewOptions-com.groupdocs.redaction.options.ICreatePageStream-com.groupdocs.redaction.options.IReleasePageStream-}
```
public PreviewOptions(ICreatePageStream createPageStream, IReleasePageStream releasePageStream)
```


Initialisiert eine neue Instanz der Klasse PreviewOptions, wodurch der Ausgabestream dem Client zur weiteren Verwendung zurückgegeben wird.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | createPageStream | [ICreatePageStream](../../com.groupdocs.redaction.options/icreatepagestream) | Erstellt einen Stream für eine bestimmte Seitenvorschau |
|
|  | releasePageStream | [IReleasePageStream](../../com.groupdocs.redaction.options/ireleasepagestream) | Benachrichtigt, dass die Erzeugung der Seitenvorschau abgeschlossen ist und gibt den Ausgabestream zurück |
|

### getWidth() {#getWidth--}
```
public final int getWidth()
```


Liest oder setzt die Breite der Seitenvorschau.


**Returns:**
int - Breite der Seitenvorschau.

### setWidth(int value) {#setWidth-int-}
```
public final void setWidth(int value)
```


Liest oder setzt die Breite der Seitenvorschau.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | Wert | int | Breite der Seitenvorschau. |
|

### getHeight() {#getHeight--}
```
public final int getHeight()
```


Liest oder setzt die Höhe der Seitenvorschau.


**Returns:**
int - Höhe der Seitenvorschau.

### setHeight(int value) {#setHeight-int-}
```
public final void setHeight(int value)
```


Liest oder setzt die Höhe der Seitenvorschau.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | Wert | int | Höhe der Seitenvorschau. |
|

### getPageNumbers() {#getPageNumbers--}
```
public final int[] getPageNumbers()
```


Liest oder setzt ein Array von Seitenzahlen, für die eine Vorschau erzeugt werden soll.


**Returns:**
int[] - Ein Array von Seitenzahlen, um eine Vorschau zu erzeugen.

### setPageNumbers(int[] value) {#setPageNumbers-int---}
```
public final void setPageNumbers(int[] value)
```


Liest oder setzt ein Array von Seitenzahlen, für die eine Vorschau erzeugt werden soll.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | Wert | int[] | Ein Array von Seitenzahlen, um eine Vorschau zu erzeugen. |
|

### getPreviewFormat() {#getPreviewFormat--}
```
public final PreviewFormats getPreviewFormat()
```


Liest oder setzt das Bildformat der Vorschau.


**Returns:**
[PreviewFormats](../../com.groupdocs.redaction.options/previewformats) - Preview image format.

### setPreviewFormat(PreviewFormats value) {#setPreviewFormat-com.groupdocs.redaction.options.PreviewFormats-}
```
public final void setPreviewFormat(PreviewFormats value)
```


Liest oder setzt das Bildformat der Vorschau.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | value | [PreviewFormats](../../com.groupdocs.redaction.options/previewformats) | Vorschau-Bildformat. |
|

### getCreatePageStream() {#getCreatePageStream--}
```
public final ICreatePageStream getCreatePageStream()
```


Liest oder setzt eine Instanz des Delegaten zur Erstellung des Seitenstreams.


**Returns:**
[ICreatePageStream](../../com.groupdocs.redaction.options/icreatepagestream) - An instance of page stream creation delegate.

### setCreatePageStream(ICreatePageStream value) {#setCreatePageStream-com.groupdocs.redaction.options.ICreatePageStream-}
```
public final void setCreatePageStream(ICreatePageStream value)
```


Liest oder setzt eine Instanz des Delegaten zur Erstellung des Seitenstreams.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | value | [ICreatePageStream](../../com.groupdocs.redaction.options/icreatepagestream) | Eine Instanz des Delegaten zur Erstellung des Seitenstroms. |
|

### getReleasePageStream() {#getReleasePageStream--}
```
public final IReleasePageStream getReleasePageStream()
```


Liest oder setzt eine Instanz des Delegaten für den Abschluss der Seitenvorschau.


**Returns:**
[IReleasePageStream](../../com.groupdocs.redaction.options/ireleasepagestream) - An instance of page preview completion delegate.

### setReleasePageStream(IReleasePageStream value) {#setReleasePageStream-com.groupdocs.redaction.options.IReleasePageStream-}
```
public final void setReleasePageStream(IReleasePageStream value)
```


Liest oder setzt eine Instanz des Delegaten für den Abschluss der Seitenvorschau.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | value | [IReleasePageStream](../../com.groupdocs.redaction.options/ireleasepagestream) | Eine Instanz des Delegaten zum Abschluss der Seitenvorschau. |
|

