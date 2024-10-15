# Services

La demande de service permet de générer une demande indépendante du stock, et a pour objectif de réaliser des opérations au sein du site logistique. Cette dernière peut-être sous la forme d'une demande de réparation, pour du mobilier ou des machine, par exemple.

Cette fonctionnalité est disponible dans l'onglet **Demande**, puis **Services**. Cette page contient plusieurs éléments :&#x20;

* Une **barre de filtre**, permettant de filtrer les données qui sont affichées dans le tableau
* Une **recherche rapide**, permettant également de filtrer les données affichées dans le tableau
* Un bouton <mark style="background-color:blue;">**Exporter au format CSV**</mark>, destiné à exporter l'ensemble des données filtrées (suivant les dates renseignées) au format CSV
* Un bouton <mark style="background-color:blue;">**Gestion des colonnes**</mark>, permettant de choisir les colonnes à afficher dans le tableau
* Un **tableau**, regroupant les différentes demandes de services créées

{% hint style="info" %}
A contrario des autres pages de l'application, le bouton de création d'une demande de service se situe dans le menu d'action rapide

![](<../../../.gitbook/assets/image (34).png>)
{% endhint %}

### Contenu des filtres

| Filtre            | Description                                                                                                                                               |
| ----------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **Du**            | La tranche basse filtrant sur la date de création, la date attendue ou la date de réalisation de la demande de service (ce choix est fait via la flèche ) |
| **Au**            | La tranche haute filtrant sur la date de création, la date attendue ou la date de réalisation de la demande de service (ce choix est fait via la flèche ) |
| **Type**          | Le type des demandes de services à filtrer                                                                                                                |
| **Statuts**       | Le(s) statut(s) des demandes de services à filtrer, si vous indiquez un type les statuts affichés seront ceux paramétré pour ce type                      |
| **Demandeurs**    | Le(s) demandeur(s) des demandes de services à filtrer. Il s'agit du référentiel **Utilisateurs**.                                                         |
| **Objet**         | L'objet des demandes de services à filtrer                                                                                                                |
| **Destinataires** | Le(s) destinataire(s) des demandes de services à filtrer. Il s'agit du référentiel **Utilisateurs**.                                                      |
| **Urgences**      | Le(s) urgence(s) des demandes de services à filtrer. Il s'agit d'un paramétrage présent dans le **Paramétrage**.                                          |

### Contenu du tableau

| Colonne                               | Description                                                            |
| ------------------------------------- | ---------------------------------------------------------------------- |
| **Numéro de demande**                 | Le numéro de la demande de service                                     |
| **Date demande**                      | La date à laquelle la demande a été créée                              |
| **Type**                              | Le type de la demande de service                                       |
| **Demandeur**                         | L'utilisateur ayant créé la demande de service                         |
| **Objet**                             | L'objet de la demande                                                  |
| **Date attendue**                     | La date à laquelle la demande est attendue                             |
| **Date de réalisation**               | La date à laquelle la demande a été réalisée                           |
| **Statut**                            | Le statut de la demande                                                |
| **Urgence**                           | Le niveau d'urgence de la demande                                      |
| **Nombre d'opération(s) réalisée(s)** | Le nombre d'opérations qui ont été réalisées concernant cette demande  |
| **Traité par**                        | L'utilisateur ayant traité la demande                                  |
| **Destinataires**                     | Les destinataires de la demande, séparés par des virgules              |

### Créer une nouvelle demande de service

Afin de créer une nouvelle demande de service, il suffit cliquer sur le bouton <mark style="background-color:blue;">**Service**</mark> présent dans le menu d'action rapide. Une modale va alors s'ouvrir, permettant ainsi de renseigner plusieurs champs :&#x20;

* Le **type**
* Le **statut**
* L'**objet**
* La **date attendue**
* L'**urgence**
* Le **lieu de chargement**
* Le **lieu de déchargement**
* Le **nombre d'opérations réalisées**
* Le(s) **destinataire(s)**
* Les **champs libres**
* Le **commentaire**
* Les **pièces jointes**

{% hint style="info" %}
Le choix des statuts est conditionné par le champ **Type**. Il s'agit d'un paramétrage modifiable dans le menu [Paramétrage > Trace > Services > Statuts](broken-reference).
{% endhint %}

Lorsque tous les champs ont été renseignés, il suffit de cliquer sur le bouton <mark style="background-color:blue;">**Enregistrer**</mark>, ce qui créera la demande de service. Il sera possible de retrouver cette dernière dans le tableau présent sur la page.

### Visualiser une demande de service et changer son statut

Cliquez sur la ligne du service, vous allez arriver sur une page avec 2 colonnes. Sur la 1er, vous avez en haut le numéro de la demande et la personne qui l'a créé. Ensuite, vous avez les différents champs ([gestions des champs fixes](../../../parametrages/trace/services/champs-fixes.md)) que vous avez remplis lors de la création de votre demande, puis en dessous se situe une catégorie champs libres ([gestion des champs libres](../../../parametrages/trace/services/types-et-champs-libres.md)).

Sur la 2e colonne, vous avez une timeline qui reprend les différents statuts par lesquels est passé votre demande. Pour modifier le statut de votre demande cliqué sur <mark style="background-color:blue;">**Changer le statut**</mark>, une fenêtre va s'ouvrir et vous allez pouvoir sélectionner un nouveau statut. La liste des statuts proposés sont ceux renseigner dans le paramétrage ([gestion des statuts](../../../parametrages/trace/services/statuts.md)). <mark style="background-color:blue;">**Enregistrer**</mark> et la timeline va automatiquement s'actualiser. Une fois la demande traité, il est impossible de changer son statuts.

{% embed url="https://www.screencast.com/t/SrtUV3N9" %}
Visualisation et changement de statut
{% endembed %}

### Modifier une demande de service

Pour modifier une demande de service, 2 chemins :&#x20;

* Dans la liste des services, cliquez sur les<img src="../../../.gitbook/assets/Capture d’écran 2023-02-06 à 12.07.16 (1).png" alt="" data-size="line">d'une ligne de référence et cliquez sur le bouton <mark style="background-color:blue;">**Modifier**</mark> pour être redirigé vers la page de modification de service.
* Sur la visualisation d'une demande de service, cliquez sur <mark style="background-color:blue;">**Modifier**</mark> pour que la page passe en mode modification.

Vous pouvez modifier plusieurs champs de la demande, cela dépendra du paramétrage des champs fixes.

Néanmoins, il n'est pas possible de modifier les informations suivantes :&#x20;

* Le **type**
* Le **statut**
* La **date de réalisation**

L'utilisateur doit avoir le droit de modification pour voir apparaître les boutons <mark style="background-color:blue;">**Modifier**</mark>.&#x20;

{% embed url="https://www.screencast.com/t/HFeTu6e0" %}
Modifier une demande
{% endembed %}

### Supprimer une demande de service

Il est également possible de supprimer une demande de service en cliquant sur<img src="../../../.gitbook/assets/Capture d’écran 2023-02-06 à 12.07.16 (1).png" alt="" data-size="line">à gauche d'une ligne, puis <mark style="background-color:blue;">**Supprimer**</mark>. Une modale de confirmation va apparaitre, nécessitant l'approbation de la suppression de la demande. Lors du clic sur <mark style="background-color:blue;">**Supprimer**</mark>, la demande de service sera retirée du tableau. Il en va de même, dans le détails d'une demande de service.

