# Tournée

**Chemin :** Demande › Tournée · création avec le bouton **+** du bandeau, puis **Tournée**

Une demande de tournée donne à un opérateur un ordre de passage sur des emplacements définis à l'avance. Sur chaque emplacement, il peut prendre ou déposer des UL, ou faire un passage à vide.

Les tournées peuvent être créées à la main ou automatiquement, à partir du [Planificateur de tournées](../../parametrage/tournees/planificateur-de-tournees.md) (tournées récurrentes).

## Créer une demande de tournée

1. Cliquez sur le bouton **+** du bandeau, puis sur **Tournée**.
2. Renseignez le **Type** et le **Statut** (obligatoires), puis si besoin la **Date attendue**, l'**Emplacement de la tournée**, l'**Urgence**, un commentaire et des pièces jointes.
3. Cliquez sur **Enregistrer**.

<figure><img src="https://806097355-files.gitbook.io/~/files/v0/b/gitbook-x-prod.appspot.com/o/spaces%2Fid6mpmGgIXZ3CFWUO3AX%2Fuploads%2FSmNfknnoGnKsHwsFLX9M%2FCapture%20d%E2%80%99e%CC%81cran%202025-11-26%20a%CC%80%2016.13.51.png?alt=media&#x26;token=6a665b57-cd6a-4552-ae0b-6c8e8dc60781" alt=""><figcaption></figcaption></figure>

{% hint style="info" %}
Les statuts proposés dépendent du type choisi. Ils se paramètrent dans **Paramétrages › Trace › Tournées**.
{% endhint %}

## Déroulement d'une tournée

L'opérateur fait la tournée sur le nomade : voir [Tournée (nomade)](../../fonctionnalites-mobile/tracabilite/tournee.md). Pendant ce temps, la page web montre l'avancement en direct.

{% file src="../../../.gitbook/assets/Vidéo Tournée.mov" %}

## Le détail d'une tournée

Cliquez sur une ligne de la liste pour ouvrir le détail.

| Bloc                         | Contenu                                                                                                                                                                                                                      |
| ---------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **Tournée**                  | Avancement des statuts, ainsi que les pièces jointes et commentaires ajoutés sur le nomade. Le menu ⋮ permet de **Modifier**, de **Supprimer** ou de **Terminer la tournée**.                                                |
| **Chemin opérateur**         | Emplacements prévus pour le type de tournée, avec le nombre d'UL prises ou déposées sur chacun. Depuis le web, vous pouvez aussi **Ajouter un emplacement**, enregistrer un **Nouveau mouvement** ou **Déclarer un litige**. |
| **Historique**               | Actions de l'opérateur : date, heure, emplacement, quantité. Les emplacements ajoutés en cours de tournée y figurent.                                                                                                        |
| **Informations**             | Dates de création, de démarrage et de traitement, et emplacement de la tournée.                                                                                                                                              |
| **Liste des ULs en encours** | UL présentes sur l'emplacement de la tournée. Cet emplacement doit être vide pour pouvoir terminer la tournée.                                                                                                               |

<figure><img src="https://806097355-files.gitbook.io/~/files/v0/b/gitbook-x-prod.appspot.com/o/spaces%2Fid6mpmGgIXZ3CFWUO3AX%2Fuploads%2Fejr0iScUNb3AyRxmpgiU%2FCapture%20d%E2%80%99e%CC%81cran%202026-02-18%20a%CC%80%2016.42.22.png?alt=media&#x26;token=a104ed14-dfb4-425c-a378-777f9126d6d7" alt=""><figcaption></figcaption></figure>

{% hint style="info" %}
Toutes les actions et tous les mouvements sont archivés dans **Traçabilité › Mouvements**.
{% endhint %}

## Retrouver une tournée

* **Filtres** : **Du** / **Au** (la flèche permet de choisir la date de création, la date attendue ou la date de traitement), **Statuts** (À faire, En cours, Pause, Terminée), **Type**, **Emplacement de la tournée** (par exemple chariot\_01).
* La flèche à côté de **Exporter au format CSV** donne accès à **Gestion des colonnes**.
* Le menu **⋮** d'une ligne propose **Modifier** et **Supprimer**.

| Colonne                                                         | Description                                                                            |
| --------------------------------------------------------------- | -------------------------------------------------------------------------------------- |
| **Numéro**                                                      | Préfixe TO suivi de l'année, du mois, du jour, de l'heure et de la minute de création. |
| **Date de création**, **Date attendue**, **Date de traitement** | Création de la demande, démarrage prévu, fin de la tournée.                            |
| **Statut**, **Type**                                            | Statut et type de la demande.                                                          |
| **Traité par**, **Demandeur**                                   | Opérateur qui a fait la tournée, et auteur de la demande.                              |
| **Urgence**                                                     | Urgence éventuelle et délai associé.                                                   |
| **Commentaire**                                                 | Commentaire de la demande.                                                             |
| **Emplacement de la tournée**                                   | Emplacement de l'opérateur pendant la tournée.                                         |

## Litiges sur tournée

Un litige peut être déclaré pendant une tournée, sur le nomade ou depuis le détail sur le web. Les types et statuts de litige se paramètrent dans **Paramétrages › Trace › Tournées** ([Litiges - Types](../../parametrage/tournees/litiges-types.md), [Litiges - Statuts](../../parametrage/tournees/litiges-statuts.md)).

## Autre utilisation

{% embed url="https://youtu.be/AD_YqqyXbZ4" %}
