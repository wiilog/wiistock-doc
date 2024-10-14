# Collectes

La demande de collecte sert à demander de venir récupérer une ou plusieurs références qui sont à remettre en stock, ce qui incrémente le stock, ou à mettre en destruction, ce qui ne change pas le stock.

Cette fonctionnalité est disponible dans le menu <mark style="background-color:blue;">**Demande**</mark>, puis <mark style="background-color:blue;">**Collectes**</mark>. Cette page contient plusieurs éléments :&#x20;

* Une **barre de filtre**, permettant de filtrer les données qui sont affichées dans le tableau
* Une **recherche rapide**, permettant également de filtrer les données affichées dans le tableau
* Un bouton **Exporter au format CSV**, destiné à exporter l'ensemble des données filtrées (suivant les dates renseignées) au format CSV
* Un **tableau**, regroupant les différentes demandes de collectes créées

### Contenu des filtres

<table><thead><tr><th width="251.52720639646054">Filtre</th><th>Description</th></tr></thead><tbody><tr><td><strong>Du</strong></td><td>La tranche basse filtrant sur la date de création de la demande de collecte</td></tr><tr><td><strong>Au</strong></td><td>La tranche haute filtrant sur la date de création de la demande de collecte</td></tr><tr><td><strong>Statuts</strong></td><td>Le(s) statut(s) des demandes de collecte à filtrer</td></tr><tr><td><strong>Utilisateurs</strong> </td><td>Pour filtrer sur la personne ayant créée la demande de collecte. Vous pouvez renseigner plusieurs utilisateurs. Ce filtre va chercher dans la liste des utilisateurs renseignées dans l'application. Vous devez taper une première lettre pour avoir une suggestion d'utilisateurs contenant cette lettre</td></tr><tr><td><strong>Type</strong></td><td>Le type des demandes de collecte à filtrer</td></tr></tbody></table>

### Contenu du tableau

| Colonne        | Description                                                                                                                                                                          |
| -------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| **Création**   | Date de création de la demande de collecte (demande créée au statut Brouillon)                                                                                                       |
| **Validation** | Date de validation de la demande de collecte (passage du statut Brouillon à A traiter)                                                                                               |
| **Demandeur**  | Personne ayant créé la demande de collecte                                                                                                                                           |
| **Numéro**     | Numéro de la demande de collecte généré par l'application Wiilog. Il est constitué du préfixe C, de l'année, du mois, du jour, de l'heure, de la minute et de la seconde de création |
| **Objet**      | Objet de la demande de collecte                                                                                                                                                      |
| **Statut**     | Statut de la demande de collecte                                                                                                                                                     |
| **Type**       | Type de la demande de collecte                                                                                                                                                       |

## Créer une demande de collecte

### Via le bouton "+"

Dans le bouton d'action rapide, sélectionnez **Collecte** pour créer une demande de collecte.

![](<../../../.gitbook/assets/image (8) (1).png>)

Une modale s'ouvrira alors pour remplir les informations d'entête de la demande :&#x20;

* **Demandeur** : personne créant la demande. Il n'est pas possible de changer ce champ. Par défaut, ce champ se remplit avec la personne connectée.
* **Type** : type de la demande. Le type permet de venir définir plus précisément le flux de demande. Sa sélection permet de faire apparaître les champs libres associés au type de collecte (pour paramétrer les champs libres : [<mark style="color:blue;">Paramétrage > Stock > Demandes > Collecte - Types et champs libres</mark>](collectes/types-et-champs-libres.md)). Le choix de type conditionne aussi le choix du point de collecte. Selon le type, il sera possible de sélectionner seulement les emplacements autorisés sur le type (à aller paramétrer directement sur l'emplacement : [Référentiel > Emplacements](../../../referentiel/emplacements.md)). Le type n'est plus modifiable une fois la demande validée.
* **Objet\*** : objet de la collecte. Champ texte libre.
* **Point de collecte\***: une fois le type sélectionné, vous pouvez choisir l'emplacement de collecte. Pour cela, commencez à taper la première lettre de l'emplacement souhaité. Vous pouvez directement faire apparaître les emplacements possibles, si le paramétrage "Gérer le champ "Point de collecte" en liste déroulante" est activé ([Paramétrage > Stock > Demandes > Collectes](collectes/))
* **Destination\*** :&#x20;
  * **Destruction** : les références / les articles collectés doivent être détruits
  * **Mise en stock** : les références / les articles collectés doivent être remis en stock
* **Champs libres :** remplissez les champs libres s'il y en a de paramétrés
* **Commentaire :** vous avez également la possibilité d'ajouter un commentaire

En cliquant sur <mark style="background-color:blue;">**Enregistrer**</mark>, la demande de collecte est créée au statut brouillon et vous êtes redirigé vers le **détail de la demande**.

Le **détail** est constitué de :&#x20;

* une **entête**. Elle contient les différents champs renseignés précédemment ainsi que la demande de création et de validation&#x20;
* le **tableau** de la **liste des articles**, qui a les colonnes suivantes :&#x20;

| Colonne         | Description                               |
| --------------- | ----------------------------------------- |
| **Référence**   | Référence à collecter                     |
| **Libellé**     | Libellé de la référence à collecter       |
| **Emplacement** | Même emplacement que le point de collecte |
| **Quantité**    | Quantité à collecter                      |

Pour ajouter un article, cliquez sur <mark style="background-color:blue;">**Ajouter article**</mark>**.**

Une modale s'ouvrira alors. Tapez le code de la référence pour faire apparaître les autres champs. La modale est constituée de ces champs :&#x20;

* **Référence\*** : référence à collecter
* **Code article (laisser vide pour créer un nouvel article)\***, _selon paramétrage_ : si la collecte est une mise en stock, si la référence est en gestion quantité par article et que votre rôle est en ajout quantité par article, ce champ apparaîtra. Vous pouvez indiquer ainsi de collecter un article qui est sorti du stock sur le dernier mois pour qu'il soit remis en stock, ou alors ne rien mettre. Un article sera automatiquement créé alors lors de la génération de l'ordre de collecte&#x20;
* **Quantité à collecter\*** : quantité de la référence à collecter

Remplissez les différents champs et cliquez sur <mark style="background-color:blue;">**Ajouter**</mark>.&#x20;

Répéter l'opération autant de fois que de référence que vous souhaitez faire collecter.&#x20;

Une fois que vous avez fini de faire votre demande de collecte, cliquez sur <mark style="background-color:blue;">**Valider**</mark> pour que votre collecte soit prise en compte et traitée.

Un ordre de collecte sera alors créé.

{% embed url="https://www.screencast.com/t/PdONks3tX" %}
Ajouter un article à la collecte
{% endembed %}

### Via le panier

Le fonctionnement du panier est détaillé précisément dans [Panier](../../../stock/fonctionnalites-web/panier.md).

Pour créer une demande de collecte via le panier, allez dans la page _Stock > Références_, et cliquez sur l'icône Panier de chaque référence qui vous souhaitez faire collecter.

Cliquez ensuite sur l'icône Panier dans l'entête pour aller dans le panier.&#x20;

Sélectionnez le type de demande Collecte, et sélectionnez _Créer une nouvelle demande_ pour faire une nouvelle demande. La section _Ma nouvelle demande de collecte_ apparaît alors. Remplissez les champs _Type_, _Objet_, _Point de collecte_, et _Destination_, les _champs libres_, et le _commentaire_ si besoin. Ils ont la même logique que décrit au dessus.

Sur la zone à droite, renseignez les quantités à se collecter pour chaque référence.&#x20;

Il n'y aura pas de sélection d'article dans le panier même si vous êtes en ajout quantité par article.&#x20;

Cliquez sur <mark style="background-color:blue;">**Valider mon panier**</mark> ensuite pour créer la demande en brouillon et être redirigé vers le détail de la demande expliqué au dessus.&#x20;

<mark style="background-color:blue;">**Validez**</mark> la demande pour qu'elle soit prise en compte et traitée ensuite.

{% embed url="https://www.screencast.com/t/kSJ5ksb0rCRH" %}
Ajout via le panier
{% endembed %}

## Modifier une demande de collecte

{% hint style="info" %}
Il est possible de modifier une demande de collecte tant que celle-ci est en brouillon.
{% endhint %}

Pour cela, cliquez sur la flèche à droite de <mark style="background-color:blue;">**Valider**</mark>, et sur <mark style="background-color:blue;">**Modifier**</mark>. Vous aurez ensuite la possibilité de modifier la date de la collecte, l'objet de la collecte, le point de collecte, et la destination, ses champs libres et son commentaire.

<mark style="background-color:blue;">**Enregistrer**</mark> pour valider les modifications

## Supprimer une demande de collecte

La suppression d'une demande de collecte est directement possible si celle-ci est en brouillon.

Pour cela, cliquez sur la flèche à droite de <mark style="background-color:blue;">**Valider**</mark>, et sur <mark style="background-color:blue;">**Supprimer**</mark>. La demande sera alors supprimée.

**Si la demande est en statut à traiter**, il vous faudra supprimer l'ordre de collecte pour que la demande liée soit passée en état brouillon et qu'elle soit supprimable à son tour.

{% hint style="info" %}
Si la demande est collectée, il n'est plus possible de la supprimer.&#x20;
{% endhint %}

## Visualiser une demande de collecte

Pour accéder au détail de la demande de collecte, cliquez sur la ligne de la demande que vous souhaitez voir. Vous arriverez alors sur le détail de la demande.&#x20;

Dans l'entête de la demande, vous avez une flèche qui donne accès au bouton <mark style="background-color:blue;">**Aller vers l'ordre de collecte**</mark>. Si la demande a été partiellement collectée à un moment, le bouton s'appellera Aller vers les ordres de collecte car plusieurs ordres de collecte auront été généré.&#x20;

En cliquant sur ce bouton, vous serez redirigé vers le détail de l'ordre de collecte généré par la demande dans le cas où il n'y a pas eu de traitement partiel. Dans le cas d'un traitement partiel, le bouton redirigera vers la liste des ordres de collecte liés à la demande.&#x20;

## Workflow d'une demande de collecte

Une demande de collecte passe par les statuts suivants :&#x20;

* **brouillon** : la demande vient d'être créer mais est toujours en cours de constitution. Elle n'a pas été encore validée
* **à traiter** : la demande a été validée et doit être traitée. L'ordre de collecte a été générée, il est en statut à traiter (Documentation Ordre de collecte : [Stock > Ordres > Collectes](../../../stock/fonctionnalites-web/ordres/collectes.md))
* **partiellement collecté** : toutes les références n'ont pas été collectées sur l'ordre de collecte ce qui a généré un nouvel ordre de collecte à traiter. La demande passe alors en partiellement collecté
* **collecté** : toutes les références demandées sont collectées. L'ordre de collecte / tous les ordres de collecte sont traités ce qui passe la demande à _Collecté_

