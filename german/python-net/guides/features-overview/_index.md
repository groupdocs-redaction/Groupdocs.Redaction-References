---
title: "Übersicht der Funktionen"
linkTitle: "Features overview"
second_title: "GroupDocs.Redaction für Python über .NET API-Referenzen"
description: "GroupDocs.Redaction für Python über .NET entfernt sensible Informationen aus Dokumenten über eine einheitliche, formatunabhängige API — Text, Metadaten, Bildbereiche, Anmerkungen und ganze Seiten — und speichert das Ergebnis im Originalformat oder als bereinigtes PDF."
type: docs
url: /de/python-net/guides/features-overview/
is_root: false
weight: 30
---


GroupDocs.Redaction für Python über .NET entfernt oder verdeckt dauerhaft sensible Informationen über eine breite Palette von [unterstützten Dokumentformaten](). Jede Redaktion folgt demselben Ablauf: Öffnen Sie ein Dokument mit [`Redactor`](/redaction/python-net/groupdocs.redaction/redactor/), wenden Sie eine oder mehrere Redaktionen mit `apply()` an und anschließend `save()` das bereinigte Ergebnis entweder im Originalformat oder als bereinigtes PDF. Die unten aufgeführten Funktionen können frei in einem Durchgang kombiniert werden.

## Text redaction

Suchen und ersetzen Sie Text anhand einer genauen Phrase oder eines regulären Ausdrucks, wobei sowohl ganze Wörter als auch komplexe Muster wie E‑Mail‑Adressen, Telefonnummern oder nationale Ausweisnummern abgedeckt werden. Gefundener Text kann durch Ersatztext ersetzt oder mit einem farbigen Kasten überdeckt werden, sodass der Originalinhalt nicht wiederhergestellt werden kann. In Tabellenkalkulationen können Sie die Suche auf ein einzelnes Arbeitsblatt oder eine Spalte eingrenzen. Siehe [Text Redactions]().

## Metadata redaction

Löschen oder überschreiben Sie Dokumentmetadaten — Autor, Titel, Unternehmen, Kommentare und EXIF‑Daten in Bildern — damit keine sensiblen Details über Dokumenteigenschaften durchsickern. Sie können alle Metadaten entfernen, bestimmte Felder anvisieren oder Werte durch neue ersetzen. Siehe [Metadata Redactions]().

## Image-area redaction

Schwärzen Sie einen rechteckigen Bereich eines eingebetteten Bildes oder einer gescannten Seite, indem Sie ein gefülltes Kästchen über den angegebenen Bereich zeichnen – nützlich zum Verbergen von Unterschriften, Fotos, Kopf- oder Fußzeilen, in denen vertrauliche Daten erwartet werden. Siehe [Image Redactions]().

## Annotation redaction

Schreiben Sie Anmerkungen, Kommentare und Notizen um oder löschen Sie sie. Sie können jede Anmerkung entfernen oder einen regulären Ausdruck verwenden, um nur die zu finden, die sensible Texte enthalten. Siehe [Annotation Redactions]().

## Page removal

Entfernen Sie ganze Seiten aus PDF-Dokumenten, Folien aus Präsentationen und Arbeitsblätter aus Tabellenkalkulationen. Sie geben eine Startseite und eine Anzahl an, zusammen mit der Richtung relativ zum Ausgangspunkt. Siehe [Remove Page Redactions]().

## Rasterization to PDF

Speichern Sie das bereinigte Dokument als PDF, dessen Seiten als Rasterbilder gerendert werden. Die resultierende Datei enthält keinen durchsuchbaren Text und keine der ursprünglichen Metadaten, sodass der entfernte Inhalt nicht wiederhergestellt werden kann. Rasterisierung ist die richtige Wahl, wenn Sie ein Dokument an Dritte weitergeben oder Vorschriften einhalten müssen, die PDF verlangen. Sie können bestimmte Seiten auswählen und PDF/A‑Konformität über die erweiterten Rasterisierungsoptionen anfordern. Siehe [Save in Rasterized PDF]() und [Advanced Rasterization Options]().

## Redaction policies

Gruppieren Sie mehrere Redaktionen in eine wiederverwendbare Richtlinie und wenden Sie denselben Regel‑Satz konsequent auf viele Dokumente an – ideal für wiederkehrende Aufgaben wie das Bereinigen eines Standardsatzes von Feldern vor der Veröffentlichung. Siehe [Use Redaction Policies]().

## Loading and saving

Laden Sie Dokumente von einem lokalen Pfad oder aus einem Stream, einschließlich passwortgeschützter Dateien, und rasterisieren Sie optional ein Dokument vor der Redaktion. Beim Speichern behalten Sie das Originalformat für weitere Bearbeitung bei, überschreiben die Originaldatei, rasterisieren zu PDF oder schreiben in einen Stream. Siehe [Loading Documents]() und [Saving Documents]().

## On-premise

GroupDocs.Redaction für Python via .NET läuft vollständig in Ihrer eigenen Infrastruktur – Ihre Dokumente verlassen niemals Ihre Umgebung. Das Paket ist ein eigenständiges Wheel, das alles Notwendige bündelt, sodass weder Microsoft Office, OpenOffice, Adobe Acrobat noch eine separate Laufzeit installiert werden muss. Siehe [System Requirements]() für die unterstützten Plattformen und nativen Abhängigkeiten.
