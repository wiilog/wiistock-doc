---
description: >-
  Suivre les alertes de stock (seuils et péremption) et prévenir automatiquement
  les gestionnaires.
---

# Alertes

**Chemin :** Stock › Alertes

Cette page liste les références qui demandent votre attention. Il existe trois types d'alerte :

| Type d'alerte         | Se déclenche quand…                                                                  |
| --------------------- | ------------------------------------------------------------------------------------ |
| **Seuil d'alerte**    | La quantité de la référence passe sous son seuil d'alerte.                           |
| **Seuil de sécurité** | La quantité passe sous son seuil de sécurité, plus bas que le seuil d'alerte.        |
| **Péremption**        | La date de péremption d'un article est dépassée, ou le sera dans le délai paramétré. |

Les seuils se règlent sur chaque [référence](references.md), et le délai de péremption dans [Paramétrage › Stock › Alertes](../parametrage/alertes.md).

## Utiliser la page

* **Filtres** : dates **Du** / **Au**, **Type** de référence, **Alerte** (type d'alerte), **Gestionnaires**.
* **Couleurs de ligne** : elles indiquent si la référence est déjà dans une demande d'achat ou attendue sur une réception.
* **Icône panier** : ajoute la référence au [panier](panier.md), par exemple pour la commander.
* Le menu **⋮** propose **Aller sur la référence**.
* Le bouton **Exporter au format CSV** exporte les alertes filtrées.

<details>

<summary>Colonnes du tableau</summary>

Type d'alerte, Date d'alerte, Libellé, Référence, Code barre, Quantité disponible, Type quantité (gestion à la référence ou à l'article), Seuil d'alerte, Seuil de sécurité, Date de péremption, Gestionnaire(s).

</details>

## Les mails d'alerte

Si l'envoi est activé dans [Paramétrage › Stock › Alertes](../parametrage/alertes.md), les gestionnaires de la référence reçoivent un mail.

**Mail de seuil** : il reprend la référence, son mode de gestion, les quantités (disponible, réservée, en stock), les seuils, les champs libres et la liste des fournisseurs. Le bouton **Demander un devis** prépare un mail au fournisseur, prérempli avec les informations de la référence et l'adresse du fournisseur (issue du référentiel [Fournisseurs](../../referentiel/fournisseurs.md)).

![Exemple de mail d'alerte de seuil](<../../.gitbook/assets/Seuil de sécurité.PNG>)

**Mail de péremption** : il part un nombre de jours paramétré avant la date de péremption de l'article.

![Mail d'alerte de péremption](<../../.gitbook/assets/seuil péremption.PNG>)
