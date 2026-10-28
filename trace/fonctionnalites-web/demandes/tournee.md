# Tournée

Une demande de tournée attribue à un opérateur un ordre de passage sur des emplacements prédéfinis. Sur chaque emplacement, il peut prendre ou déposer des UL, ou faire un passage à vide.

Les tournées peuvent être créées à la main ou automatiquement, à partir du [Planificateur de tournées](../../parametrage/tournees/planificateur-de-tournees.md) (tournées récurrentes).

Accès : menu **Demande | Tournée**, ou bouton **+** puis **Tournée**.

### Liste des tournées

La page contient une barre de filtres, une recherche rapide, un export CSV et le tableau des demandes de tournée.

| Filtre                        | Description                                                       |
| ----------------------------- | ----------------------------------------------------------------- |
| **Du / Au**                   | Date de création de la demande                                    |
| **Statut**                    | Statut(s) de la demande                                           |
| **Type**                      | Type de tournée                                                   |
| **Emplacement de la tournée** | Emplacement de l'opérateur pendant la tournée (ex. : chariot\_01) |

| Colonne                                | Description                                                                           |
| -------------------------------------- | ------------------------------------------------------------------------------------- |
| **Numéro**                             | Préfixe TO suivi de l'année, du mois, du jour, de l'heure et de la minute de création |
| **Date de création**                   | Date de création de la demande                                                        |
| **Date et heure de démarrage attendu** | Moment où l'opérateur doit démarrer la tournée                                        |
| **Date de traitement**                 | Date et heure de fin de la tournée                                                    |
| **Statut**, **Type**                   | Statut et type de la demande                                                          |
| **Traité par**, **Demandeur**          | Opérateur ayant réalisé la tournée, et auteur de la demande                           |
| **Urgence**                            | Urgence éventuelle et délai associé                                                   |
| **Commentaire**                        | Commentaire de la demande                                                             |
| **Emplacement de la tournée**          | Emplacement de l'opérateur pendant la tournée                                         |

### Créer une demande de tournée

Cliquez sur **+** puis **Tournée**, et renseignez : type, statut, date et heure de démarrage attendu, emplacement de la tournée, urgence et champs libres.

<figure><img src="https://806097355-files.gitbook.io/~/files/v0/b/gitbook-x-prod.appspot.com/o/spaces%2Fid6mpmGgIXZ3CFWUO3AX%2Fuploads%2FSmNfknnoGnKsHwsFLX9M%2FCapture%20d%E2%80%99e%CC%81cran%202025-11-26%20a%CC%80%2016.13.51.png?alt=media&#x26;token=6a665b57-cd6a-4552-ae0b-6c8e8dc60781" alt=""><figcaption></figcaption></figure>

{% hint style="info" %}
Les statuts proposés dépendent du type choisi. Ils se paramètrent dans **Paramétrages | Trace | Tournées**.
{% endhint %}

### Déroulement d'une tournée

L'opérateur réalise la tournée sur le nomade : voir [Tournée (nomade)](../../fonctionnalites-mobile/tracabilite/tournee.md). Pendant ce temps, la page web suit l'avancement en direct.

{% file src="../../../.gitbook/assets/Vidéo Tournée.mov" %}

### Détail d'une tournée

Cliquez sur une ligne de la liste pour ouvrir le détail.

| Bloc                   | Contenu                                                                                                                                       |
| ---------------------- | --------------------------------------------------------------------------------------------------------------------------------------------- |
| **Tournée**            | Avancement des statuts, pièces jointes et commentaires ajoutés sur le nomade. Le menu ⋮ permet de modifier, supprimer ou terminer la tournée. |
| **Chemin opérateur**   | Emplacements paramétrés pour le type de tournée et nombre d'UL prises ou déposées sur chacun.                                                 |
| **Historique**         | Actions de l'opérateur : date, heure, emplacement, quantité. Les emplacements ajoutés en cours de tournée y apparaissent.                     |
| **Informations**       | Dates de création, de démarrage et de traitement, et emplacement de la tournée.                                                               |
| **UL sur emplacement** | UL présentes sur l'emplacement de la tournée. Il doit être vide pour pouvoir terminer la tournée.                                             |

<figure><img src="https://806097355-files.gitbook.io/~/files/v0/b/gitbook-x-prod.appspot.com/o/spaces%2Fid6mpmGgIXZ3CFWUO3AX%2Fuploads%2Fejr0iScUNb3AyRxmpgiU%2FCapture%20d%E2%80%99e%CC%81cran%202026-02-18%20a%CC%80%2016.42.22.png?alt=media&#x26;token=a104ed14-dfb4-425c-a378-777f9126d6d7" alt=""><figcaption></figcaption></figure>

{% hint style="info" %}
Toutes les actions et tous les mouvements sont archivés dans **Traçabilité | Mouvements**.
{% endhint %}

### Litiges sur tournée

Un litige peut être déclaré pendant une tournée. Les types et statuts de litiges se paramètrent dans **Paramétrages | Trace | Tournées** ([Litiges - Types](../../parametrage/tournees/litiges-types.md), [Litiges - Statuts](../../parametrage/tournees/litiges-statuts.md)).

### Autre utilisation

{% embed url="https://youtu.be/AD_YqqyXbZ4" %}
