# Détails arrivage

En cliquant sur une ligne d'arrivage, vous arriverez sur le détail de l'arrivage.

Le détail de l'arrivage contient 3 zones :&#x20;

* L'**entête** de l'arrivage
* La **liste des colis**
* La [**liste des litiges**](litiges-qualite.md) (voir page suivante)

{% embed url="https://www.screencast.com/t/EuAzbQY33Gg" %}
Détails d'un arrivage
{% endembed %}

### Entête d'arrivage

L'entête d'arrivage contient tous les différents champs renseignés sur le formulaire de création de l'arrivage.&#x20;

Elle va contenir également la mention "Cet arrivage est à traiter en URGENCE." lorsque l'application a détecté que les éléments renseignés concordent avec ceux d'une urgence existante (Voir [Urgences](../urgences.md)). La ligne de l'arrivage sera rouge dans la liste des arrivages également.

Elle contient également les boutons suivants :&#x20;

* <mark style="background-color:blue;">**Modifier**</mark> : pour modifier les informations de l'arrivage
* <mark style="background-color:blue;">**Imprimer arrivage**</mark> : pour imprimer l'étiquette du numéro d'arrivage
* <mark style="background-color:blue;">**Acheminer**</mark> : pour transférer les colis de l'arrivage dans un acheminement
* <mark style="background-color:blue;">**Supprimer**</mark> : pour supprimer l'arrivage

### Liste des colis

La liste des colis contient :&#x20;

* La **recherche rapide** : pour chercher rapidement une unité logistique
* Un bouton <mark style="background-color:blue;">**Ajouter colis**</mark> : pour ajouter des unités logistiques dans l'arrivage si certaines ont été oublié sur le formulaire de création d'arrivage
* Un bouton <mark style="background-color:blue;">**Imprimer colis**</mark> : pour relancer l'impression des étiquettes des unités logistiques de l'arrivage
* Un **tableau**, regroupant les unités logistiques de l'arrivage :&#x20;

| Colonne                    | Description                                                        |
| -------------------------- | ------------------------------------------------------------------ |
| **nature**                 | nature de l'unité logistique                                       |
| **Code**                   | Code de l'unité logistique généré par Follow GT                    |
| **Date dernier mouvement** | Date et heure de dernier mouvement de l'unité de logistique        |
| **Dernier emplacement**    | Dernier emplacement où est passé l'unité logistique                |
| **Opérateur**              | Opérateur ayant réalisé le dernier mouvement de l'unité logistique |

Sur chaque ligne du tableau, les<img src="../../../.gitbook/assets/3points" alt="" data-size="line">donne accès à :&#x20;

* <mark style="background-color:blue;">**Imprimer**</mark> : pour lancer l'impression de l'étiquette de cette unité logistique.
* <mark style="background-color:blue;">**Modifier**</mark> : pour modifier et ajouter des informations sur l'unité logistique (possibilité de modifier la nature de colis, la quantité, le poids, le volume et le commentaire).
* <mark style="background-color:blue;">**Supprimer**</mark> : pour supprimer l'unité logistique. La suppression est possible seulement si tous les mouvements de traçabilité liés à cette unité logistique sont supprimés.

