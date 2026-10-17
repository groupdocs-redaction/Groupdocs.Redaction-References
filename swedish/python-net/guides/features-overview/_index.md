---
title: "Översikt över funktioner"
linkTitle: "Features overview"
second_title: "GroupDocs.Redaction för Python via .NET API-referenser"
description: "GroupDocs.Redaction för Python via .NET tar bort känslig information från dokument genom ett enda formatoberoende API — text, metadata, bildområden, annotationer och hela sidor — och sparar resultatet i originalformatet eller som en sanerad PDF."
type: docs
url: /sv/python-net/guides/features-overview/
is_root: false
weight: 30
---


GroupDocs.Redaction för Python via .NET tar bort eller permanent döljer känslig information över ett brett spektrum av [supported document formats](). Varje redigering följer samma arbetsflöde: öppna ett dokument med [`Redactor`](/redaction/python-net/groupdocs.redaction/redactor/), tillämpa en eller flera redigeringar med `apply()`, sedan `save()` det rengjorda resultatet antingen i dess originalformat eller som en sanerad PDF. Följande funktioner kan kombineras fritt i ett enda pass.

## Text redaction

Sök och ersätt text med en exakt fras eller med ett reguljärt uttryck, vilket täcker både hela ord och komplexa mönster såsom e‑postadresser, telefonnummer eller nationella ID‑nummer. Matchad text kan ersättas med ersättningstext eller täckas av en färgad ruta så att det ursprungliga innehållet inte kan återställas. I kalkylblad kan du begränsa sökningen till ett enda arbetsblad eller en kolumn. Se [Text Redactions]().

## Metadata redaction

Radera eller skriv om dokumentmetadata — författare, titel, företag, kommentarer och EXIF-data på bilder — så att inga känsliga detaljer läcker genom dokumentegenskaper. Du kan rensa all metadata, rikta in dig på specifika fält eller ersätta värden med nya. Se [Metadata Redactions]().

## Image-area redaction

Svärta ett rektangulärt område i en inbäddad bild eller en skannad sida genom att rita en fylld ruta över ett givet område — användbart för att dölja signaturer, foton, sidhuvuden eller sidfötter där konfidentiell data kan förekomma. Se [Image Redactions]().

## Annotation redaction

Skriv om eller ta bort annotationer, kommentarer och anteckningar. Du kan ta bort varje annotation eller använda ett reguljärt uttryck för att endast matcha de som innehåller känslig text. Se [Annotation Redactions]().

## Page removal

Ta bort hela sidor från PDF-dokument, bilder från presentationer och arbetsblad från kalkylblad. Du anger en startssida och ett antal, tillsammans med riktningen relativt startpunkten. Se [Remove Page Redactions]().

## Rasterization to PDF

Spara det rengjorda dokumentet som en PDF vars sidor renderas som rasterbilder. Den resulterande filen innehåller ingen sökbar text och ingen av den ursprungliga metadata, så det borttagna innehållet kan inte återställas. Rasterisering är rätt val när du måste överlämna ett dokument till tredje part eller följa regler som kräver PDF. Du kan välja specifika sidor och begära PDF/A‑kompatibilitet via de avancerade rasteriseringsalternativen. Se [Save in Rasterized PDF]() och [Advanced Rasterization Options]().

## Redaction policies

Gruppera flera raderingar i en återanvändbar policy och tillämpa samma uppsättning regler konsekvent över många dokument — idealiskt för återkommande uppgifter som att rensa ett standardset av fält innan publicering. Se [Använd redigeringspolicyer]().

## Loading and saving

Läs in dokument från en lokal sökväg eller från en ström, inklusive lösenordsskyddade filer, och valfritt för‑rastera ett dokument innan radering. Vid sparande, behåll originalformatet för vidare redigering, skriv över den ursprungliga filen, rastera till PDF eller skriv till en ström. Se [Ladda dokument]() och [Spara dokument]().

## On-premise

GroupDocs.Redaction för Python via .NET körs helt på din egen infrastruktur — dina dokument lämnar aldrig din miljö. Paketet är ett självständigt wheel som samlar allt som behövs, så ingen Microsoft Office, OpenOffice, Adobe Acrobat eller separat runtime behöver installeras. Se [Systemkrav]() för de stödda plattformarna och inhemska beroenden.
