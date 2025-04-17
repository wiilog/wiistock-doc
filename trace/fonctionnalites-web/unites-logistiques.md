# Unités logistiques

La page des unités logistiques récapitule tous les UL créés sur l'application Wiilog, ainsi que les groupes d'UL.

Pour accéder à la page, vous devez aller dans le menu **Traçabilité**, puis choisir **Unités logistiques**.

La page des unités logistiques contient plusieurs éléments :&#x20;

* Une **barre de filtre**, permettant de filtrer les données qui sont affichées dans les tableaux
* Une **recherche rapide**, permettant également de filtrer les données affichées dans les colonnes du tableau
* Un bouton **Exporter au format CSV** destiné à exporter l'ensemble des données filtrées (suivant les dates renseignées) au format CSV
* Une **gestion des colonnes** pour afficher ou non les colonnes choisies.&#x20;
* Un bouton **"Loupe"** par UL pour visualiser l'historique des mouvements de l'unité logistique.&#x20;

### Contenu des filtres

Une fois que vous avez renseigné vos filtres, cliquez sur <mark style="background-color:blue;">**Filtrer**</mark>. Les filtres sont conservés d'une session à l'autre (ils seront toujours actifs si vous changez de page ou que vous vous déconnectez et reconnectez).

| Filtre                  | Description                                                                                                                                                                                                                                                           |
| ----------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **Du**                  | La tranche basse filtrant sur la date de dernier mouvement du colis                                                                                                                                                                                                   |
| **Au**                  | La tranche haute filtrant sur la date de dernier mouvement du colis                                                                                                                                                                                                   |
| **Unités logistiques**  | Tapez le numéro d'UL sur lequel vous souhaitez faire une recherche                                                                                                                                                                                                    |
| **Natures**             | Sélectionnez les natures d'UL sur lesquelles vous souhaitez filtrer la liste des unités logistiques                                                                                                                                                                   |
| **Emplacement**         | <p>Renseignez ici un emplacement pour voir tous les UL dont le dernier emplacement connu est cet emplacement<br><em><mark style="color:orange;">Attention, cela ne signifie pas que l'UL est à cet emplacement si son dernier mouvement est une prise</mark></em></p> |
| **n° d'arrivage**       | Tapez ici un numéro d'arrivage pour avoir tous les UL issus de cet arrivage                                                                                                                                                                                           |
| **Projet**              | Tapez le nom d'un projet provenant du référentiel Projet                                                                                                                                                                                                              |
| **Association**         | Tapez le nom d'un bon de réception associé à votre UL pour la retrouver.                                                                                                                                                                                              |
| **Type**                | Sélectionner si vous voulez voir des UL uniquement ou des groupes uniquement. Si vide, vous visulaiser les deux dans le même tableau.                                                                                                                                 |
| **Délai de traitement** | Case à cocher pour filtrer des UL uniquement avec des délais de traitement                                                                                                                                                                                            |

### Contenu du tableau

| Colonne                       | Description                                                                                                                                                                                                                                              |
| ----------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **Numéro UL**                 | Numéro du colis. Ce numéro peut être un numéro résultant de la création d'un arrivage, d'une unité de manutention ajoutée sur un acheminement, ou sur une prise/dépose, ou de la création d'une réception (numéro d'article ou de référence dans ce cas) |
| **Nature**                    | Nature associée au UL. Pour le cas des unités logistiques  résultants de réception, il n'y aura pas de nature d'UL                                                                                                                                       |
| **Quantité**                  | Quantité dans l'unité logistique                                                                                                                                                                                                                         |
| **Date du dernier mouvement** | Date et heure du dernier mouvement de l'UL                                                                                                                                                                                                               |
| **Issu de**                   | Lien vers l'arrivage, l'acheminement ou la réception dont est issu l'UL                                                                                                                                                                                  |
| **Emplacement**               | Dernier emplacement du dernier mouvement connu de l'UL                                                                                                                                                                                                   |
| **Arrivage camion**           | Numéro d'arrivage camion auquel l'UL est liée                                                                                                                                                                                                            |
| **Délai de traitement**       | Temps de traitement de l'UL (chrono spécifique)                                                                                                                                                                                                          |
| **Date limite de traitement** | Dernière date pour laquelle le traitement de l'UL sera valide (chrono spécifique)                                                                                                                                                                        |
| **Groupe rattaché**           | Si l'UL est dans un groupe, nom du groupe                                                                                                                                                                                                                |
| **Fournisseur**               | Fournisseur identifié lors de l'arrivage UL                                                                                                                                                                                                              |
| **N° commande / BL**          | N° commande identifié lors de l'arrivage UL                                                                                                                                                                                                              |
| **Projet**                    | Projet identifié lors de l'arrivage UL                                                                                                                                                                                                                   |
| **Transporteur**              | Transporteur identifié lors de l'arrivage UL ou arrivage camion.                                                                                                                                                                                         |
| **Association**               | Numéro d'association lié lors de l'association BR                                                                                                                                                                                                        |

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

Vous devez avoir au préalable supprimé tous les mouvements et éléments associés a l'UL avant de le supprimer. Si ce n'est pas le cas, vous obtiendrez un message d'erreur.

<figure><img src="../../.gitbook/assets/image (1).png" alt=""><figcaption></figcaption></figure>

