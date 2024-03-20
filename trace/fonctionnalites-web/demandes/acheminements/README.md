# Acheminements

Les acheminements permettent de déplacer une unité de manutention qui ne se trouve pas dans le stock. Il s'agit d'une fonctionnalité annexe à la gestion de stock.

Cette fonctionnalité est disponible dans l'onglet **Demande**, puis **Acheminements**. Cette page contient plusieurs éléments :&#x20;

* Une **barre de filtre**, permettant de filtrer les données qui sont affichées dans le tableau
* Une **recherche rapide**, permettant également de filtrer les données affichées dans le tableau
* Un bouton **Exporter au format CSV**, destiné à exporter l'ensemble des données filtrées (suivant les dates renseignées) au format CSV
* Un bouton **Gestion des colonnes**, permettant de choisir les colonnes à afficher dans le tableau
* Un **tableau**, regroupant les différentes demandes d'acheminement créées

{% hint style="info" %}
A contrario des autres pages de l'application, le bouton de création d'une demande d'acheminement se situe dans le menu d'action rapide

![](<../../../../.gitbook/assets/image (72).png>)
{% endhint %}

### Contenu des filtres

| Filtre                 | Description                                                                                              |
| ---------------------- | -------------------------------------------------------------------------------------------------------- |
| **Du**                 | La tranche basse filtrant sur la date de création de la demande d'acheminement                           |
| **Au**                 | La tranche haute filtrant sur la date de création de la demande d'acheminement                           |
| **Numéro de demande**  | Le numéro d'acheminement à filtrer                                                                       |
| **Statuts**            | Le(s) statut(s) des demandes d'acheminement à filtrer                                                    |
| **Types**              | Le(s) types(s) des demandes d'acheminement à filtrer                                                     |
| **Demandeurs**         | Le(s) demandeur(s) des demandes d'acheminement à filtrer. Il s'agit du référentiel **Utilisateurs**.     |
| **Transporteurs**      | Le(s) transporteur(s) des demandes d'acheminement à filtrer. Il s'agit du référentiel **Transporteurs**. |
| **Urgences**           | Le(s) urgence(s) des demandes d'acheminement à filtrer                                                   |
| **Destinataires**      | Le(s) destinataire(s) des demandes d'acheminement à filtrer. Il s'agit du référentiel **Utilisateurs**.  |
| **Numéro de commande** | Le numéro de commande des demandes d'acheminement à filtrer                                              |
| **Destination**        | La destination des demandes d'acheminement à filtrer. Il s'agit du référentiel **Emplacements**.         |

### Contenu du tableau

| Colonne                | Description                                               |
| ---------------------- | --------------------------------------------------------- |
| **Numéro demande**     | Le numéro de la demande                                   |
| **Transporteur**       | Le transporteur de la demande                             |
| **Numéro de commande** | Le numéro de commande de la demande                       |
| **Date de création**   | La date à laquelle la demande a été créée                 |
| **Date de validation** | La date à laquelle la demande a été validée               |
| **Date de traitement** | La date à laquelle la demande a été traitée               |
| **Date d'échéance**    | La date d'échéance de fin de la demande                   |
| **Type**               | Le type de la demande                                     |
| **Demandeur**          | Le demandeur de la demande                                |
| **Destinataires**      | Les destinataires de la demande, séparés par des virgules |
| **Emplacement prise**  | L'emplacement de prise de la demande                      |
| **Emplacement dépose** | L'emplacement de dépose de la demande                     |
| **Destination**        | La destination de la demande                              |
| **Nb colis**           | Le nombre de colis présents dans la demande               |
| **Statut**             | Le statut de la demande                                   |
| **Urgence**            | Le niveau d'urgence de la demande                         |
| **Traité par**         | L'opérateur ayant traité la demande                       |
| _**Champs libres**_    | Les différents champs libres de la demande                |

### Créer une nouvelle demande d'acheminement

Afin de créer une nouvelle demande d'acheminement, il suffit cliquer sur le bouton **Acheminement** présent dans le menu d'action rapide. Une modale va alors s'ouvrir, permettant ainsi de renseigner plusieurs champs :&#x20;

* Le **type**
* Le **statut**
* Le **demandeur**
* L'**emplacement de prise**
* L'**emplacement de dépose**
* L'**urgence**
* Le **transporteur**
* Le **numéro de tracking transporteur**
* La **destination**
* Le **numéro de commande**
* Le **numéro de projet**
* Le(s) **destinataire(s)**
* Le **business unit**
* La/les **date(s) d'échéance**
* Les **champs libres**
* Le **commentaire**
* La/les **pièce(s) jointe(s)**

{% hint style="info" %}
Le choix des statuts est conditionné par le champ **Type**. Il s'agit d'un paramétrage modifiable dans le menu **Paramétrage** > **Trace** > **Acheminements**, puis **Statuts**.
{% endhint %}

Lorsque tous les champs ont été renseignés, il suffit de cliquer sur le bouton **Enregistrer**, ce qui créera la demande d'acheminement. Il sera possible de retrouver cette dernière dans le tableau présent sur la page.

### Visualiser une demande d'acheminement

Afin de visualiser les détails d'une demande d'acheminement, il suffit de cliquer sur la ligne de cette dernière. Une page de détails de l'acheminement va alors apparaitre, contenant plusieurs éléments, dont :

* Les différentes valeurs des champs renseignés lors de la création/modification
* Un bouton Valider/Terminer la demande, permettant de modifier le statut de la demande
* Un bouton Retour au statut brouillon, permettant de rétablir la demande au statut brouillon
* Un bouton Générer un bon de livraison
* Un bouton Générer un bon de surconsommation
* Un bouton Générer une lettre de voiture
* Un bouton Générer un bon d'acheminement
* Un bouton Modifier, permettant de modifier la demande
* Un bouton Supprimer, permettant de supprimer la demande
* Une liste des colis contenus dans l'acheminement

### Modifier une demande d'acheminement

Afin de modifier une demande d'acheminement existante, il suffit de cliquer sur le bouton **Modifier** présent dans les détails de cette dernière. Une modale d'édition va s'ouvrir, permettant de modifier plusieurs champs de la demande. Néanmoins, il n'est pas possible de modifier les informations suivantes :&#x20;

* Le **type**
* Le **statut**

### Supprimer une demande d'acheminement

Il est également possible de supprimer une demande d'acheminement en cliquant sur le bouton **Supprimer** présent dans les détails de cette dernière. Une modale de confirmation va apparaitre, nécessitant l'approbation de la suppression de la demande. Lors du clic sur **Supprimer**, une redirection sera effectuée vers le tableau et la demande de d'acheminement sera supprimée.

## Tableau des colis

Ce tableau recense tous les colis qui ont été ajoutés dans la demande d'acheminement.

### Contenu du tableau

| Colonne                    | Description                                                                      |
| -------------------------- | -------------------------------------------------------------------------------- |
| **Code**                   | Le code de l'unité de manutention                                                |
| **Quantité à acheminer**   | La quantité à acheminer pour cette unité de manutention                          |
| **Nature**                 | La nature de l'unité de manutention                                              |
| **Poids**                  | Le poids de l'unité de manutention, exprimé en kg                                |
| **Volume**                 | Le volume de l'unité de manutention, exprimé en m³                               |
| **Commentaire**            | Le commentaire associé à l'unité de manutention                                  |
| **Date dernier mouvement** | La date du dernier mouvement de traçabilité associé à cette unité de manutention |
| **Dernier emplacement**    | Le dernier emplacement connu concernant cette unité de manutention               |
| **Opérateur**              | L'opérateur ayant mouvementé cette unité de manutention pour la dernière fois    |
| **Statut**                 | Le statut de l'unité de manutention au sein de la demande d'acheminement         |
