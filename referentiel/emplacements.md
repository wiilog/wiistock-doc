---
description: Emplacements, groupes d'emplacements et zones.
---

# Emplacements

**Chemin :** Référentiel › Emplacements

La page a 3 onglets :

* **Emplacements** : lieux de prise, de dépose ou de stockage ;
* **Groupes** : ensembles d'emplacements (dropzone d'un utilisateur, association à un capteur IoT) ;
* **Zones** : par défaut « Activité standard ». D'autres zones peuvent être créées, notamment pour les inventaires RFID (contactez Wiilog).

<figure><img src="../.gitbook/assets/image (172).png" alt=""><figcaption></figcaption></figure>

## Créer un emplacement

Cliquez sur **Nouvel Emplacement**. Les champs sont regroupés par thème :

| Section                               | Champs                                                                                                                                                                                                                                                                                    |
| ------------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **Général**                           | **Nom\*** (24 caractères maximum, unique, sans accent : lettres, chiffres, `_`, `/`, `-` et espace), **Description**, **Statut** (actif/inactif), **Zone\***, **Délai maximum de traçabilité HH:MM** (au-delà, l'UL apparaît en retard dans Traçabilité › Encours).                       |
| **Contraintes de dépose**             | **Natures autorisées** et **Températures autorisées** (vide = tout est autorisé), **Types de livraisons** et **Types de collectes autorisés** (l'emplacement est proposé comme destination ou point de collecte pour ces types).                                                          |
| **Encours visible sur nomade**        | À la prise sur cet emplacement, le nomade affiche toutes les UL présentes. À éviter sur les emplacements très chargés.                                                                                                                                                                    |
| **Acheminements - Signature groupée** | **Signataire(s)** et **Email** utilisés pour signer les acheminements.                                                                                                                                                                                                                    |
| **Traçabilité - emails**              | **Point de livraison** : mail au destinataire de l'arrivage quand ses UL sont déposées ici (et relances à 7, 15, 30 et 42 jours). **Emplacement de la tournée** : emplacement dédié aux tournées de traçabilité. **Envoi d'email à chaque dépose aux responsables** + **Responsable(s)**. |
| **Typologie d'emplacement**           | **Prise initiale** (démarre le chrono de l'UL), **Dépose finale** (l'arrête), **Pause** (le met en pause). **Changement de nature à la prise / à la dépose** : la nature de l'UL change automatiquement pour la nouvelle nature choisie.                                                  |

<figure><img src="../.gitbook/assets/Photo sélectionnée (1).jpg" alt=""><figcaption><p>Encours visible sur nomade, à la prise</p></figcaption></figure>

Cliquez sur **Enregistrer**.

## Actions

| Action                                                | Où                                                                                                                         |
| ----------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------- |
| **Modifier**                                          | Clic sur la ligne. Passez l'emplacement en **Inactif** s'il n'est plus utilisé mais ne peut pas être supprimé.             |
| **Imprimer** / **Supprimer**                          | Menu **⋮** de la ligne.                                                                                                    |
| **Imprimer les étiquettes**                           | Flèche à côté de **Nouvel Emplacement** : imprime les étiquettes des emplacements affichés (faites d'abord une recherche). |
| **Statut emplacement actif**                          | Même menu : n'affiche que les emplacements actifs.                                                                         |
| **Exporter au format CSV** / **Gestion des colonnes** | Même menu.                                                                                                                 |

## Groupes d'emplacements

Dans l'onglet **Groupes**, cliquez sur **Nouveau groupe** : **Nom du groupe\*** (différent de tout nom d'emplacement), **Description\***, **Statut\*** et **Emplacements\***.

Une icône wifi signale un groupe lié à un objet connecté : le menu **⋮** propose alors **Historique des données** (voir [IoT](../iot/capteurs.md)).

{% hint style="info" %}
Un emplacement ou un groupe déjà utilisé ne peut pas être supprimé : passez-le en inactif.
{% endhint %}
