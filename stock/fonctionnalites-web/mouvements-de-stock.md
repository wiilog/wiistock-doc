---
description: >-
  Consulter toutes les entrées, sorties et transferts de stock, et enregistrer
  un mouvement manuel.
---

# Mouvements de stock

**Chemin :** Stock › Mouvements de stock

Chaque fois qu'une quantité entre, sort ou change d'emplacement dans le stock, Follow GT enregistre un **mouvement de stock**. Ces mouvements viennent des réceptions, préparations, livraisons, collectes, transferts, imports et inventaires. Vous pouvez aussi en créer un à la main.

| Type de mouvement                             | Effet sur le stock                              |
| --------------------------------------------- | ----------------------------------------------- |
| **Entrée**                                    | Augmente la quantité en stock.                  |
| **Sortie**                                    | Diminue la quantité en stock.                   |
| **Transfert**                                 | Change l'emplacement, sans changer la quantité. |
| **Entrée inventaire** / **Sortie inventaire** | Corrige la quantité après un inventaire.        |

<figure><img src="../../.gitbook/assets/Capture d’écran 2025-08-14 à 09.30.51.png" alt=""><figcaption></figcaption></figure>

## Créer un mouvement manuel

{% stepper %}
{% step %}
### Ouvrir le formulaire

Cliquez sur **Nouveau mouvement**. Le champ **Créé par** est prérempli avec votre nom.
{% endstep %}

{% step %}
### Choisir la référence

Sélectionnez la **Référence**. Le libellé et le code-barre se remplissent automatiquement. Pour une référence gérée à l'article, choisissez aussi le **Code barre article** concerné.
{% endstep %}

{% step %}
### Choisir le type et la quantité

Choisissez le **Type** :

* **Entrée** ou **Sortie** : saisissez la quantité à ajouter ou à retirer ;
* **Transfert** : choisissez l'emplacement de destination. Pour une référence gérée à la référence, toute sa quantité est transférée ; pour un article, seul cet article est déplacé.

La **quantité disponible** s'affiche pour vous aider. Ajoutez si besoin un **Commentaire**.
{% endstep %}

{% step %}
### Enregistrer

Cliquez sur **Enregistrer** : le mouvement apparaît en haut du tableau.
{% endstep %}
{% endstepper %}

{% hint style="warning" %}
Un transfert est impossible si la référence se trouve dans une demande de livraison, de collecte ou de transfert en cours.
{% endhint %}

## Retrouver ou supprimer un mouvement

* **Filtres** : dates **Du** / **Au**, **Emplacements** (d'origine ou de destination), **Type**, **Créé par**.
* La flèche à côté de **Nouveau mouvement** donne accès à **Exporter au format CSV** et à **Gestion des colonnes**.
* Un mouvement ne se modifie pas. Pour le **supprimer**, utilisez le menu **⋮** de la ligne. C'est impossible s'il est lié à des mouvements de traçabilité.

{% hint style="info" %}
Supprimer un mouvement de stock ne modifie pas la quantité en stock de la référence.
{% endhint %}

<details>

<summary>Colonnes disponibles</summary>

| Colonne                               | Description                                                                                                                                |
| ------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------ |
| **Date**                              | Date du mouvement.                                                                                                                         |
| **Issu de**                           | Élément à l'origine du mouvement (réception, préparation, livraison, collecte, transfert, import, inventaire). La plupart sont cliquables. |
| **Code barre**, **Référence article** | Article ou référence concerné.                                                                                                             |
| **Quantité**                          | Quantité déplacée.                                                                                                                         |
| **Origine**, **Destination**          | Emplacements de départ et d'arrivée, selon le type.                                                                                        |
| **Type**                              | Type du mouvement.                                                                                                                         |
| **Créé par**                          | Personne à l'origine du mouvement.                                                                                                         |
| **Prix unitaire**                     | Prix, s'il est renseigné.                                                                                                                  |
| **Commentaire**                       | Commentaire saisi sur le mouvement.                                                                                                        |

</details>
