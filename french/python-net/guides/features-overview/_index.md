---
title: "Aperçu des fonctionnalités"
linkTitle: "Features overview"
second_title: "Références API de GroupDocs.Redaction pour Python via .NET"
description: "GroupDocs.Redaction pour Python via .NET supprime les informations sensibles des documents grâce à une API unique, indépendante du format — texte, métadonnées, zones d'image, annotations et pages entières — et enregistre le résultat dans le format d'origine ou sous forme de PDF assaini."
type: docs
url: /fr/python-net/guides/features-overview/
is_root: false
weight: 30
---


GroupDocs.Redaction pour Python via .NET supprime ou masque définitivement les informations sensibles sur un large éventail de [supported document formats](). Chaque masquage suit le même flux de travail : ouvrez un document avec [`Redactor`](/redaction/python-net/groupdocs.redaction/redactor/), appliquez un ou plusieurs masquages avec `apply()`, puis `save()` le résultat nettoyé soit dans son format d'origine, soit sous forme de PDF assaini. Les capacités ci-dessous peuvent être combinées librement en une seule passe.

## Text redaction

Rechercher et remplacer du texte par une phrase exacte ou par une expression régulière, en couvrant à la fois les mots entiers et les modèles complexes tels que les adresses e‑mail, les numéros de téléphone ou les numéros d'identité nationale. Le texte correspondant peut être remplacé par du texte de substitution ou couvert par une boîte colorée afin que le contenu original ne puisse pas être récupéré. Dans les feuilles de calcul, vous pouvez restreindre la recherche à une seule feuille ou colonne. Voir [Text Redactions]().

## Metadata redaction

Effacer ou réécrire les métadonnées du document — auteur, titre, société, commentaires et données EXIF sur les images — afin qu'aucun détail sensible ne fuite via les propriétés du document. Vous pouvez supprimer toutes les métadonnées, cibler des champs spécifiques ou remplacer les valeurs par de nouvelles. Voir [Metadata Redactions]().

## Image-area redaction

Noircir une zone rectangulaire d'une image intégrée ou d'une page numérisée en dessinant une boîte remplie sur la zone donnée — utile pour masquer les signatures, photos, en‑têtes ou pieds de page où des données confidentielles sont susceptibles d'apparaître. Voir [Image Redactions]().

## Annotation redaction

Réécrire ou supprimer les annotations, commentaires et notes. Vous pouvez enlever chaque annotation ou utiliser une expression régulière pour ne correspondre qu'aux celles qui contiennent du texte sensible. Voir [Annotation Redactions]().

## Page removal

Supprimer des pages entières des documents PDF, des diapositives des présentations et des feuilles de calcul des classeurs. Vous indiquez une page de départ et un nombre, ainsi que la direction par rapport au point de départ. Voir [Remove Page Redactions]().

## Rasterization to PDF

Enregistrez le document nettoyé au format PDF dont les pages sont rendues en images raster. Le fichier résultant ne contient aucun texte recherchable ni aucune des métadonnées d'origine, de sorte que le contenu supprimé ne puisse pas être récupéré. La rasterisation est le bon choix lorsque vous devez remettre un document à des tiers ou vous conformer à des réglementations qui exigent le PDF. Vous pouvez sélectionner des pages spécifiques et demander la conformité PDF/A via les options avancées de rasterisation. Voir [Save in Rasterized PDF]() et [Advanced Rasterization Options]().

## Redaction policies

Regroupez plusieurs censures dans une politique réutilisable et appliquez le même ensemble de règles de manière cohérente sur de nombreux documents — idéal pour les tâches récurrentes telles que le nettoyage d'un ensemble standard de champs avant la publication. Voir [Use Redaction Policies]().

## Loading and saving

Chargez des documents depuis un chemin local ou depuis un flux, y compris les fichiers protégés par mot de passe, et éventuellement pré‑rasterisez un document avant la censure. Lors de l'enregistrement, conservez le format d'origine pour une édition ultérieure, écrasez le fichier original, rasterisez en PDF ou écrivez dans un flux. Voir [Loading Documents]() et [Saving Documents]().

## On-premise

GroupDocs.Redaction for Python via .NET s'exécute entièrement sur votre propre infrastructure — vos documents ne quittent jamais votre environnement. Le package est une roue autonome qui regroupe tout ce dont il a besoin, de sorte qu'aucun Microsoft Office, OpenOffice, Adobe Acrobat ou runtime séparé n'ait besoin d'être installé. Voir [System Requirements]() pour les plateformes prises en charge et les dépendances natives.
