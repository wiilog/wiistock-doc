# Unités logistiques

La page des unités logistiques récapitule tous les UL créés sur l'application Wiilog, ainsi que les groupes d'UL.

Pour accéder à la page, vous devez aller dans le menu **Traçabilité**, puis choisir **Unités logistiques**.

La page des unités logistiques contient plusieurs éléments :&#x20;

* Une **barre de filtre**, permettant de filtrer les données qui sont affichées dans les tableaux
* Une **recherche rapide**, permettant également de filtrer les données affichées dans les tableaux
* Un bouton <mark style="background-color:blue;">**Exporter au format CSV**</mark> destiné à exporter l'ensemble des données filtrées (suivant les dates renseignées) au format CSV
* 2 **onglets** Unités logistiques et Groupes
* Un **tableau** dans chaque onglet, l'un avec la liste des unités logistiques, l'un avec la liste des groupes

### Contenu des filtres

Une fois que vous avez renseigné vos filtres, cliquez sur <mark style="background-color:blue;">**Filtrer**</mark>. Les filtres sont conservés d'une session à l'autre (ils seront toujours actifs si vous changez de page ou que vous vous déconnectez et reconnectez).

| Filtre                 | Description                                                                                                                                                                                                                                                           |
| ---------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **Du**                 | La tranche basse filtrant sur la date de dernier mouvement du colis                                                                                                                                                                                                   |
| **Au**                 | La tranche haute filtrant sur la date de dernier mouvement du colis                                                                                                                                                                                                   |
| **Unités logistiques** | Tapez le numéro d'UL sur lequel vous souhaitez faire une recherche                                                                                                                                                                                                    |
| **Natures**            | Sélectionnez les natures d'UL sur lesquelles vous souhaitez filtrer la liste des unités logistiques                                                                                                                                                                   |
| **Emplacement**        | <p>Renseignez ici un emplacement pour voir tous les UL dont le dernier emplacement connu est cet emplacement<br><em><mark style="color:orange;">Attention, cela ne signifie pas que l'UL est à cet emplacement si son dernier mouvement est une prise</mark></em></p> |
| **n° d'arrivage**      | Tapez ici un numéro d'arrivage pour avoir tous les UL issus de cet arrivage                                                                                                                                                                                           |

### Onglet Unités logistiques

#### Contenu du tableau

| Colonne                       | Description                                                                                                                                                                                                                                              |
| ----------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **Numéro UL**                 | Numéro du colis. Ce numéro peut être un numéro résultant de la création d'un arrivage, d'une unité de manutention ajoutée sur un acheminement, ou sur une prise/dépose, ou de la création d'une réception (numéro d'article ou de référence dans ce cas) |
| **Nature d'UL**               | Nature associée au UL. Pour le cas des unités logistiques  résultants de réception, il n'y aura pas de nature d'UL                                                                                                                                       |
| **Quantité**                  | Quantité dans l'unité logistique                                                                                                                                                                                                                         |
| **Date du dernier mouvement** | Date et heure du dernier mouvement de l'UL                                                                                                                                                                                                               |
| **Issu de**                   | Lien vers l'arrivage, l'acheminement ou la réception dont est issu l'UL                                                                                                                                                                                  |
| **Emplacement**               | Dernier emplacement du dernier mouvement connu de l'UL                                                                                                                                                                                                   |

Sur chaque ligne d'UL peut aussi apparaître un logo wifi si l'UL est lié ou a été lié à un objet connecté.&#x20;

![](<../../.gitbook/assets/image (82).png>)

Si la ligne a un logo wifi, un bouton <mark style="background-color:blue;">**Historique des données**</mark> est présent en plus sous les<img src="../../.gitbook/assets/3-points.png" alt="" data-size="line">. Il ouvre une page permettant de suivre toutes les données remontées par les capteurs qui ont été associés à cette UL (Voir la partie [IoT](broken-reference)).

#### Modifier une unité logistique

Vous pouvez modifier les informations d'une UL en cliquant sur <mark style="background-color:blue;">**Modifier**</mark> dans les<img src="../../.gitbook/assets/3-points.png" alt="" data-size="line">de la ligne souhaité. Une modale s'ouvrira alors avec les éléments suivants :&#x20;

* **Numéro UL :** numéro de l'unité logistique, champ non modifiable
* **Nature\* :** ce champ est modifiable et est obligatoire pour valider le formulaire
* **Quantité :** quantité connue dans l'UL, champ modifiable
* **Poids (kg) :** poids de l'UL, champ modifiable. Ce champ est pertinent dans le cadre d'un acheminement avec la génération de lettre de voiture
* **Volume (m3) :** volume de l'UL, champ modifiable. Ce champ est pertinent dans le cadre d'un acheminement avec la génération de lettre de voiture
* **Commentaire :** commentaire pour ajouter de l'information supplémentaire sur l'UL, champ modifiable
* **Historique de groupage :** tableau permettant de connaitre dans quels groupes est passé l'UL avec les colonnes suivantes&#x20;
  * **Groupe :** nom du groupe de l'UL dans lequel a été mis l'UL
  * **Date :** date à laquelle l'UL a été mis ou enlevé du groupe
  * **Type :** groupage/dégroupage. Groupage : l'UL a été mis dans le groupe. Dégroupage : l'UL a été enlevé du groupe

N'oubliez pas d'enregistrer vos modifications.&#x20;

#### Supprimer une unité logistique

Vous pouvez supprimer une UL en cliquant sur les<img src="../../.gitbook/assets/3-points.png" alt="" data-size="line">de la ligne du colis souhaité et en cliquant sur <mark style="background-color:blue;">**Supprimer**</mark>.&#x20;

Vous devez avoir au préalable supprimé tous les mouvements et éléments associés a l'UL avant de le supprimer. Si ce n'est pas le cas, vous obtiendrez un message d'erreur

### Onglet Groupes

#### Contenu du tableau

Ici la présentation des éléments diffèrent des tableaux habituels. Nous avons des systèmes de zones et étiquettes pour représenter chaque groupe avec chaque unité logistique contenu dans le groupe.

Un groupe est une unité logistique pouvant contenir d'autre unité logistique. Lorsque un mouvement sera appliqué sur un groupe, celui-ci sera aussi appliqué à toutes les UL contenus dans ce groupe. Si le groupe est vide, vous pouvez le déplacer comme uneUL.

{% embed url="https://www.screencast.com/t/YG9oTTNXqf" %}
Onglet groupe
{% endembed %}

{% hint style="info" %}
Pour réaliser un groupage, allez dans la page [Traçabilité > Mouvements](mouvements-de-tracabilite.md), ou alors sur le nomade dans le menu [Groupage](../fonctionnalites-mobile/tracabilite-i-groupage-degroupage.md) sous Traçabilité.
{% endhint %}

**Zone Groupe**

| Elément                            | Description                                                      |
| ---------------------------------- | ---------------------------------------------------------------- |
| **Groupe**                         | Nom du groupe                                                    |
| **Nature**                         | Nature du groupe (même choix de natures que pour les UL)         |
| **Nombre d'UL**                    | Nombre d'UL contenu dans le groupe                               |
| **Mouvementé la dernière fois le** | Date et heure du dernier mouvement connu du groupe               |
| **sur l'emplacement**              | Dernier emplacement connu du groupe                              |
| **par**                            | Opérateur ayant réalisé le dernier mouvement connu sur le groupe |

**Etiquettes unités logistiques**

Les étiquettes d'UL se positionnent dans la zone Groupe.

{% embed url="https://www.screencast.com/t/MqJzQBhO" %}
Étiquette UL dans zone groupe
{% endembed %}

| Elément              | Description                |
| -------------------- | -------------------------- |
| **Unité logistique** | Numéro d'UL                |
| **Quantité**         | Quantité contenu dans l'UL |
| **Nature**           | Nature de l'UL             |

Il y aura autant d'étiquette unité logistique que d'UL contenus dans le groupe.

#### Modifier un groupe

Pour modifier un groupe, cliquez sur les<img src="../../.gitbook/assets/3-points.png" alt="" data-size="line">dans la zone du colis et cliquez sur <mark style="background-color:blue;">**Modifier**</mark>.

Une modale quasi semblable à celle de modification d'UL s'ouvrira alors :&#x20;

* **Numéro groupe** : numéro du groupe. Ce champs n'est pas modifiable
* **Nature\*** : champ obligatoire pour la modification. Vous pouvez venir attribuer ainsi une nature au groupe
* **Nombre d'UL** : nombre d'unité logistique contenu dans le groupe. Ce champ n'est pas modifiable
* **Poids (kg) :** poids du groupe, champ modifiable
* **Volume (m3) :** volume du groupe, champ modifiable
* **Commentaire** : vous pouvez ajouter un commentaire sur le groupe

N'oubliez pas d'appuyez sur le bouton <mark style="background-color:blue;">**Enregistrer**</mark> pour valider vos modifications.

#### Dégrouper un groupe

Pour dégrouper un groupe, c'est-à-dire signifier que les unités logistiques contenus dans le groupe sont enlevés du groupe, cliquez sur les<img src="../../.gitbook/assets/3-points.png" alt="" data-size="line">de la zone du groupe et sur le bouton <mark style="background-color:blue;">**Dégrouper**</mark>.

Une première modale demande dans un premier temps de renseigner l'emplacement sur lequel les UL seront déposés suite au dégroupage.

Validez ensuite le dégroupage en cliquant sur <mark style="background-color:blue;">**Dégrouper**</mark>. Les étiquettes d'unité logistique disparaitront de la zone Groupe. Chaque UL aura un mouvement de dégroupage et de dépose sur l'emplacement renseigné de généré.&#x20;

&#x20;
