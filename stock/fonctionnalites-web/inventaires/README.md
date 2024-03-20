---
description: >-
  Page de récapitulatif des inventaires à réaliser, le traitement se fait sur le
  l'application mobile.
---

# Inventaires

Cette page est disponible dans le menu **Stock**, puis **Inventaire**. Cette page contient plusieurs éléments :&#x20;

* Une **barre de filtre**, permettant de filtrer les données qui sont affichées dans le tableau
* Une **recherche rapide**, permettant également de filtrer les données affichées dans le tableau
* Un bouton <mark style="background-color:blue;">**Ajouter une mission**</mark> pour créer un nouvel inventaire
* Un bouton <mark style="background-color:blue;">**Voir les saisies**</mark>, sous le bouton Ajouter une mission, qui ouvre une nouvelle page pour avoir le récapitulatif de toutes les quantités relevées.
* Un bouton <mark style="background-color:blue;">**Gérer les anomalies**</mark>, sous le bouton Ajouter une mission, qui ouvre une nouvelle page récapitulant les anomalies de quantité détectées sur les inventaires.
* Un **tableau**, regroupant les différents inventaires

{% embed url="https://www.screencast.com/t/C5J9C3mr" %}
Page inventaire
{% endembed %}

## Contenu des filtres

<table><thead><tr><th width="234.5">Filtre</th><th>Description</th></tr></thead><tbody><tr><td><strong>Du</strong></td><td>La tranche basse filtrant sur la date de début d'inventaire</td></tr><tr><td><strong>Au</strong></td><td>La tranche haute filtrant sur la date de fin d'inventaire</td></tr><tr><td><strong>Types</strong></td><td>Type d'invantaire (Art/Ref ou Emplacement)</td></tr></tbody></table>

## Contenu du tableau

<table><thead><tr><th width="252">Colonne</th><th>Description</th></tr></thead><tbody><tr><td><strong>Libellé</strong></td><td>Nom de l'inventaire</td></tr><tr><td><strong>Date de début</strong></td><td>Date de début de traitement de l'inventaire</td></tr><tr><td><strong>Date de fin</strong></td><td>Date de fin de traitement de l'inventaire</td></tr><tr><td><strong>Taux d'avancement</strong></td><td>Pourcentage d'avancement de l'inventaire, quand un opérateur saisit une quantité le % augmente</td></tr><tr><td><strong>Type</strong></td><td><p>Types d'inventaire : </p><ul><li>Art/Ref : création de la mission avec choix des code barres article/référence ou avec un emplacement</li><li>Emplacement : <em>Uniquement avec l'utilisation des étiquettes RFID.</em> Création de la mission avec choix des emplacements </li></ul></td></tr><tr><td><strong>Demandeur</strong></td><td>Personne ayant créé la demande</td></tr></tbody></table>

## Créer une mission d'inventaire

Cliquer sur le bouton <mark style="background-color:blue;">**Ajouter une mission**</mark> la modale de création s'ouvre, vous devez renseigner plusieurs champs :&#x20;

* **Libellé** : Nom de l'inventaire qui s'affichera sur le terminal mobile
* **Date prévue de début\*** : Date de début de traitement de l'inventaire, à partir de cette date l'inventaire apparaitra sur le terminal mobile
* **Date prévue de fin\*** : Date de fin de traitement de l'inventaire, arrivé à cette date l'inventaire disparaîtra du le terminal mobile
* **Description\*** : Description de l'inventaire
* **Type de mission\*** :&#x20;
  * Mission quantité article (Art/Ref) : création de la mission avec choix des code barres article/référence ou choix d'inventorier toute les références/articles d'un ou des emplacements
  * Article sur emplacement (Emplacement) : _Uniquement avec l'utilisation des étiquettes RFID._ Création de la mission avec choix des emplacements&#x20;
* **Demandeur\*** : Créateur de la mission, par défaut c'est l'utilisateur connecté mais ce user peut être changé

## Art/Ref (Mission quantité article)

Sur le détail de la mission vous retrouvez plusieurs éléments :&#x20;

* Un **filtre** anomalies : pour retrouver les références/articles qui ont une erreur de quantité en  stock
* un bouton <mark style="background-color:blue;">**Ajouter des emplacements**</mark> : pour ajouter les articles ou références présents sur cet ou ces emplacements
* un bouton <mark style="background-color:blue;">**Ajouter des références ou des articles**</mark> : pour ajouter les articles ou références via leur codebarre
* Un bouton <mark style="background-color:blue;">**Exporter au format CSV**</mark>, sous le bouton Ajouter des références ou des articles, destiné à exporter l'ensemble des données au format CSV
* Un **tableau Liste des articles** : qui récapitule l'ensemble des articles à inventorier
* Un **tableau Liste des références** : qui récapitule l'ensemble des références à inventorier

#### Contenu des tableaux (Articles et Référence)

<table><thead><tr><th width="225">Colonne</th><th>Description</th></tr></thead><tbody><tr><td><strong>Référence</strong></td><td>Code de référence</td></tr><tr><td><strong>Code barre</strong></td><td>Code barre référence ou article</td></tr><tr><td><strong>Libellé</strong></td><td>Libellé de la référence</td></tr><tr><td><strong>Emplacement</strong></td><td>Emplacement de l'article ou de la référence</td></tr><tr><td><strong>Date de saisie</strong></td><td>Date de l'inventaire de la référence/ de l'article</td></tr><tr><td><strong>Anomalie</strong></td><td><p>Oui ou Non</p><p>Si un écart est constaté par un opérateur sur une référence ou article, il sera indiqué oui sur la ligne de référence/article</p></td></tr><tr><td><strong>Quantité en stock</strong></td><td>Quantité de la référence ou de l'article </td></tr><tr><td><strong>Quantité comptée</strong></td><td>Quantité compté par l'opérateur qui à fait l'inventaire</td></tr><tr><td><strong>Unité logistique</strong></td><td><p><em>Que disponible pour les articles.</em> </p><p>Si l'article est dans une UL, elle sera indiqué dans cette colonne</p></td></tr></tbody></table>

{% hint style="info" %}
Vous ne pouvez pas ajouter dans un nouvel inventaire des références ou articles qui sont déjà dans un inventaire en cours.
{% endhint %}

#### Ajouter des emplacements

Pour ajouter toutes les références ou des articles d'un emplacement, cliquer sur le bouton <mark style="background-color:blue;">**Ajouter des emplacements**</mark> une modale s'ouvre avec un champ emplacement, sélectionner un ou plusieurs emplacements. À la validation, les références et les articles s'ajoutent respectivement dans la liste des références ou liste des articles.

{% embed url="https://www.screencast.com/t/gtxOwCTR" %}
Ajout emplacement
{% endembed %}

#### Ajouter des références ou articles

Vous pouvez ajouter des références ou des articles via leurs code barres. Cliquer sur <mark style="background-color:blue;">**Ajouter des références ou des articles**</mark> une modale s'ouvre avec un champ "Codes barre articles/références". Pour ajouter plusieurs code barres, à la suite utiliser la virgule pour séparer les code barres (ex : REF230500000014, ART230500000090). Puis cliquer sur <mark style="background-color:blue;">**Enregistrer**</mark>, les références et les articles s'ajoutent respectivement dans la liste des références ou liste des articles.

### Traitement inventaire

Le traitement d'un inventaire ne peut se faire que sur le nomade. Voir [Stock > fonctionnalités mobile > inventaire](../../fonctionnalites-mobile/stock-i-inventaire.md).

Vous pouvez voir de manière plus général l'avancement de vos inventaires sur la page de liste grace à la jauge du taux d'avancement qui grandit au fur et à mesur.

Au fur et à mesure que l'opérateur avance sur l'inventaire la Date de saisie, la Quantité comptée et le champ Anomalie se remplissent.

{% embed url="https://www.screencast.com/t/CRGgU9wt" %}

#### Sur le détails d'un article et d'une référence

La date de dernier inventaire se met à jour avec la date de saisie.

### Gestion des anomalies

Lorsqu'une anomalie est détectée, il sera demandé à l'opérateur de recompter l'article ou la référence en question.&#x20;

* Si la quantité est bien différente de la quantité en stock, l'anomalie est confirmée et la quantité en stock se met à jour.
* Si la quantité est la même que celle en stock, l'anomalie disparait

Cette opération peut aussi se faire sur le web sur la page [**Gérer les anomalies**](anomalies.md)**.**

#### Mouvements de stock

Vous allez avoir des mouvements de stock de **sortie inventaire** (si la quantité comptée est inférieure à la quantité en stock) ou des mouvements d'**entrée inventaire** (si la quantité comptée est supérieure à la quantité en stock)

{% embed url="https://www.screencast.com/t/OTQicqWL0" %}
Mouvements de stock issu de l'inventaire
{% endembed %}

## Emplacement (Article sur emplacement)

{% hint style="warning" %}
Uniquement avec l'utilisation d'étiquette RFID
{% endhint %}

_À venir_
