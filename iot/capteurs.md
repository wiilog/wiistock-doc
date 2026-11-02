---
description: Provisionner et suivre les capteurs connectés.
---

# Capteurs

**Chemin :** IoT › Capteurs

{% hint style="info" %}
Un capteur doit d'abord être paramétré par Wiilog avant de pouvoir être ajouté dans FollowGT.
{% endhint %}

## Provisionner un capteur

{% stepper %}
{% step %}
### Choisir le capteur

Cliquez sur **Provisionner un capteur**, puis choisissez le capteur dans le champ **Code** : son type et son profil s'affichent.
{% endstep %}

{% step %}
### Le décrire

Renseignez le **Nom**, le **Gestionnaire** et, si besoin, les champs libres du type.
{% endstep %}

{% step %}
### Enregistrer

Cliquez sur **Enregistrer** : le capteur apparaît dans la liste.
{% endstep %}
{% endstepper %}

## Types de capteurs

| Type                                                            | Usage                                                                                                 |
| --------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------- |
| **Température**, **Hygrométrie**, **Température & Hygrométrie** | Suivi de la température et/ou de l'humidité. Des capteurs étalonnables sont disponibles sur commande. |
| **Action**                                                      | Bouton connecté qui déclenche une action (alerte ou demande).                                         |
| **GPS**                                                         | Suivi du trajet d'un véhicule (boîtier avec carte SIM branché sur la prise OBD).                      |
| **Tracer**, **Zone**, **Gateway**, **Extender**                 | Équipements de localisation et de réseau des objets connectés.                                        |

<figure><img src="https://806097355-files.gitbook.io/~/files/v0/b/gitbook-x-prod.appspot.com/o/spaces%2Fid6mpmGgIXZ3CFWUO3AX%2Fuploads%2FugJjg9oXsF0p6jVVX5DQ%2Fimage.png?alt=media&#x26;token=a2df5922-a6b5-4b33-b63a-ad46a4e0be06" alt="Trajet d&#x27;un véhicule suivi par capteur GPS"><figcaption><p>Trajet d'un véhicule suivi par capteur GPS</p></figcaption></figure>

## Actions sur un capteur

Menu **⋮** de la ligne :

* **Voir les messages** : toutes les remontées du capteur ;
* **Voir les éléments associés** : éléments associés, avec dates de début et de fin. Le **⋮** d'un élément donne accès à l'historique des données ;
* **Modifier** : nom, gestionnaire, seuil d'inactivité ;
* **Supprimer**.

<details>

<summary>Colonnes du tableau</summary>

| Colonne                                   | Description                                                                                    |
| ----------------------------------------- | ---------------------------------------------------------------------------------------------- |
| **Type** / **Profil**                     | Type de capteur et profil (selon le fabricant).                                                |
| **Nom** / **Code**                        | Nom unique donné au capteur, code non modifiable.                                              |
| **Adresse MAC Clover-Net**                | Adresse réseau du capteur, si concerné.                                                        |
| **Dernière remontée**                     | Date et heure du dernier message reçu.                                                         |
| **Niveau de batterie**                    | Batterie restante.                                                                             |
| **Gestionnaire**                          | Utilisateur prévenu par email si la batterie est faible ou si le capteur ne remonte plus rien. |
| **Seuil d'alerte d'inactivité (minutes)** | Durée sans message au-delà de laquelle le gestionnaire est alerté.                             |

</details>
