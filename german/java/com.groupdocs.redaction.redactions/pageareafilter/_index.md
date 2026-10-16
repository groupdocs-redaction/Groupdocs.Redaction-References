---
title: "PageAreaFilter"
second_title: "GroupDocs.Redaction for Java API-Referenz"
description: "Stellt einen Redaktionsfilter dar, der einen Bereich innerhalb einer Seite eines Dokuments festlegt, um eine Redaktion anzuwenden."
type: docs
weight: 22
url: /de/java/com.groupdocs.redaction.redactions/pageareafilter/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.redaction.redactions.RedactionFilter](../../com.groupdocs.redaction.redactions/redactionfilter)
```
public class PageAreaFilter extends RedactionFilter
```

Stellt einen Redaktionsfilter dar, der einen Bereich innerhalb einer Seite eines Dokuments festlegt, in dem die Redaktion angewendet wird.

*** ** * ** ***


**Learn more**

* More details about applying redactions: [Redaction basics](../https://docs.groupdocs.com/redaction/java/redaction-basics/)
* More details about redaction filters: [Use PDF redaction filters](../https://docs.groupdocs.com/redaction/java/use-pdf-redaction-filters/)

<br />


## Konstruktoren

| Konstruktor | Beschreibung |
| --- | --- |
|  | [PageAreaFilter(Point topLeft, Dimension size)](#PageAreaFilter-java.awt.Point-java.awt.Dimension-) | Initialisiert eine neue Instanz der Klasse PageAreaFilter zum Redigieren eines bestimmten Bereichs. |
|
## Methoden

| Methode | Beschreibung |
| --- | --- |
|  | [getRectangle()](#getRectangle--) | Gibt das Rechteck (Position oben links und Größe des Bereichs) auf einer Seite zurück. |
|
|  | [isInTheArea(Rectangle rectangle)](#isInTheArea-java.awt.Rectangle-) | Prüft, ob dieser Filterbereich eine Schnittmenge mit dem angegebenen Rechteck hat. |
|
### PageAreaFilter(Point topLeft, Dimension size) {#PageAreaFilter-java.awt.Point-java.awt.Dimension-}
```
public PageAreaFilter(Point topLeft, Dimension size)
```


Initialisiert eine neue Instanz der Klasse PageAreaFilter zum Redigieren eines bestimmten Bereichs.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | topLeft | java.awt.Point | Koordinaten des Bereichs oben links |
|
|  | size | java.awt.Dimension | Größe und Farbe des Bereichs |
|

### getRectangle() {#getRectangle--}
```
public final Rectangle getRectangle()
```


Gibt das Rechteck (Position oben links und Größe des Bereichs) auf einer Seite zurück.


**Returns:**
java.awt.Rectangle - Das Rechteck (Position oben links und Größe des Bereichs) auf einer Seite.

### isInTheArea(Rectangle rectangle) {#isInTheArea-java.awt.Rectangle-}
```
public final boolean isInTheArea(Rectangle rectangle)
```


Prüft, ob dieser Filterbereich eine Schnittmenge mit dem angegebenen Rechteck hat.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | rectangle | java.awt.Rectangle | Zu prüfendes Rechteck |
|

**Returns:**
boolean - true, wenn dieser Filterbereich eine Schnittmenge hat

