---
title: "GroupDocs.Redaction.Redactions"
second_title: "Riferimento API di GroupDocs.Redaction per .NET"
description: "Lo spazio dei nomi Redactions fornisce classi per diversi tipi di redazioni."
type: docs
weight: 80
url: /it/net/groupdocs.redaction.redactions/
---
Lo spazio dei nomi Redactions fornisce classi per diversi tipi di redazioni.

## Classi

| Classe | Descrizione |
| --- | --- |
| [AnnotationRedaction](./annotationredaction) | Rappresenta una redazione che sostituisce il testo delle annotazioni (commenti, ecc.) che corrisponde a una determinata espressione regolare. |
| [CellColumnRedaction](./cellcolumnredaction) | Rappresenta una redazione di testo che sostituisce il testo nei documenti di foglio di calcolo (CSV, Excel, ecc.). |
| [CellFilter](./cellfilter) | Fornisce un'opzione per limitare l'ambito di una [`CellColumnRedaction`](../groupdocs.redaction.redactions/cellcolumnredaction) a un foglio di lavoro e a una colonna. |
| [CustomRedactionContext](./customredactioncontext) | Fornisce il contesto per l'elaborazione di redazioni personalizzate. |
| [CustomRedactionResult](./customredactionresult) | Rappresenta il risultato di un'operazione di redazione personalizzata. |
| [DeleteAnnotationRedaction](./deleteannotationredaction) | Rappresenta una redazione di testo che elimina le annotazioni se il testo corrisponde a una determinata espressione regolare (opzionalmente elimina tutte le annotazioni). |
| [EraseMetadataRedaction](./erasemetadataredaction) | Rappresenta una redazione dei metadati che cancella tutti i metadati o i metadati corrispondenti a specifici MetadataFilters dal documento. |
| [ExactPhraseRedaction](./exactphraseredaction) | Rappresenta una redazione del testo che sostituisce la frase esatta nel testo del documento, senza distinzione tra maiuscole e minuscole per impostazione predefinita. |
| [ImageAreaRedaction](./imagearearedaction) | Rappresenta una redazione che inserisce un rettangolo colorato nell'area specificata di un documento immagine. |
| [MetadataRedaction](./metadataredaction) | Rappresenta una classe astratta di base per le redazioni dei metadati del documento. |
| [MetadataSearchRedaction](./metadatasearchredaction) | Rappresenta una redazione dei metadati che ricerca e cancella i metadati usando espressioni regolari, corrispondendo chiavi e/o valori. |
| [PageAreaFilter](./pageareafilter) | Rappresenta un filtro di redazione, impostando un'area all'interno di una pagina di un documento per applicare la redazione. |
| [PageAreaRedaction](./pagearearedaction) | Rappresenta una redazione testuale complessa che influisce su testo, immagini e annotazioni in un'area della pagina. |
| [PageRangeFilter](./pagerangefilter) | Rappresenta un filtro di redazione, impostando l'intervallo di pagine all'interno di un documento per applicare la redazione. |
| [RedactionDescription](./redactiondescription) | Rappresenta le informazioni di una singola azione di modifica eseguita durante il processo di redazione. |
| [RedactionFilter](./redactionfilter) | Rappresenta un filtro di redazione, impostando l'ambito all'interno di un documento per applicare le redazioni. |
| [RegexRedaction](./regexredaction) | Rappresenta una redazione del testo che ricerca e sostituisce il testo nel documento corrispondendo all'espressione regolare fornita. |
| [RegionReplacementOptions](./regionreplacementoptions) | Rappresenta i parametri di colore e area per la sostituzione di una regione immagine. Vedi [`ImageAreaRedaction`](../groupdocs.redaction.redactions/imagearearedaction). |
| [RemovePageRedaction](./removepageredaction) | Rappresenta una redazione che rimuove una pagina (diapositiva, foglio di lavoro, ecc.) da un documento. |
| [ReplacementOptions](./replacementoptions) | Rappresenta le opzioni per la sostituzione del testo corrispondente. |
| [TextRedaction](./textredaction) | Rappresenta una classe astratta di base per le redazioni del testo del documento. |
| [TextReplacement](./textreplacement) | Rappresenta le informazioni di una sostituzione testuale. |
## Interfacce

| Interfaccia | Descrizione |
| --- | --- |
| [ICustomRedactionHandler](./icustomredactionhandler) | Fornisce un'interfaccia per implementare una logica di redazione personalizzata. |
| [IRedactionCallback](./iredactioncallback) | Definisce i metodi richiesti per ricevere informazioni su ogni modifica di redazione e, facoltativamente, impedirla. |
## Enumerazione

| Enumerazione | Descrizione |
| --- | --- |
| [MetadataFilters](./metadatafilters) | Rappresenta un elenco dei tipi più comuni di metadati del documento. |
| [PageSeekOrigin](./pageseekorigin) | Fornisce i campi che rappresentano i punti di riferimento in un documento per la ricerca. |
| [RedactionActionType](./redactionactiontype) | Rappresenta le azioni che possono essere eseguite per effettuare la redazione. |
| [RedactionType](./redactiontype) | Rappresenta un tipo di dati del documento, interessato dalla redazione. |
| [ReplacementType](./replacementtype) | Rappresenta un tipo di sostituzione per il testo corrispondente. |

<!-- NON MODIFICARE: generato da xmldocmd per GroupDocs.Redaction.dll -->
