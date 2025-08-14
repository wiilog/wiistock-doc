# Mouvements de traçabilité

Les mouvements de traçabilité permettent de connaitre l'emplacement d'une unité de manutention, et cela avant la mise en stock. Cette fonctionnalité permet de déplacer une ou plusieurs unités de manutention d'un **emplacement A** à un **emplacement B**, tout en conservant ses différentes informations associées. Il est possible d'utiliser cette fonctionnalité sur l'application web et l'application mobile.

Ces derniers sont consultables dans l'onglet **Traçabilité**, puis **Mouvements**. Cette page contient plusieurs éléments :&#x20;

* Une **barre de filtre**, permettant de filtrer les données qui sont affichées dans le tableau
* Une **recherche rapide**, permettant également de filtrer les données affichées dans le tableau
* Un bouton <mark style="background-color:blue;">**Nouveau mouvement**</mark>, destiné à la création d'un mouvement de traçabilité
* Un bouton <mark style="background-color:blue;">**Exporter au format CSV**</mark>, destiné à exporter l'ensemble des données filtrées (suivant les dates renseignées) au format CSV
* Un bouton <mark style="background-color:blue;">**Gestion des colonnes**</mark>, permettant de choisir les colonnes à afficher dans le tableau
* Un **tableau**, regroupant les différents mouvements de traçabilité créés

### Contenu des filtres

| Filtre                 | Description                                                    |
| ---------------------- | -------------------------------------------------------------- |
| **Du**                 | La tranche basse filtrant sur la date de création du mouvement |
| **Au**                 | La tranche haute filtrant sur la date de création du mouvement |
| **Unités logistiques** | Le numéro de l'unité logistique à filtrer                      |
| **Emplacement**        | L'emplacement à filtrer                                        |
| **Types**              | Le(s) type(s) à filtrer                                        |
| **Opérateurs**         | Le(s) opérateur(s) à filtrer                                   |

### Contenu du tableau

| Colonne                | Description                                             |
| ---------------------- | ------------------------------------------------------- |
| **Issu de**            | L'origine du mouvement                                  |
| **Date**               | La date du mouvement de traçabilité                     |
| **Unités logistiques** | L'unité logistique/article mouvementée                  |
| **Référence**          | La référence de l'article ou de la référence mouvementé |
| **Libellé**            | Le libellé de l'article ou de la référence mouvementé   |
| **Groupe**             | Le groupe associé à l'unité logistique                  |
| **Quantité**           | La quantité mouvementée                                 |
| **Emplacement**        | L'emplacement du mouvement                              |
| **Type**               | Le type du mouvement                                    |
| **Opérateur**          | L'opérateur ayant réalisé le mouvement                  |
| _**Champs libres**_    | Les différents champs libres du mouvement               |

### Créer un nouveau mouvement

Afin de créer un nouveau mouvement de traçabilité, il suffit cliquer sur le bouton <mark style="background-color:blue;">**Nouveau mouvement**</mark>. Une modale va alors s'ouvrir, permettant ainsi de renseigner plusieurs champs :&#x20;

* La **date** du mouvement, par défaut initialisée à la date et heure actuelle
* L'**opérateur** du mouvement, qui est lié au référentiel **Utilisateurs**
* L'**action** à réaliser, qui peut être de plusieurs types :&#x20;
  * Prise
  * Dépose
  * Prise(s) et dépose(s)
  * Groupage
  * Dégroupage
  * Passage à vide
* La **quantité** à mouvementer, par défaut initialisée à 1
* Le **commentaire**
* Les **pièces jointes**
* Les **champs libres** (possible de rendre obligatoire depuis les paramètres)

<figure><img src="../../.gitbook/assets/Capture d’écran 2025-08-14 à 12.20.51 (1).png" alt=""><figcaption></figcaption></figure>

{% hint style="info" %}
L'action conditionne l'affichage des autres champs du formulaire. Ainsi, sélectionner l'action **Prise(s) et dépose(s)** affichera les champs **Emplacement de prise**, **Unités logistiques** et **Emplacement de dépose**.
{% endhint %}

Lorsque tous les champs ont été renseignés, il suffit de cliquer sur le bouton <mark style="background-color:blue;">**Enregistrer**</mark>, ce qui créera le mouvement de traçabilité. Il sera possible de retrouver ce dernier dans le tableau présent sur la page.

### Modifier un mouvement

Si une erreur a été commise lors de la création du mouvement de traçabilité, il reste toujours la possibilité de le modifier. Pour se faire, il suffit simplement de cliquer sur la ligne dans le tableau. Une modale d'édition va s'ouvrir, permettant de modifier quelques champs. Néanmoins, il n'est pas possible de modifier les informations suivantes :&#x20;

* La **date**
* **L'opérateur**
* L'**unité logistique**
* **La quantité**
* **Pièce jointe**
* L'**action**
* L'**emplacement**

<figure><img src="../../.gitbook/assets/Capture d’écran 2025-08-14 à 13.47.48.png" alt=""><figcaption></figcaption></figure>

{% hint style="info" %}
Si vous activez le droit "Modifier l'ensemble de la modale mouvement" (dans Traçabilité>Mouvements) vous pourrez modifier tous les champs de la modale.
{% endhint %}

### Supprimer un mouvement

Il est également possible de supprimer un mouvement de traçabilité en cliquant sur les<img src="../../.gitbook/assets/3-points.png" alt="" data-size="line">à gauche d'une ligne, puis <mark style="background-color:blue;">**Supprimer**</mark>. Une modale de confirmation va apparaitre, nécessitant l'approbation de la suppression du mouvement. Lors du clic sur <mark style="background-color:blue;">**Supprimer**</mark>, le mouvement sera retiré du tableau.

### Visualiser un mouvement

Enfin, il y a également la possibilité de seulement visualiser un mouvement de traçabilité Pour se faire, il faut cliquer sur les<img src="../../.gitbook/assets/3-points.png" alt="" data-size="line">à gauche d'une ligne, puis <mark style="background-color:blue;">**Détails**</mark>. Les différentes caractéristiques du mouvement vont alors apparaitre dans une modale, sans possibilité de modification.

<figure><img src="../../.gitbook/assets/Capture d’écran 2025-08-14 à 13.52.23.png" alt=""><figcaption></figcaption></figure>
