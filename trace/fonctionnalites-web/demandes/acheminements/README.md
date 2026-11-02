---
description: >-
  Demander le déplacement d'unités logistiques (UL) d'un emplacement à un autre,
  hors stock, et suivre la demande jusqu'à son traitement.
---

# Acheminements

**Chemin :** Demande › Acheminement · création avec le bouton **+** du bandeau, puis **Acheminement**

Une demande d'acheminement sert à faire déplacer des UL d'un point A à un point B, par exemple d'un quai vers un laboratoire. Les opérateurs la traitent sur le nomade, et vous suivez son avancement statut par statut.

## Créer une demande d'acheminement

{% stepper %}
{% step %}
### Ouvrir le formulaire

Cliquez sur le bouton **+** du bandeau, puis sur **Acheminement**. Il n'y a pas de bouton de création sur la page de liste.

<figure><img src="../../../../.gitbook/assets/image (72).png" alt="Menu de création rapide"><figcaption></figcaption></figure>
{% endstep %}

{% step %}
### Renseigner la demande

Les champs obligatoires sont : **Type**, **Statut**, **Demandeur**, **Emplacement de prise** et **Emplacement de dépose**. Les statuts proposés dépendent du type choisi.

Selon votre paramétrage, d'autres champs peuvent apparaître (voir le détail ci-dessous).
{% endstep %}

{% step %}
### Enregistrer

Cliquez sur **Enregistrer**. Vous arrivez sur le détail de la demande, où vous pouvez ajouter les UL à acheminer puis valider la demande.
{% endstep %}
{% endstepper %}

{% hint style="info" %}
Vous pouvez aussi créer un acheminement depuis les [arrivages UL](../../arrivages-unites-logistiques/#acheminer-un-ou-plusieurs-arrivages), à partir des UL d'un ou plusieurs arrivages.
{% endhint %}

<details>

<summary>Champs du formulaire</summary>

Les champs affichés et obligatoires se règlent dans [Paramétrage › Trace › Acheminements](../../../parametrage/acheminements/).

| Champ                                                                            | À quoi il sert                                                       |
| -------------------------------------------------------------------------------- | -------------------------------------------------------------------- |
| **Type** \*, **Statut** \*                                                       | Le type détermine les statuts proposés et le parcours de la demande. |
| **Demandeur** \*                                                                 | Personne à l'origine de la demande.                                  |
| **Emplacement de prise** \*, **Emplacement de dépose** \*                        | Point de départ et point d'arrivée des UL.                           |
| **Destination**                                                                  | Destination finale, si elle diffère de l'emplacement de dépose.      |
| **Urgence**                                                                      | Niveau d'urgence de la demande.                                      |
| **Transporteur**, **N° tracking transporteur**                                   | Utiles quand l'acheminement passe par un transporteur.               |
| **Intervenant**                                                                  | Personne concernée par la demande.                                   |
| **N° commande**, **Numéro projet**, **Business unit**                            | Informations de rattachement.                                        |
| **Email(s)**                                                                     | Adresses à prévenir.                                                 |
| **Échéance Du / Au**                                                             | Période dans laquelle la demande doit être traitée.                  |
| **Client**, **Téléphone client**, **À l'attention de**, **Adresse de livraison** | Coordonnées du destinataire, notamment pour une livraison externe.   |
| **Champs libres**                                                                | Champs propres à votre activité, définis par type.                   |
| **Commentaire**, **Pièces jointes**                                              | Informations complémentaires.                                        |

</details>

## Le détail d'une demande

Cliquez sur une ligne de la liste pour ouvrir la demande. Vous y trouvez :

* à gauche : le numéro, le type, la **timeline des statuts** (avec la date et l'auteur de chaque changement), les pièces jointes et le commentaire ;
* à droite : le bloc **Informations**, qui reprend tous les champs de la demande ;
* en bas : la **Liste des UL**, avec pour chacune son emplacement et, si besoin, le détail de son contenu (référence, quantité, n° de lot, n° de série, poids, volume…).

Le menu **⋮** en haut à gauche regroupe les actions :

| Action                                                                                                                                          | Résultat                                                                                                                                      |
| ----------------------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------- |
| **Valider** / **Terminer** / **Retour au statut brouillon**                                                                                     | Faire avancer la demande. Les boutons proposés dépendent du statut.                                                                           |
| **Générer un bon de transport**, **bon de livraison**, **bon de surconsommation**, **lettre de voiture**, **étiquette**, **bon d'acheminement** | Produire les documents de l'acheminement. Les modèles se règlent dans [Modèles de document](../../../../parametrages/modeles-de-document.md). |
| **Modifier**                                                                                                                                    | Modifier la demande (sauf le type et le statut).                                                                                              |
| **Supprimer**                                                                                                                                   | Supprimer la demande après confirmation.                                                                                                      |

## Retrouver une demande

* **Filtres** : période (la flèche permet de choisir la date de **création**, de **validation**, de **traitement** ou d'**échéance**), **N° demande**, **Statut**, **Type**, **Emplacement de prise**, **Emplacement de dépose**, **Demandeurs**, **Transporteur**, **Urgences**, **Intervenant**, **N° commande**, **Destination**, **Business unit**, **Numéro projet**, **Unité(s) logistique(s)**.
* La flèche à côté de **Exporter au format CSV** donne accès à **Gestion des colonnes** et à **Signature groupée**. Voir [Traitement par signature groupée](traitement-par-signature-groupee.md).

<details>

<summary>Colonnes disponibles</summary>

N° demande, Date de création, Date de validation, Date de traitement, Date d'échéance, Type, Créé par, Intervenant, Transporteur, N° commande, Emplacement de prise, Emplacement de dépose, Destination, Nombre d'UL, Statut, Urgence, Traité par, et les champs libres.

</details>
