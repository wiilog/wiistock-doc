---
description: Exporter des données une fois, ou automatiquement par email ou SFTP.
---

# Export CSV

**Chemin :** Paramétrage › Données › Exports CSV

La plupart des listes ont leur propre bouton **Exporter au format CSV**. Cette page permet en plus de lancer des exports complets, **uniques** ou **planifiés**, et d'en suivre l'historique.

## Créer un export

{% stepper %}
{% step %}
### Choisir le mode

Cliquez sur **Ajouter un export**, puis **Export CSV unique** ou **Export CSV planifié**.
{% endstep %}

{% step %}
### Choisir les données

**Type de données à exporter** : Références, Articles, Tournées, Arrivages, Référence emplacement, Acheminements, Productions, Mouvements, Unités logistiques, Arrivages camion, Associations BR, Litiges, Urgences, Emplacements ou Contacts.
{% endstep %}

{% step %}
### Planifier (export planifié)

* **Fréquence** : une fois, chaque heure, chaque jour, chaque semaine ou chaque mois ;
* **Destination d'export** : **Envoi email** (utilisateurs FollowGT et/ou emails libres) ou **Envoi vers serveur SFTP** (serveur hôte, port, utilisateur, mot de passe, répertoire cible).
{% endstep %}
{% endstepper %}

{% hint style="info" %}
Les références et articles exportés sont seulement ceux des groupes de visibilité de l'utilisateur.
{% endhint %}

## Suivre les exports

Le tableau liste les exports (statut, dates de création, début et fin, prochaine exécution, fréquence, utilisateur, type, données exportées). Filtrez par dates, statut ou utilisateur.
