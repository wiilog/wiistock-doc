---
description: >-
  Créer et gérer vos références (les produits que vous stockez), suivre leurs
  quantités et les ajouter au panier.
---

# Références

**Chemin :** Stock › Référence

Une **référence** décrit un produit que vous stockez : code, libellé, fournisseurs, quantités, seuils d'alerte. Sa quantité se gère de deux façons :

| Gestion quantité   | Principe                                                                                                           | Exemple                                                |
| ------------------ | ------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------ |
| **À la référence** | Toute la quantité est suivie globalement, sur un seul emplacement.                                                 | Des boîtes de gants rangées au même endroit.           |
| **À l'article**    | Chaque pièce ou conditionnement est un **article** unique, avec son emplacement, son lot ou sa date de péremption. | Des réactifs avec des dates de péremption différentes. |

## Retrouver une référence

* Cliquez sur **Ajouter un filtre**, choisissez le champ et la valeur, puis cliquez sur **Appliquer**. Le filtre s'affiche sous forme d'étiquette ; la croix le retire.
* Pour une recherche rapide, utilisez le champ **Rechercher**. Le choix des colonnes où elle cherche se fait dans **Recherche rapide**, via la flèche à côté de **Nouvel article de référence**.
* La même flèche donne accès à **Gestion des colonnes** (vous pouvez aussi réordonner les colonnes par glisser-déposer), à **Impression des étiquettes** (après une recherche) et à l'option **Références actives seulement**.

{% hint style="info" %}
Deux couleurs de ligne vous aident : **Demande d'achat en cours** (la référence est dans une demande d'achat non clôturée) et **En attente de réception** (des quantités sont attendues sur une réception).
{% endhint %}

## Créer une référence

{% stepper %}
{% step %}
### Ouvrir le formulaire

Cliquez sur **Nouvel article de référence**. Une page de création s'ouvre.
{% endstep %}

{% step %}
### Identifier la référence

Renseignez la **Référence** (code), le **Libellé**, le **Type** et le **Statut** : **Brouillon**, **Actif** ou **Inactif**. Vous pouvez aussi ajouter des images et cocher **Synchronisation nomade** pour pouvoir la demander hors ligne depuis le terminal.
{% endstep %}

{% step %}
### Choisir la gestion de quantité

Dans **Gestion quantité**, choisissez :

* **Référence** : renseignez l'**Emplacement** et la **Quantité** ;
* **Article** : choisissez la **Gestion de stock**, c'est-à-dire **FIFO** (le premier entré sort en premier) ou **FEFO** (le premier qui périme sort en premier).

Dans les deux cas, vous pouvez indiquer les **Gestionnaires**, l'**Acheteur**, le **Prix unitaire**, le **Seuil d'alerte** et le **Seuil de sécurité**.
{% endstep %}

{% step %}
### Ajouter au moins un fournisseur

Renseignez **Nom fournisseur**, **Code fournisseur**, **Ref article fournisseur** et **Libellé**. Cliquez sur **Ajouter un article fournisseur** pour en ajouter d'autres.
{% endstep %}

{% step %}
### Compléter et enregistrer

Complétez si besoin les autres blocs (voir ci-dessous), puis cliquez sur **Enregistrer**.
{% endstep %}
{% endstepper %}

{% hint style="warning" %}
**Référence en brouillon** : elle ne peut pas être utilisée tant qu'un valideur ne l'a pas passée en **Actif**. Les utilisateurs qui ont le droit _Valideur de références_ reçoivent un mail, puis le créateur est prévenu de la validation. Une référence sortie du statut Brouillon ne peut plus y revenir.
{% endhint %}

{% hint style="info" %}
**Référence en gestion quantité Référence, statut Actif et quantité supérieure à 0** : la création génère automatiquement un mouvement de stock d'entrée dans l'emplacement saisi et un mouvement de traçabilité de type _Dépose_ lié à ce mouvement de stock. Pour une référence créée en brouillon, ces mouvements sont générés lors de son passage en **Actif**.
{% endhint %}

<details>

<summary>Les autres blocs du formulaire</summary>

| Bloc                 | Champs                                                                                                                                                                                                                                                     |
| -------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **Informations**     | **Groupe de visibilité** (seuls les utilisateurs de ce groupe voient la référence, voir [Groupes de visibilité](../parametrage/groupes-de-visibilite.md)), **Code NDP**, **Pièces jointes**, **Nomenclature**.                                             |
| **Description**      | **Matériel hors format** (Oui / Non), **Code fabriquant**, **Poids**, **Longueur**, **Largeur**, **Hauteur**. Le **Volume** est calculé automatiquement.                                                                                                   |
| **Données sécurité** | **Marchandise dangereuse** (Oui / Non) et **Fiche** de sécurité. Si vous répondez **Oui**, le **Code ONU** et la **Classe produit** deviennent obligatoires.                                                                                               |
| **Inventaires**      | **Catégorie d'inventaire** : la référence (ou ses articles) sera ajoutée automatiquement aux missions d'inventaire selon la fréquence de la catégorie. Les missions sont générées chaque dimanche soir. Voir [Inventaires](../parametrage/inventaires.md). |
| **Champs libres**    | Ils dépendent du type choisi. Voir [Types & champs libres](../parametrage/articles/types-et-champs-libres.md).                                                                                                                                             |

</details>

{% hint style="info" %}
Pour signaler qu'une référence est attendue en urgence, créez une **urgence Stock** sur cette référence. Voir [Urgences](../../urgences/urgences.md).
{% endhint %}

## Le détail d'une référence

Cliquez sur une ligne pour ouvrir la fiche. En plus des informations saisies, vous y trouvez :

* la **quantité disponible** (non réservée par une demande de livraison ou de transfert) et la **quantité en stock** ;
* les dates de **création**, de **dernière modification**, de **dernière entrée** et de **dernière sortie** ;
* les **fournisseurs** et la **règle de stockage** (blocs repliables) ;
* la **Prévision stock** : l'évolution prévue de la quantité à 1, 3 ou 6 mois, selon les demandes et les réceptions en cours ;
* le bouton **Ajouter au panier**.

{% hint style="info" %}
**Règle de stockage** : en mode modification, **Ajouter une règle de stockage** permet de définir un **Emplacement**, une **Qté sécurité** et une **Qté conditionnement** pour la référence.
{% endhint %}

## Agir sur une référence

| Action                         | Où la trouver                                  | Résultat                                                                                                                                                                                          |
| ------------------------------ | ---------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **Modifier**                   | Menu **⋮** ou bouton **Modifier** de la fiche  | Modifier la référence. Avec un droit de modification partielle, seuls certains champs sont modifiables (image, libellé, pièces jointes, nomenclature, prix, seuils, fournisseurs, champs libres). |
| **Voir les mouvements**        | Menu **⋮**                                     | Liste des mouvements de stock de la référence.                                                                                                                                                    |
| **Voir les demandes d'achats** | Menu **⋮**                                     | Demandes d'achat qui contiennent la référence.                                                                                                                                                    |
| **Voir les articles**          | Menu **⋮**                                     | Articles de la référence (gestion à l'article).                                                                                                                                                   |
| **Supprimer**                  | Menu **⋮**                                     | Impossible si la référence est liée à un autre élément (mouvement, demande, réception…). Passez-la plutôt en **Inactif**.                                                                         |
| **Ajouter au panier**          | Icône panier de la ligne ou bouton de la fiche | Pour la demander en livraison, en collecte ou en achat. Voir [Panier](panier.md). Une référence inactive n'a pas de panier.                                                                       |

<details>

<summary>Colonnes disponibles</summary>

Image, Libellé, Référence, Code barre, Type, Statut, Quantité stock, Quantité disponible, Acheteur, Emplacement, Seuil de sécurité, Seuil d'alerte, Prix unitaire, Synchronisation nomade, Nom fournisseur, Code fournisseur, Dernier inventaire, Gestion de stock, Gestionnaire(s), Commentaire, Créée le / par, Dernière modification le / par, Dernière entrée le, Dernière sortie le, Groupe de visibilité, et les champs libres.

</details>
