---
title: "Overzicht van functies"
linkTitle: "Features overview"
second_title: "GroupDocs.Redaction voor Python via .NET API-referenties"
description: "GroupDocs.Redaction voor Python via .NET verwijdert gevoelige informatie uit documenten via een enkele, formaat‑onafhankelijke API — tekst, metadata, afbeeldingsgebieden, annotaties en volledige pagina's — en slaat het resultaat op in het oorspronkelijke formaat of als een gesaniteerde PDF."
type: docs
url: /nl/python-net/guides/features-overview/
is_root: false
weight: 30
---


GroupDocs.Redaction voor Python via .NET verwijdert of maakt permanent onleesbaar gevoelige informatie over een breed scala aan [supported document formats](). Elke redactie volgt dezelfde workflow: open een document met [`Redactor`](/redaction/python-net/groupdocs.redaction/redactor/), pas een of meer redacties toe met `apply()`, vervolgens `save()` je het opgeschoonde resultaat ofwel in het oorspronkelijke formaat of als een gesaniteerde PDF. De onderstaande mogelijkheden kunnen vrij worden gecombineerd in één doorloop.

## Text redaction

Zoek en vervang tekst met een exacte frase of met een reguliere expressie, waarbij zowel volledige woorden als complexe patronen zoals e‑mailadressen, telefoonnummers of nationale ID‑nummers worden gedekt. Geselecteerde tekst kan worden vervangen door vervangende tekst of worden afgedekt met een gekleurde doos zodat de oorspronkelijke inhoud niet kan worden hersteld. In spreadsheets kun je de zoekopdracht beperken tot één werkblad of kolom. Zie [Text Redactions]().

## Metadata redaction

Wis of herschrijf documentmetadata — auteur, titel, bedrijf, opmerkingen en EXIF‑gegevens op afbeeldingen — zodat geen gevoelige details via documenteigenschappen lekken. Je kunt alle metadata wissen, specifieke velden selecteren, of waarden vervangen door nieuwe. Zie [Metadata Redactions]().

## Image-area redaction

Maak een rechthoekig gebied van een ingesloten afbeelding of een gescande pagina zwart door een gevulde doos over een bepaald gebied te tekenen — handig om handtekeningen, foto’s, kopteksten of voetteksten te verbergen waar vertrouwelijke gegevens kunnen verschijnen. Zie [Image Redactions]().

## Annotation redaction

Herschrijf of verwijder annotaties, opmerkingen en notities. Je kunt elke annotatie verwijderen of een reguliere expressie gebruiken om alleen diegene te selecteren die gevoelige tekst bevatten. Zie [Annotation Redactions]().

## Page removal

Verwijder volledige pagina’s uit PDF‑documenten, dia’s uit presentaties en werkbladen uit spreadsheets. Je geeft een startpagina en een aantal op, samen met de richting ten opzichte van het startpunt. Zie [Remove Page Redactions]().

## Rasterization to PDF

Sla het opgeschoonde document op als een PDF waarvan de pagina’s worden gerenderd als rasterafbeeldingen. Het resulterende bestand bevat geen doorzoekbare tekst en geen originele metadata, zodat de verwijderde inhoud niet kan worden hersteld. Rasterisatie is de juiste keuze wanneer je een document aan derden moet overhandigen of moet voldoen aan regelgeving die PDF vereist. Je kunt specifieke pagina’s selecteren en PDF/A‑conformiteit aanvragen via de geavanceerde rasterisatie‑opties. Zie [Save in Rasterized PDF]() en [Advanced Rasterization Options]().

## Redaction policies

Groeperen meerdere redactie‑acties in een herbruikbaar beleid en pas dezelfde reeks regels consequent toe op veel documenten — ideaal voor terugkerende taken zoals het schoonmaken van een standaardset velden vóór publicatie. Zie [Use Redaction Policies]().

## Loading and saving

Laad documenten vanaf een lokaal pad of vanuit een stream, inclusief met wachtwoord beveiligde bestanden, en rasteriseer een document eventueel vooraf voordat je het redigeert. Bij het opslaan kun je het oorspronkelijke formaat behouden voor verdere bewerking, het originele bestand overschrijven, rasteriseren naar PDF, of naar een stream schrijven. Zie [Loading Documents]() en [Saving Documents]().

## On-premise

GroupDocs.Redaction voor Python via .NET draait volledig op je eigen infrastructuur — je documenten verlaten nooit je omgeving. Het pakket is een zelfstandige wheel die alles bundelt wat nodig is, zodat geen Microsoft Office, OpenOffice, Adobe Acrobat of aparte runtime geïnstalleerd hoeft te worden. Zie [System Requirements]() voor de ondersteunde platforms en native afhankelijkheden.
