---
description: >-
  Planifier des missions d'inventaire, suivre leur avancement et corriger les
  écarts de stock.
---

# Inventaires

**Chemin :** Stock › Inventaire

Une **mission d'inventaire** liste les références, les articles ou les emplacements à compter. Les opérateurs font les comptages sur le nomade (voir [Inventaire nomade](../../fonctionnalites-mobile/stock-i-inventaire.md)), et cette page suit l'avancement.

{% hint style="info" %}
Des missions peuvent aussi être générées automatiquement, selon la **catégorie d'inventaire** des références. Voir [Paramétrage › Stock › Inventaires](../../parametrage/inventaires.md).
{% endhint %}

## Créer une mission

{% stepper %}
{% step %}
### Ouvrir le formulaire

Cliquez sur **Ajouter une mission**.
{% endstep %}

{% step %}
### Renseigner la mission

* **Libellé** : nom affiché sur le terminal.
* **Date prévue de début** et **Date prévue de fin** : la mission apparaît sur le terminal pendant cette période.
* **Description**.
* **Type de mission** :
  * **Mission quantité article** (Art/Ref) : comptage de références et d'articles ;
  * **Article sur emplacement** (Emplacement) : comptage par emplacement, **avec des étiquettes RFID**.
* **Créé par** : vous, par défaut.

Cliquez sur **Enregistrer**.
{% endstep %}

{% step %}
### Ajouter ce qu'il faut compter (mission Art/Ref)

Ouvrez la mission, puis :

* **Ajouter des emplacements** : toutes les références et tous les articles de ces emplacements sont ajoutés ;
* **Ajouter des références ou des articles** : saisissez les codes-barres séparés par des virgules (ex. : `REF230500000014, ART230500000090`).
{% endstep %}
{% endstepper %}

{% hint style="warning" %}
Une référence ou un article déjà présent dans une mission en cours ne peut pas être ajouté à une autre.
{% endhint %}

## Suivre une mission

**Dans la liste** : la colonne **Taux d'avancement** progresse à chaque comptage. Filtres : dates **Du** / **Au** et **Type** (Art/Ref ou Emplacement).

**Dans le détail d'une mission Art/Ref** : deux tableaux, **Liste des articles** et **Liste des références**. Au fil des comptages, la **date de saisie**, la **quantité comptée** et l'**anomalie** (Oui / Non) se remplissent. Le filtre **Anomalies** affiche les lignes en écart, et la flèche à côté de **Ajouter des références ou des articles** donne accès à **Exporter au format CSV**.

**Dans le détail d'une mission Emplacement** : la liste des zones et des emplacements, avec la date de scan, l'opérateur et le pourcentage scanné.

Le menu **⋮** d'une mission propose **Dupliquer** (pour la reprogrammer) et **Supprimer**.

## Écarts et mouvements de stock

Quand l'opérateur trouve un écart, le nomade lui demande de recompter :

* si l'écart est confirmé, la quantité en stock est corrigée ;
* sinon, l'anomalie disparaît.

Les écarts peuvent aussi se traiter sur le web, dans [Anomalies](anomalies.md). Chaque correction crée un mouvement de stock **entrée inventaire** (quantité comptée supérieure) ou **sortie inventaire** (quantité comptée inférieure). La **date de dernier inventaire** de la référence ou de l'article est mise à jour.

## Pages liées

La flèche à côté de **Ajouter une mission** donne accès à :

* **Voir les saisies** : tous les comptages réalisés, voir [Saisies d'inventaire](saisies-dinventaire.md) ;
* **Gérer les anomalies** : les écarts à traiter, voir [Anomalies](anomalies.md).
