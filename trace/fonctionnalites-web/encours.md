# Encours

La fonctionnalité des encours permet de visualiser la durée d'une unité logistique sur un emplacement. Les encours sont liés à des emplacements, qui sont eux-mêmes liés à des délais de traçabilité qu'il est possible de paramétrer dans le référentiel Emplacements.

Cette fonctionnalité est disponible dans l'onglet **Traçabilité**, puis **Encours**. Cette page contient plusieurs éléments :&#x20;

* Une **barre de filtre**, permettant de filtrer les données qui sont affichées dans le tableau
* Une indication de **dernière actualisation**
* Une **recherche rapide**, permettant également de filtrer les données affichées dans le tableau
* Un bouton <mark style="background-color:blue;">**Exporter au format CSV**</mark>, destiné à exporter l'ensemble des données filtrées du tableau sélectionné au format CSV
* Un bouton **Gestion des colonnes**, pour afficher ou masquer certaines colonnes.
* Un ou plusieurs **tableau(x)**, regroupant chacun les différentes unités logistiques présentes sur l'emplacement

{% hint style="info" %}
Le filtre **Emplacement** génère autant de tableaux que d'emplacements sélectionnés
{% endhint %}

### Contenu des filtres

| Filtre                                   | Description                                                                                                  |
| ---------------------------------------- | ------------------------------------------------------------------------------------------------------------ |
| **Emplacements**                         | Le(s) emplacement(s) à sélectionner pour lister les unités logistiques sur ce(s) dernier(s)                  |
| **Natures**                              | Le(s) nature(s) des unités logistiques à afficher dans le(s) tableau(x)                                      |
| **Prise en compte des arrivages camion** | Les éléments filtrés affiche un délai qui prend en compte le temps entre l'arrivage camion et l'arrivage UL. |

{% hint style="info" %}
Un emplacement au minimum est nécessaire afin d'afficher du contenu sur la page.
{% endhint %}

### Contenu du tableau

| Colonne              | Description                                                         |
| -------------------- | ------------------------------------------------------------------- |
| **Unité logistique** | Le numéro de l'unité logistique sur l'emplacement                   |
| **Date de dépose**   | La date de dépose de l'unité logistique sur l'emplacement           |
| **Délai**            | La durée totale de présence de l'unité logistique sur l'emplacement |
| **N° commande / BL** | Le numéro de commande de l'unité logistique lors de l'arrivage UL.  |
| **Issu de**          | Fonctionnalité qui a créé l'UL.                                     |
| **Référence**        | Nom de la référence si elle est manipulée comme une UL              |
| **Libellé**          | Libellé de la référence si elle est manipulée comme une UL          |

{% hint style="info" %}
Si une unité logistique déposé sur un emplacement d'encours dépasse le délais de traçabilité, la ligne correspondante sera surlignée en rouge.
{% endhint %}
