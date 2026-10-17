---
title: "Redactions de métadonnées"
linkTitle: "Metadata redactions"
second_title: "Références API de GroupDocs.Redaction pour Python via .NET"
description: "Cet article montre comment l’API de redaction Python vous permet de remplacer ou de supprimer des métadonnées à l’aide de filtres ou de recherches par expression régulière."
type: docs
url: /fr/python-net/guides/metadata-redactions/
is_root: false
weight: 70
---


Avec l’API GroupDocs.Redaction, vous pouvez appliquer des redactions de métadonnées aux documents de différents formats tels que PDF, DOC, DOCX, PPT, PPTX, XLS, XLSX et autres. Voir la liste complète dans l’article [supported document formats]().

GroupDocs.Redactions fournit une API flexible qui permet de remplacer ou de supprimer des métadonnées à l’aide de filtres ou de recherches par expression régulière.

## Filter metadata

Fonctionnalité de base pour toutes les redactions, dérivée de la classe de base [MetadataRedaction](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction.redactions/metadataredaction/) qui est le *filtrage des métadonnées* et qui est obligatoire pour les redactions de métadonnées. Elle utilise l’énumération à drapeaux [MetadataFilters](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction.redactions/metadatafilters/), contenant des éléments pour les entrées de métadonnées les plus fréquentes. Vous pouvez définir le filtre sur *All*, ou toute combinaison de métadonnées. Par exemple, l’exemple ci‑dessous définit le filtre sur *Author*, *Manager* et *NameOfApplication* – pour la redaction textuelle ou leur nettoyage :

```python
# redaction dérivée de MetadataRedaction
redaction.filter = MetadataFilters.AUTHOR | MetadataFilters.MANAGER | MetadataFilters.NAME_OF_APPLICATION
```

Ci‑dessous le tableau avec la liste complète des éléments de [MetadataFilters](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction.redactions/metadatafilters/):

| Filtre | Valeur numérique | Description |
| --- | --- | --- |
| *None* | 0 | Paramètre de filtre vide, ne correspond à aucun élément de métadonnées |
| *Author* | 1 | Auteur du document |
| *Catégorie* | 2 | Catégorie du document |
| *Commentaires* | 4 | Commentaire du document |
| *Entreprise* | 8 | Entreprise de l'auteur |
| *StatutContenu* | 16 | Statut du contenu |
| *HeureCréation* | 32 | Heure de création |
| *BaseLienHypertexte* | 64 | Base du lien hypertexte |
| *DernièreImpression* | 128 | Date et heure de la dernière impression |
| *DernierEnregistréPar* | 256 | Dernière sauvegarde par l'utilisateur |
| *LastSavedTime* | 1024 | Date et heure du dernier enregistrement |
| *NameOfApplication* | 2048 | Nom de l'application où le document a été créé |
| *Manager* | 4096 | Nom du responsable de l'auteur |
| *RevisionNumber* | 8192 | Numéro de révision |
| *Subject* | 16384 | Sujet du document |
| *Template* | 32768 | Nom du modèle de document |
| *Title* | 65536 | Titre du document |
| *TotalEditingTime* | 131072 | Temps total d'édition |
| *Version* | 262144 | Version du document |
| *Description* | 524288 | Description du document |
| *Mots-clés* | 1048576 | Mots-clés du document |
| *ContentType* | 2097152 | Type de contenu |
| *Tous* | 2147483647 | Tous les types d'éléments de métadonnées |

## Clean metadata

Vous pouvez remplacer toutes les métadonnées ou des métadonnées spécifiques dans le document par des valeurs vides (blanches ou minimales) en utilisant la classe [EraseMetadataRedaction](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction.redactions/erasemetadataredaction/). L'exemple ci‑dessous supprime toutes les propriétés du document :

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.options import SaveOptions
from groupdocs.redaction.redactions import EraseMetadataRedaction, MetadataFilters

def clean_all_metadata():
    # Spécifiez les options de rédaction pour effacer toutes les métadonnées
    met_red = EraseMetadataRedaction(MetadataFilters.ALL)

    # Chargez le document à censurer
    with Redactor("./sample.docx") as redactor:
        # Appliquer le masquage
        result = redactor.apply(met_red)

        # Enregistrez le document masqué à côté du fichier source
        so = SaveOptions()
        so.add_suffix = True
        so.rasterize_to_pdf = False
        so.redacted_file_suffix = "redacted"
        redactor.save(so)

if __name__ == "__main__":
    clean_all_metadata()
```

`sample.docx` est le fichier d'exemple utilisé dans cet exemple. Cliquez [ici](https://docs.groupdocs.com/redaction/python-net/_sample_files/developer-guide/basic-usage/metadata-redactions/sample.docx) pour le télécharger.

  
```text
Binary file (DOCX, 16 KB)
```
[Download full output](https://docs.groupdocs.com/redaction/python-net/_output_files/developer-guide/basic-usage/metadata-redactions/clean_all_metadata/sample_redacted.docx)

Vous pouvez spécifier [MetadataFilter.All](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction.redactions/metadatafilters/) ou utiliser le constructeur par défaut pour supprimer toutes les métadonnées du document donné, Custom – pour effacer toutes les entrées de métadonnées personnalisées.

## Redact metadata

Vous pouvez utiliser [MetadataSearchRedaction](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction.redactions/metadatasearchredaction/) pour supprimer les données sensibles des métadonnées du document en utilisant des expressions régulières. Par exemple, nous pouvons supprimer toute mention de "Company Ltd." :

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.options import SaveOptions
from groupdocs.redaction.redactions import MetadataSearchRedaction

def redact_metadata():
    # Spécifiez les options de rédaction : motif de recherche et chaîne de remplacement
    met_red = MetadataSearchRedaction("Company Ltd.", "--company--")

    # Chargez le document à censurer
    with Redactor("./sample.docx") as redactor:
        # Appliquer le masquage
        result = redactor.apply(met_red)

        # Enregistrez le document masqué à côté du fichier source
        so = SaveOptions()
        so.add_suffix = True
        so.rasterize_to_pdf = False
        so.redacted_file_suffix = "redacted"
        redactor.save(so)

if __name__ == "__main__":
    redact_metadata()
```

`sample.docx` est le fichier d'exemple utilisé dans cet exemple. Cliquez [ici](https://docs.groupdocs.com/redaction/python-net/_sample_files/developer-guide/basic-usage/metadata-redactions/sample.docx) pour le télécharger.

  
```text
Binary file (DOCX, 16 KB)
```
[Download full output](https://docs.groupdocs.com/redaction/python-net/_output_files/developer-guide/basic-usage/metadata-redactions/redact_metadata/sample_redacted.docx)

Le premier argument est une expression régulière, le second est une chaîne de remplacement. Vous pouvez également définir la portée de la rédaction en définissant le filtre, par ex. à [MetadataFilter.Company](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction.redactions/metadatafilters/). – cela laissera les correspondances des expressions régulières non modifiées dans tous les éléments de métadonnées, sauf la propriété "Company" :

```python
from groupdocs.redaction import Redactor
from groupdocs.redaction.options import SaveOptions
from groupdocs.redaction.redactions import MetadataSearchRedaction, MetadataFilters

def redact_metadata_with_filter():
    # Spécifiez les options de rédaction : motif de recherche et chaîne de remplacement
    met_red = MetadataSearchRedaction("Company Ltd.", "--company--")

    # Limitez la portée de la rédaction à l'élément de métadonnées Company uniquement
    met_red.filter = MetadataFilters.COMPANY

    # Chargez le document à censurer
    with Redactor("./sample.docx") as redactor:
        # Appliquer le masquage
        result = redactor.apply(met_red)

        # Enregistrez le document masqué à côté du fichier source
        so = SaveOptions()
        so.add_suffix = True
        so.rasterize_to_pdf = False
        so.redacted_file_suffix = "redacted"
        redactor.save(so)

if __name__ == "__main__":
    redact_metadata_with_filter()
```

`sample.docx` est le fichier d'exemple utilisé dans cet exemple. Cliquez [ici](https://docs.groupdocs.com/redaction/python-net/_sample_files/developer-guide/basic-usage/metadata-redactions/sample.docx) pour le télécharger.

  
```text
Binary file (DOCX, 16 KB)
```
[Download full output](https://docs.groupdocs.com/redaction/python-net/_output_files/developer-guide/basic-usage/metadata-redactions/redact_metadata_with_filter/sample_redacted.docx)

## Metadata redaction status

Toutes les rédactions de métadonnées s'appliquent à chaque élément de métadonnées séparément, et même si la rédaction d'un élément échoue, le reste des éléments sera mis à jour. Vous pouvez trouver une liste des éléments de métadonnées échoués, ignorés (rejetés) et les raisons correspondantes dans la propriété [ErrorMessage](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction/redactionresult/error_message/) de [RedactorLogEntry.Result](https://reference.groupdocs.com/redaction/python-net/groupdocs.redaction/redactorlogentry/result/).
