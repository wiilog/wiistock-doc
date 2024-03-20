# Transferts

L'ordre de transfert est généré suite à la validation de la demande de transfert. L'ordre est ce qui sera traité, et son traitement passera la demande en traité

Cette fonctionnalité est disponible dans le menu **Ordre**, puis **Transferts**. Vous pouvez arriver aussi directement sur le détail d'un ordre de transfert à partir du détail d'une demande de transfert en cliquant sur la flèche à droite de l'entête puis sur **Aller vers l'ordre de transfert**. Cette page contient plusieurs éléments :&#x20;

* Une **barre de filtre**, permettant de filtrer les données qui sont affichées dans le tableau
* Une **recherche rapide**, permettant également de filtrer les données affichées dans le tableau
* Un bouton **Exporter au format CSV**, destiné à exporter l'ensemble des données filtrées (suivant les dates renseignées) au format CSV
* Un **tableau**, regroupant les différents ordres de transfert créées

### Contenu des filtres

| Filtre         | Description                                                                                        |
| -------------- | -------------------------------------------------------------------------------------------------- |
| **Du**         | La tranche basse filtrant sur la date de création de l'ordre de transfert                          |
| **Au**         | La tranche haute filtrant sur la date de création de l'ordre de transfert                          |
| **Statuts**    | Le(s) statut(s) des ordres de transfert à filtrer                                                  |
| **Demandeurs** | Pour filtrer sur la personne ayant créée la demande de transfert qui a généré l'ordre de transfert |
| **Opérateurs** | Pour filtrer sur la personne ayant traitée l'ordre de transfert                                    |

### Contenu du tableau

| Colonne                | Description                                                                                                                                                                                                                       |
| ---------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **Numéro**             | Numéro de l'ordre de transfert                                                                                                                                                                                                    |
| **Statut**             | <p>Statut de l'ordre de transfert. 2 statuts sont possibles pour un ordre de transfert : <br>- A traiter : les références / articles n'ont pas encore été déplacées<br>- Traité : les références / articles ont été déplacées</p> |
| **Demandeur**          | Personne ayant créée la demande de transfert ayant générée l'ordre de transfert                                                                                                                                                   |
| **Opérateur**          | Opérateur ayant traité l'ordre de transfert                                                                                                                                                                                       |
| **Origine**            | Emplacement d'origine du transfert                                                                                                                                                                                                |
| **Destination**        | Emplacement de destination sur lequel doivent être déposées les références / articles                                                                                                                                             |
| **Date de création**   | Date de création de l'ordre de transfert                                                                                                                                                                                          |
| **Date de traitement** | Date de traitement de l'ordre de transfert                                                                                                                                                                                        |

### Détails de l'ordre de transfert

L'ordre de transfert est constitué d'une entête et d'un tableau contenant la liste des références et articles à transférer.

L'entête est constituée des champs :&#x20;

* **Numéro** : numéro de l'ordre de transfert
* **Statut** : statut actuel de l'ordre de transfert
* **Demandeur** : personne ayant créée la demande ayant générée l'ordre de transfert
* **Opérateur** : opérateur ayant traité l'ordre de transfert. Le champ est donc rempli seulement si l'ordre de transfert est traité
* **Origine** : emplacement d'origine du transfert
* **Destination** : emplacement de destination sur lequel doivent être déposées les références / articles
* **Dépose réelle** : si le paramétrage _"Autoriser la dépose des articles sur un emplacement libre"_ est activé (Voir [Fonctionnalités mobiles > Paramétrage Terminal mobile](../../parametrage-terminal-mobile.md)), l'opérateur a la possibilité de déposer les articles sur un autre emplacement que celui renseigné dans Destination. Dans ce cas là, cet emplacement autre que celui de destination sera renseigné dans ce champ. Le champ est donc rempli seulement si l'ordre de transfert est traité
* **Date de création** : date de création de l'ordre de transfert
* **Date de transfert** : date à laquelle l'ordre de collecte a été transfert

Dans cette entête se trouve également les boutons :&#x20;

* **Transférer** : pour faire le transfert des articles / références. Ce bouton clôture le transfert.
* Sous la flèche :&#x20;
  * **Supprimer** : suppression de l'ordre de transfert . La demande passera alors en état Brouillon. Si l'ordre est déjà traité, la suppression ouvrira une modale où il faut sélectionner un emplacement où déposer les références/articles transférées, afin de ne pas perdre leur traçabilité. Si l'ordre n'est pas encore traité, une modale de confirmation s'ouvrira
  * **Aller vers la demande de transfert** : pour retourner sur le détail de la demande de transfert ayant générée l'ordre

Tableau de la liste des articles :&#x20;

| Colonne        | Description                                        |
| -------------- | -------------------------------------------------- |
| **Référence**  | Référence à transférer                             |
| **Code barre** | Code barre article ou de la référence à transférer |
| **Quantité**   | Quantité de la référence ou de l'article           |

Si vous cliquez sur une des lignes du tableau, vous ouvrirez la modale de détail d'un article ou de la référence.

### Traiter l'ordre de transfert

Il est possible de traiter l'ordre de transfert sur la supervision, ce que nous allons voir ici. Pour voir le traitement sur le terminal mobile, voir Stock > Fonctionnalités mobiles > Transfert.

Pour traiter l'ordre de transfert, cliquez sur **Transférer**. Le transfert se fera alors.

Suite à la validation du transfert, il va alors se passer :&#x20;

* L'**ordre de transfert** passe au statut _**Traité**_
* La **demande de transfert** passe au statut _**Traité**_
* Un **mouvement de transfert** est créé pour chaque référence/article de l'ordre de transfert allant de l'emplacement d'origine à l'emplacement de destination indiqué sur la demande de transfert
