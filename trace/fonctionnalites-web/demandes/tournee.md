# Tournée

La demande de Tournée permet d'attribuer à un opérateur, un ordre de passage précis sur des emplacements pré-définis. Il peut, sur ces emplacements, faire des prises/déposes d'UL ou passage à vide si besoin.&#x20;

Cette fonctionnalité est disponible dans le menu Demande puis Tournée. Ou via le bouton + puis Tournée.&#x20;

Cette page contient :

* Une **barre de filtre**, permettant de filtrer les données qui sont affichées dans le tableau
* Une **recherche rapide**, permettant également de filtrer les données affichées dans le tableau
* Un bouton **Exporter au format CSV**, destiné à exporter l'ensemble des données filtrées (suivant les dates renseignées) au format CSV
* Un **tableau**, regroupant les différentes demandes de Tournées créées

### Contenu des filtres

<table><thead><tr><th width="251.52720639646054">Filtre</th><th>Description</th></tr></thead><tbody><tr><td><strong>Du</strong></td><td>La tranche basse filtrant sur la date de création de la demande de tournée</td></tr><tr><td><strong>Au</strong></td><td>La tranche haute filtrant sur la date de création de la demande de tournée</td></tr><tr><td><strong>Statut</strong></td><td>Le(s) statut(s) des demandes de tournée à filtrer</td></tr><tr><td><strong>Type</strong></td><td>Le type des demandes de tournée à filtrer</td></tr><tr><td><strong>Emplacement de la tournée</strong></td><td>Filtrer la demande par l'emplacement de la tournée. Cet emplacement est pré-défini lors du paramétrage de la tournée. C'est l'emplacement sur lequel l'opérateur viendra faire sa tournée </td></tr></tbody></table>

### Contenu du tableau

| Colonne                                | Description                                                                                                                                                            |
| -------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **Numéro**                             | Numéro de la demande de tournée généré par l'application Wiilog. Il est constitué du préfixe TO, de l'année, du mois, du jour, de l'heure et de la minute de création. |
| **Date de création**                   | Date de création de la demande de tournée                                                                                                                              |
| **Date et heure de démarrage attendu** | Date et heure auxquelles l'opérateur doit démarrer la tournée. Elles sont indiquées lors de la création d'une tournée.                                                 |
| **Date de traitement**                 | Date et heure auxquelles la tournée a été terminée.                                                                                                                    |
| **Statut**                             | Statut de la demande de tournée                                                                                                                                        |
| **Type**                               | Type de la demande de tournée                                                                                                                                          |
| **Traité par**                         | L'utilisateur qui à traité la demande de tournée                                                                                                                       |
| **Demandeur**                          | Le demandeur de la demande de tournée                                                                                                                                  |
| **Urgence**                            | Si la demande est classée urgence et sous quel délai                                                                                                                   |
| **Commentaire**                        | Le commentaire associé à la demande de tournée                                                                                                                         |
| **Emplacement** de la tournée          | L'emplacement sur lequel l'opérateur va faire sa tournée (ex: chariot\_01)                                                                                             |

### Créer une demande de tournée

#### Via le bouton "+"

<div align="left"><figure><img src="../../../.gitbook/assets/Capture d’écran 2025-11-26 à 14.46.18.png" alt=""><figcaption></figcaption></figure></div>

Au clic sur la tournée une modale "Nouvelle demande de tournée" s'ouvrira comprenant :

<figure><img src="../../../.gitbook/assets/Capture d’écran 2025-11-26 à 16.13.51.png" alt=""><figcaption></figcaption></figure>



* **Type**&#x20;
* **Statut**
* **Date et heure de démarrage attendu**
* **Emplacement de la tournée**
* **Urgence**
* **Champs libres**

{% hint style="info" %}
Le choix des statuts est conditionné par le champ **Type**. Il s'agit d'un paramétrage modifiable dans le menu Paramétrages > Trace > tournées
{% endhint %}

### Passer les statuts d'une demande de tournée

Cliquer sur la ligne de la demande de tournée concernée.&#x20;

Ci-dessous une vidéo explicative avec vue WEB + vue NOMADE.&#x20;

Ici, comme exemple, l'opérateur va faire des prises, déposes et passage à vide sur les emplacements de sa tournée. Les UL "Cadeau1" ou "Surprise1" sont créées manuellement mais peuvent être scannées par l'opérateur.

De même pour sélectionner un emplacement, il doit le scanner.

{% file src="../../../.gitbook/assets/Vidéo Tournée.mov" %}



***

## Mode opératoire — Fonctionnalité « Tournée » — Fonctionnalité « Tournée » (voir vidéo ci-dessus)

Ce document décrit étape par étape le déroulement d’une tournée telle qu’elle est réalisée dans cette vidéo, avec la **Vue WEB** (à gauche) et la **Vue NOMADE** (à droite). Il sert de mode d’emploi utilisateur pour comprendre le fonctionnement complet : navigation, exécution d’opérations (déposer, prendre, passage à vide) et consultation du récapitulatif final.

***

#### 1. Démarrage de la tournée

1. L’opérateur ouvre l’application **NOMADE** et sélectionne la tournée assignée depuis Traçabilité > Tournée puis clique sur démarrer la tournée.&#x20;
2. La **Vue WEB** affiche simultanément la tournée en cours, avec la liste des étapes et leurs statuts initiaux (_non commencé_ ou _en attente_).

#### 2. Arrivée sur un emplacement

1. Sur NOMADE, l’opérateur sélectionne l'emplacement suivant en scannant. Chaque emplacement peut donner lieu à une ou plusieurs actions.

#### 3. Déposer une unité logistique

1. Depuis l’emplacement sur NOMADE, sélectionner **Déposer**.
2. Choisir l’unité logistique à déposer (ex. : _cadeau1_).
3. Confirmer l’opération.
4. Un message confirme la réussite.

**Effet côté WEB** :

* l’étape affiche le statut **Déposé**,
* l’unité est enregistrée dans l’historique de la tournée avec l’heure et le nom de l’opérateur.

***

#### 3.2. Prendre une unité logistique

1. Depuis l’écran de l’emplacement, sélectionner **Prendre**.
2. Choisir ou scanner l’unité à récupérer.
3. Confirmer l’opération.
4. L’application affiche une confirmation.

**Effet côté WEB** :

* le système enregistre une opération **Prise**,
* l’unité apparaît comme récupérée dans le récapitulatif.

***

#### 3.3. Effectuer un passage à vide

1. Dans l’emplacement, sélectionner **Passage à vide**.
2. Valider l’opération.

**Effet côté WEB** :

* le stop est marqué comme **Visité – Passage à vide**,
* aucune unité logistique n’est associée à l’étape.

### 4. Validation de l’étape

Après avoir réalisé les opérations prévues :

1. L’opérateur clique sur **Terminer l’étape**.
2. La NOMADE passe automatiquement à l’emplacement suivant.
3. La WEB met à jour le statut (_Réalisé_, _Déposé_, _Pris_ ou _Passage à vide_ selon le cas).

### 5. Fin de la tournée

#### 5.1. Clôture sur NOMADE

1. Lorsque toutes les étapes sont traitées, l’application affiche un bouton **Terminer la tournée**.
2. L’opérateur confirme la fermeture.
3. La tournée bascule en statut **Terminée**.

#### 5.2. Visualisation du récapitulatif sur WEB

La Vue WEB présente un ensemble d’informations utiles :

**• Liste complète des emplacements**

* Statut final de chaque étape
* Heure d’arrivée
* Type d’action : Dépose, Prise, Passage à vide
* Unités logistiques manipulées

**• Détails chronologiques**

* Historique horodaté de toutes les opérations
* Identification de l’opérateur ayant réalisé chaque action

## Page des détails d'une tournée

#### Tournée

Le module tourrnée permet de voir l'avancée des statuts de la tournée . Pour rappel, les statuts sotn paramétrables depuis les parametres de la tournée. Les 3 points à gauche permettent de modifier, supprimer ou terminer la tournée.&#x20;

On retrouve sous ce module les Pièces jointes ou les commentaires associés. Ces derniers ont été ajouté sur nomade pendant la tournée de l'opérateur

#### Chemin opérateur

Le chemin opérateur correspond aux emplacements paramétrés par type de tournée. On retrouve également le nombre d'UL prises ou déposées par emplacement.

#### Historique

On retrouve l'historique des actions faites par l'opérateur (date/heure/emplacement/quantité). Si l'opérateur ajoute un emplacment lors de sa tournée, l'information est remontée dans cet historique.

#### Information

Les informations conernées par la création de cette tournée. Date de démarrage / de traitement / de création et Emplacmeent de Tournée (chariot de l'opérateur).

#### UL sur emplacement

LA liste des UL sur l'emplacement de tournée. Les encours sur cet emplacement doivent être vide à la fin de la tournée pour pouvoir la terminer



<figure><img src="../../../.gitbook/assets/Capture d’écran 2026-02-18 à 16.42.22.png" alt=""><figcaption></figcaption></figure>



{% hint style="info" %}
Toutes les actions et tous les mouvements sont archivés dans le menu Traçabilité > mouvements
{% endhint %}

***

