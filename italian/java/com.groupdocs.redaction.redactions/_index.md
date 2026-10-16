---
title: "com.groupdocs.redaction.redactions"
second_title: "GroupDocs.Redaction per Java Riferimento API"
description: "Il pacchetto fornisce classi per diversi tipi di redazioni."
type: docs
weight: 16
url: /it/java/com.groupdocs.redaction.redactions/
---

Il pacchetto fornisce classi per diversi tipi di redazioni.



## Classi

| Classe | Descrizione |
| --- | --- |
| [AnnotationRedaction](../com.groupdocs.redaction.redactions/annotationredaction) | Rappresenta una redazione che sostituisce il testo delle annotazioni (commenti, ecc.) corrispondente a una data espressione regolare. |
| [CellColumnRedaction](../com.groupdocs.redaction.redactions/cellcolumnredaction) | Rappresenta una redazione di testo che sostituisce il testo in documenti di foglio di calcolo (CSV, Excel, ecc.). |
| [CellFilter](../com.groupdocs.redaction.redactions/cellfilter) | Fornisce un'opzione per limitare l'ambito di una CellColumnRedaction a un foglio di lavoro e a una colonna. |
| [CustomRedactionContext](../com.groupdocs.redaction.redactions/customredactioncontext) | Fornisce dati di input per [ICustomRedactionHandler](../com.groupdocs.redaction.redactions/icustomredactionhandler). |
| [CustomRedactionResult](../com.groupdocs.redaction.redactions/customredactionresult) | Rappresenta un risultato restituito da [ICustomRedactionHandler](../com.groupdocs.redaction.redactions/icustomredactionhandler). |
| [DeleteAnnotationRedaction](../com.groupdocs.redaction.redactions/deleteannotationredaction) | Rappresenta una redazione di testo che elimina le annotazioni se il testo corrisponde a una data espressione regolare (opzionalmente elimina tutte le annotazioni). |
| [EraseMetadataRedaction](../com.groupdocs.redaction.redactions/erasemetadataredaction) | Rappresenta una redazione dei metadati che cancella tutti i metadati o i metadati corrispondenti a specifici MetadataFilters dal documento. |
| [ExactPhraseRedaction](../com.groupdocs.redaction.redactions/exactphraseredaction) | Rappresenta una redazione di testo che sostituisce una frase esatta nel testo del documento, senza distinzione tra maiuscole e minuscole per impostazione predefinita. |
| [ImageAreaRedaction](../com.groupdocs.redaction.redactions/imagearearedaction) | Rappresenta una redazione che inserisce un rettangolo colorato nell'area specificata di un documento immagine. |
| [MetadataFilters](../com.groupdocs.redaction.redactions/metadatafilters) | Rappresenta un elenco dei tipi di metadati di documento più comuni. |
| [MetadataRedaction](../com.groupdocs.redaction.redactions/metadataredaction) | Rappresenta una classe astratta di base per le redazioni dei metadati del documento. |
| [MetadataSearchRedaction](../com.groupdocs.redaction.redactions/metadatasearchredaction) | Rappresenta una redazione dei metadati che ricerca e rimuove i metadati usando espressioni regolari, corrispondendo chiavi e/o valori. |
| [PageAreaFilter](../com.groupdocs.redaction.redactions/pageareafilter) | Rappresenta un filtro di redazione, impostando un'area all'interno di una pagina di un documento per applicare la redazione. |
| [PageAreaRedaction](../com.groupdocs.redaction.redactions/pagearearedaction) | Rappresenta una redazione testuale complessa che influisce su testo, immagini e annotazioni in un'area della pagina. |
| [PageRangeFilter](../com.groupdocs.redaction.redactions/pagerangefilter) | Rappresenta un filtro di redazione, impostando l'intervallo di pagine all'interno di un documento per applicare la redazione. |
| [RedactionDescription](../com.groupdocs.redaction.redactions/redactiondescription) | Rappresenta le informazioni di una singola azione di modifica eseguita durante il processo di redazione. |
| [RedactionFilter](../com.groupdocs.redaction.redactions/redactionfilter) | Rappresenta un filtro di redazione, impostando l'ambito all'interno di un documento per applicare le redazioni. |
| [RedactionType](../com.groupdocs.redaction.redactions/redactiontype) | Rappresenta un tipo di dati del documento, influenzato dalla redazione. |
| [RegexRedaction](../com.groupdocs.redaction.redactions/regexredaction) | Rappresenta una redazione di testo che ricerca e sostituisce il testo nel documento corrispondendo all'espressione regolare fornita. |
| [RegionReplacementOptions](../com.groupdocs.redaction.redactions/regionreplacementoptions) | Rappresenta i parametri di colore e area per la sostituzione di una regione immagine. |
| [RemovePageRedaction](../com.groupdocs.redaction.redactions/removepageredaction) | Rappresenta una redazione che rimuove una pagina (diapositiva, foglio di lavoro, ecc.) da un documento. |
| [ReplacementOptions](../com.groupdocs.redaction.redactions/replacementoptions) | Rappresenta le opzioni per la sostituzione del testo corrispondente. |
| [TextRedaction](../com.groupdocs.redaction.redactions/textredaction) | Rappresenta una classe astratta di base per le redazioni testuali del documento. |
| [TextReplacement](../com.groupdocs.redaction.redactions/textreplacement) | Rappresenta le informazioni di una sostituzione testuale. |

## Interfacce

| Interfaccia | Descrizione |
| --- | --- |
| [ICustomRedactionHandler](../com.groupdocs.redaction.redactions/icustomredactionhandler) | Definisce un callback di redazione personalizzato. |
| [IRedactionCallback](../com.groupdocs.redaction.redactions/iredactioncallback) | Definisce i metodi necessari per ricevere informazioni su ogni modifica di redazione e, facoltativamente, impedirla. |

## Enumerazioni

| Enum | Descrizione |
| --- | --- |
| [PageSeekOrigin](../com.groupdocs.redaction.redactions/pageseekorigin) | Fornisce i campi che rappresentano i punti di riferimento in un documento per la ricerca. |
| [RedactionActionType](../com.groupdocs.redaction.redactions/redactionactiontype) | Rappresenta le azioni che possono essere eseguite per effettuare la redazione. |
| [ReplacementType](../com.groupdocs.redaction.redactions/replacementtype) | Rappresenta un tipo di sostituzione per il testo corrispondente. |
