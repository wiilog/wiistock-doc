# Livraisons

L'ordre de livraison est généré suite à la validation de l'ordre de préparation. Une fois que l'ordre de livraison sera traité, il fera avancé le statut de la demande de livraison.

Cette fonctionnalité est disponible dans le menu <mark style="background-color:blue;">**Ordre**</mark>, puis <mark style="background-color:blue;">**Livraisons**</mark>. Vous pouvez arriver aussi directement sur le détail d'un ordre de livraison à partir du détail d'une demande de livraison ou d'un ordre de préparation en cliquant sur la flèche à droite de l'entête puis sur <mark style="background-color:blue;">**Aller vers l'ordre de livraison**</mark>. Cette page contient plusieurs éléments :&#x20;

* Une **barre de filtre**, permettant de filtrer les données qui sont affichées dans le tableau
* Une **recherche rapide**, permettant également de filtrer les données affichées dans le tableau
* Un bouton **Exporter au format CSV**, destiné à exporter l'ensemble des données filtrées (suivant les dates renseignées) au format CSV
* Un **tableau**, regroupant les différents ordres de livraison créés

### Contenu des filtres

| Filtre                 | Description                                                                                                                                                                                                                                                                                                |
| ---------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **Du**                 | La tranche basse filtrant sur la date de création de l'ordre de livraison                                                                                                                                                                                                                                  |
| **Au**                 | La tranche haute filtrant sur la date de création de l'ordre de livraison                                                                                                                                                                                                                                  |
| **Statuts**            | Le(s) statut(s) des ordres de livraison à filtrer                                                                                                                                                                                                                                                          |
| **Numéros de demande** | Pour filtrer sur les numéros de demande de livraison ayant générés les ordres                                                                                                                                                                                                                              |
| **Utilisateurs**       | Pour filtrer sur la personne ayant traitée l'ordre de livraisons. Vous pouvez renseigner plusieurs utilisateurs. Ce filtre va chercher dans la liste des utilisateurs renseignées dans l'application. Vous devez taper une première lettre pour avoir une suggestion d'utilisateurs contenant cette lettre |
| **Type**               | Le type des ordres de livraison à filtrer                                                                                                                                                                                                                                                                  |

### Contenu du tableau

| Colonne              | Description                                                                                        |
| -------------------- | -------------------------------------------------------------------------------------------------- |
| **Numéro**           | Numéro de l'ordre de livraison                                                                     |
| **Statut**           | Statut de l'ordre de livraison                                                                     |
| **Date de création** | Date de création de l'ordre de livraison                                                           |
| **Opérateur**        | Opérateur ayant traité l'ordre de livraison                                                        |
| **Type**             | Type de la demande de livraison ayant créée l'ordre de préparation qui a créé l'ordre de livraison |

### Détails de l'ordre de livraison

L'ordre de livraison est constituée d'une entête et d'un tableau contenant la liste des références à livrer.

L'entête est constituée des champs :&#x20;

* **Numéro** : numéro de l'ordre de livraison&#x20;
* **Statut** : statut actuel de l'ordre de livraison&#x20;
* **Opérateur** : opérateur ayant traité l'ordre de livraison . Le champ est donc rempli seulement si l'ordre de livraison est traité
* **Demandeur** : utilisateur ayant créé la demande de livraison ayant générée l'ordre de préparation qui a généré l'ordre de livraison
* **Point de livraison** : emplacement où livrer les références demandées
* **Date de livraison** : date de traitement de l'ordre de livraison. Ce champ est donc rempli quand l'ordre de livraison est traité

Dans cette entête se trouve également les boutons :&#x20;

* **Finir la livraison** : pour finir la livraison. Ce bouton clôture la livraison
* Sous la flèche :&#x20;
  * **Supprimer** : suppression de l'ordre de livraison. L'ordre de préparation passera alors en statut A traiter. La suppression ouvrira une modale où il faut sélectionner un emplacement où déposer les références/articles préparés sur la livraison, afin de ne pas perdre leur traçabilité
  * **Retourner à la demande de livraison** : pour aller sur la demande de livraison ayant générée l'ordre de préparation qui a généré l'ordre de livraison
  * **Retourner à la préparation** : pour aller sur l'ordre de préparation ayant générée l'ordre de livraison

Tableau de la liste des articles :&#x20;

| Colonne         | Description                                               |
| --------------- | --------------------------------------------------------- |
| **Référence**   | Référence à livrer                                        |
| **Libellé**     | Libellé de la référence à livrer                          |
| **Emplacement** | Emplacement où se situe la référence / l'article à livrer |
| **Quantité**    | Quantité de la référence à livrer                         |

Si vous cliquez sur la ligne du tableau, la modale de détail d'un article de référence ou de l'article (selon si la référence est en gestion quantité par référence ou par article) s'ouvre

### Traiter l'ordre de livraison

Il est possible de traiter l'ordre de livraison sur la supervision, ce que nous allons voir ici. Pour voir le traitement sur le terminal mobile, voir [Stock > Fonctionnalités mobiles > Livraison](../../fonctionnalites-mobile/stock-i-livraison.md).

Pour traiter l'ordre de livraison, cliquez sur <mark style="background-color:blue;">**Finir la livraison**</mark>.&#x20;

Suite à la validation de la livraison, il va alors se passer :&#x20;

* L'**ordre de livraison** passe au statut _**Livré**_, ou _**Partiellement livré**_ si l'ordre de livraison provient d'un ordre de préparation en _**Partiellement préparé**_
* La **demande de livraison** passe au statut _**Livré**_, ou _**Partiellement livré,**_ si toutes les préparations associés à la livraison ne sont pas terminées et livrées
* Un **mouvement de sortie** est créé pour chaque référence/article de l'ordre de livraison allant de l'emplacement de préparation de la référence ou de l'article, jusqu'à l'emplacement de livraison indiqué
