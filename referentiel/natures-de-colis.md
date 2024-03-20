---
description: >-
  Les natures de colis permettent de venir différencier les marchandises reçues
  par catégorie. Elles sont utilisées dans la brique Trace.
---

# Natures de colis

Ces derniers sont consultables dans l'onglet **Référentiel**, puis **Nature de colis**. Cette page contient plusieurs éléments :&#x20;

* Une **recherche rapide**, permettant de filtrer les données affichées dans le tableau
* Un bouton <mark style="background-color:blue;">**Ajouter nature colis**</mark>, pour créer une nouvelle nature de colis
* Un **tableau**, regroupant les différents types de natures de colis créées

### Contenu du tableau

| Colonne                           | Description                                                                                          |
| --------------------------------- | ---------------------------------------------------------------------------------------------------- |
| **Libellé**                       | Libellé de la nature, apparaîtra sur les formulaires                                                 |
| **Code**                          | Code de la nature de colis                                                                           |
| **Quantité par défaut**           | Nombre de colis par défaut qui sera préremplie lors de la création d'un nouvel arrivage              |
| **Préfixe**                       | Préfixe qui figurera sur le numéro de colis généré lors d'un arrivage avec des colis de cette nature |
| **Couleur**                       | Couleur de cette nature apparaissant sur les dashboard, et sur le nomade                             |
| **Description**                   | Description de la nature                                                                             |
| **Synchronisation nomade**        | <p>Possibilité de sélectionner cette nature de colis pour un colis sur le nomade<br>Oui/Non</p>      |
| **Affichage sur les formulaires** | Liste des formulaires sur lesquels la nature apparaît                                                |
| **Températures**                  | Plages de température associées à la nature                                                          |

### Créer une nouvelle nature de colis

Pour créer une nouvelle nature de colis, cliquez sur <mark style="background-color:blue;">**Ajouter nature colis**</mark>. Une modale va alors s'ouvrir, permettant ainsi de renseigner plusieurs champs :&#x20;

* Le **label** (libellé) de la nature de colis, obligatoire
* Le **code** de la nature de colis, obligatoire
* La **description** de la nature de colis
* La **quantité par défaut** de la nature de colis qui sera renseignée sur le formulaire de création des arrivages, obligatoire
* La **couleur** de la nature de colis qui apparaîtra sur les dahsboard et sur le nomade, obligatoire
* Le **préfixe** de la nature de colis qui apparaîtra sur le numéro de colis généré suite à un arrivage
* Le switch **Synchronisation nomade ?**. Ce paramétrage sert quand vous scannez un colis, avec le terminal mobile, non connu de l'application et que souhaitez lui assigner une nature. Le choix de la nature se fera parmi les natures ayant la synchronisation nomade activée
* Le switch **Nature par défaut (acheminements)**. Ce paramétrage permet d'identifier la nature comme nature par défaut lors de la création d'un acheminement : si un colis ajouté sur un acheminement n'a pas de nature connue, il aura pas défaut cette nature paramétrée
* Le switch **Affichage sur les formulaires ?**. Ce paramétrage sert à décider si la nature apparaît ou non sur le formulaire choisi
  * **Arrivage** : si vous cochez _**Arrivage**_, cette nature sera disponible parmi les natures possibles d'unité logistique créé à l'arrivage
  * **Transport - Collecte** : si vous cochez _**Transport - Collecte**_, la nature sera disponible parmi les natures de colis à collecter sur les demandes de transport de collecte. Il vous faut également choisir les types de demande de transport de collecte sur lesquels la nature doit apparaître
  * **Transport - Livraison**: si vous cochez _**Transport - Livraison**_, la nature sera disponible parmi les natures de colis à collecter sur les demandes de transport de livraison. Il vous faut également choisir les types de demande de transport de livraison sur lesquels la nature doit apparaître
  * **Températures** : associer des plages de températures (les plages de température doivent au préalable avoir été paramétrées dans la page Track > Températures) à la nature pour pouvoir la sélectionner lors de la création d'une demande de transport

{% embed url="https://www.screencast.com/t/OHfg9I4fC" %}
Modale de création d'une nature
{% endembed %}

Cliquez sur <mark style="background-color:blue;">**Enregistrer**</mark> pour valider l'ajout de la nature de colis.&#x20;

### Modifier une nature de colis

Pour modifier une nature de colis, cliquez sur la ligne de la nature de colis à modifier pour ouvrir la modale de modification.

Modifiez ensuite les champs de la même façon qu'à la création et cliquez sur **Enregistrer**.&#x20;

### Supprimer une nature de colis

Il est également possible de supprimer une nature de colis en cliquant sur les trois points à gauche d'une ligne, puis **Supprimer**. Une modale de confirmation va apparaitre, nécessitant l'approbation de la suppression de la nature. Si la nature de colis est déjà utilisé dans l'application, vous ne pourrez pas le supprimer et une modale d'erreur apparaîtra.&#x20;
