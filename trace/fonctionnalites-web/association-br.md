---
description: >-
  L'objectif de l'association BR est de lier une ou plusieurs unités logistiques
  à des numéros de réceptions provenant d'un ERP.
---

# Association BR

L'association BR est une fonctionnalité permettant d'associer une ou plusieurs **unités logistiques** à un ou plusieurs **bon(s) de réception provenant d'un ERP**. Après la réalisation de l'association BR, les opérateurs pourrons effectuer des mouvements de traçabilité directement sur les numéros de réceptions de l'ERP.&#x20;

<figure><img src="../../.gitbook/assets/association BR.png" alt=""><figcaption><p>Schéma de l'association BR si paramétré tel quel</p></figcaption></figure>

La fonctionnalité Association BR est disponible dans l'onglet **Traçabilité**, puis **Association BR**. Cette page contient plusieurs éléments :&#x20;

* Une **barre de filtre**, permettant de filtrer les données qui sont affichées dans le tableau
* Une **recherche rapide**, permettant également de filtrer les données affichées dans le tableau
* Un bouton <mark style="background-color:blue;">**Association/BR**</mark>, destiné à la création d'une association BR
* Un bouton <mark style="background-color:blue;">**Exporter au format CSV**</mark>, destiné à exporter l'ensemble des données filtrées (suivant les dates renseignées) au format CSV
* Un **tableau**, regroupant les différentes associations BR créées

### Contenu des filtres

| Filtre               | Description                                                        |
| -------------------- | ------------------------------------------------------------------ |
| **Du**               | La tranche basse filtrant sur la date de création de l'association |
| **Au**               | La tranche haute filtrant sur la date de création de l'association |
| **Unité logistique** | Le(s) numéro(s) d'unité logistique à afficher                      |
| **Réceptions**       | Le(s) numéro(s) de réception à afficher                            |
| **Utilisateurs**     | Le(s) utilisateur(s) ayant créé l'association                      |

### Contenu du tableau

| Colonne              | Description                                                            |
| -------------------- | ---------------------------------------------------------------------- |
| **Date**             | La date de l'association                                               |
| **Unité logistique** | Les UL contenus dans l'association, séparés par des virgules           |
| **Réception**        | Les réceptions contenues dans l'association, séparées par des virgules |
| **Utilisateur**      | L'utilisateur ayant réalisé l'association                              |

### Créer une nouvelle association

Afin de créer une nouvelle association BR, il suffit cliquer sur le bouton <mark style="background-color:blue;">**Association/BR**</mark>. Une modale va alors s'ouvrir, permettant ainsi de renseigner plusieurs champs :&#x20;

* Le(s) **association(s) UL**, contenant les différentes unités logistiques à associer. Une UL correspond à une ligne (à ajouter avec le bouton +)
* Le(s) **numéro(s) de réception**, contenant les différentes réceptions à associer. Une réception correspond à une ligne (à ajouter avec le bouton +)

{% hint style="info" %}
Il est possible de créer une association BR sans UL à l'aide du bouton <mark style="background-color:blue;">**Sans arrivage**</mark><mark style="background-color:blue;">.</mark>
{% endhint %}

Lorsque tous les champs ont été renseignés, il suffit de cliquer sur le bouton <mark style="background-color:blue;">**Enregistrer**</mark>, ce qui créera l'association BR. Il sera possible de retrouver cette dernière dans le tableau présent sur la page.

### Supprimer une association

Afin de supprimer une association BR, il suffit de cliquer sur les<img src="../../.gitbook/assets/3-points.png" alt="" data-size="line">à gauche d'une ligne, puis <mark style="background-color:blue;">**Supprimer**</mark>. Une modale de confirmation va apparaitre, nécessitant l'approbation de la suppression de l'association. Lors du clic sur <mark style="background-color:blue;">**Supprimer**</mark>, l'association sera retirée du tableau.
