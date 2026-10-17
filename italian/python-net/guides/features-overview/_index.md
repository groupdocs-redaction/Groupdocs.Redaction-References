---
title: "Panoramica delle funzionalità"
linkTitle: "Features overview"
second_title: "Riferimenti API di GroupDocs.Redaction per Python tramite .NET"
description: "GroupDocs.Redaction per Python via .NET rimuove le informazioni sensibili dai documenti tramite un'unica API indipendente dal formato — testo, metadati, aree immagine, annotazioni e pagine intere — e salva il risultato nel formato originale o come PDF sanificato."
type: docs
url: /it/python-net/guides/features-overview/
is_root: false
weight: 30
---


GroupDocs.Redaction per Python via .NET rimuove o oscura permanentemente le informazioni sensibili su un'ampia gamma di [supported document formats](). Ogni redazione segue lo stesso flusso di lavoro: apri un documento con [`Redactor`](/redaction/python-net/groupdocs.redaction/redactor/), applica una o più redazioni con `apply()`, quindi `save()` il risultato pulito sia nel suo formato originale sia come PDF sanificato. Le funzionalità di seguito possono essere combinate liberamente in un unico passaggio.

## Text redaction

Trova e sostituisci il testo con una frase esatta o con un'espressione regolare, coprendo sia parole intere sia schemi complessi come indirizzi e‑mail, numeri di telefono o codici fiscali nazionali. Il testo corrispondente può essere sostituito con testo di riserva o coperto da una casella colorata in modo che il contenuto originale non possa essere recuperato. Nei fogli di calcolo è possibile limitare la ricerca a un singolo foglio di lavoro o a una colonna. Vedi [Text Redactions]().

## Metadata redaction

Cancella o riscrivi i metadati del documento — autore, titolo, azienda, commenti e dati EXIF nelle immagini — in modo che nessun dettaglio sensibile trapeli attraverso le proprietà del documento. Puoi cancellare tutti i metadati, selezionare campi specifici o sostituire i valori con nuovi. Vedi [Metadata Redactions]().

## Image-area redaction

Oscura una regione rettangolare di un'immagine incorporata o di una pagina scansionata disegnando una casella piena sull'area specificata — utile per nascondere firme, foto, intestazioni o piè di pagina dove si prevede la presenza di dati riservati. Vedi [Image Redactions]().

## Annotation redaction

Riscrivi o elimina annotazioni, commenti e note. Puoi rimuovere ogni annotazione o usare un'espressione regolare per corrispondere solo a quelle che contengono testo sensibile. Vedi [Annotation Redactions]().

## Page removal

Rimuovi pagine intere da documenti PDF, diapositive da presentazioni e fogli di lavoro da fogli di calcolo. Specifica una pagina iniziale e un numero di pagine, insieme alla direzione rispetto al punto di partenza. Vedi [Remove Page Redactions]().

## Rasterization to PDF

Salva il documento pulito come PDF le cui pagine sono renderizzate come immagini raster. Il file risultante non contiene testo ricercabile né i metadati originali, quindi il contenuto rimosso non può essere recuperato. La rasterizzazione è la scelta giusta quando devi consegnare un documento a terze parti o rispettare normative che richiedono il PDF. Puoi selezionare pagine specifiche e richiedere la conformità PDF/A tramite le opzioni avanzate di rasterizzazione. Vedi [Save in Rasterized PDF]() e [Advanced Rasterization Options]().

## Redaction policies

Raggruppa diverse redazioni in una politica riutilizzabile e applica lo stesso insieme di regole in modo coerente su molti documenti — ideale per attività ricorrenti come la pulizia di un insieme standard di campi prima della pubblicazione. Vedi [Use Redaction Policies]().

## Loading and saving

Carica documenti da un percorso locale o da uno stream, inclusi file protetti da password, e opzionalmente pre‑rasterizza un documento prima della redazione. Durante il salvataggio, mantieni il formato originale per ulteriori modifiche, sovrascrivi il file originale, rasterizza in PDF o scrivi su uno stream. Vedi [Loading Documents]() e [Saving Documents]().

## On-premise

GroupDocs.Redaction per Python via .NET funziona interamente sulla tua infrastruttura — i tuoi documenti non lasciano mai l'ambiente. Il pacchetto è una wheel autonoma che include tutto il necessario, quindi non è necessario installare Microsoft Office, OpenOffice, Adobe Acrobat o runtime separati. Vedi [System Requirements]() per le piattaforme supportate e le dipendenze native.
