---
description: >-
  Signaler à un acheteur les références à commander, suivre la commande et créer
  automatiquement la réception.
---

# Achats

**Chemin :** Demande › Achat · création avec le bouton **+** du bandeau, puis **Achat**

Une demande d'achat signale à un acheteur des références à commander. Elle suit un parcours de statuts que vous paramétrez : **Brouillon** → **À traiter** → **En cours** → **Traité**. À la fin, elle peut créer automatiquement une réception.

{% hint style="info" %}
Avant la première demande, paramétrez vos statuts dans [Paramétrage › Stock › Demandes › Achats › Statuts](../../parametrage/demandes/achats/statuts.md).
{% endhint %}

## Créer une demande d'achat

{% stepper %}
{% step %}
### Créer l'entête

Cliquez sur le bouton **+** du bandeau, puis sur **Achat**. Renseignez le **Demandeur** et le **Statut** (obligatoires), et si besoin le **Fournisseur**, les **Frais de livraison**, un **Commentaire** et des **Pièces jointes**. Cliquez sur **Enregistrer**.
{% endstep %}

{% step %}
### Ajouter les références

Sur la fiche de la demande, cliquez sur **Ajouter référence**. Choisissez la **Référence** et la **Quantité demandée** ; le libellé, la quantité en stock et l'acheteur s'affichent. Pour une référence gérée à l'article qui a des règles de stockage, vous pouvez aussi choisir un **Emplacement**.

{% hint style="warning" %}
Toutes les références d'une demande doivent avoir **le même acheteur**. L'acheteur de la demande est celui de la première référence ajoutée.
{% endhint %}
{% endstep %}

{% step %}
### Valider

Cliquez sur **Valider**, puis choisissez un statut à l'état **À traiter**. L'acheteur peut être prévenu par mail, selon le paramétrage du statut.
{% endstep %}
{% endstepper %}

Vous pouvez aussi créer des demandes d'achat depuis le [panier](../panier.md) : une demande est créée par acheteur.

## Faire avancer la demande

| Étape                    | Qui        | Action                                                                                                                                                                  |
| ------------------------ | ---------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **À traiter → En cours** | L'acheteur | Cliquez sur **Prendre en compte** et choisissez un statut à l'état En cours.                                                                                            |
| **Saisir la commande**   | L'acheteur | Cliquez sur chaque ligne de référence et renseignez la **Quantité commandée**, le **N° commande**, le **Fournisseur**, la **Date de commande** et la **Date attendue**. |
| **En cours → Traité**    | L'acheteur | Cliquez sur **Terminer la demande** et choisissez un statut à l'état Traité.                                                                                            |

{% hint style="info" %}
Si le statut final est paramétré pour **créer une réception**, les informations de commande doivent être renseignées sur chaque ligne. Ensuite, **Aller vers les réceptions** (sous la flèche) ouvre la ou les réceptions créées.
{% endhint %}

À chaque étape, **Modifier** (sous la flèche) permet de choisir un autre statut du même état, d'ajouter un commentaire ou une pièce jointe.

## Générer un bon de commande

Depuis la fiche d'une demande, le bouton **Générer bon de commande** produit un bon de commande à partir de votre modèle, paramétré dans [Modèles de document › Achats – Bon de commande](../../../parametrages/modeles-de-document.md#achats-bon-de-commande).

* La génération peut faire passer la demande au statut suivant : cochez l'option sur le statut, dans **Paramétrage › Stock › Demandes › Achats › Statuts**.
* Le rôle doit avoir le droit **Afficher achats**.

## Supprimer une demande

Sur la fiche, ouvrez la flèche et cliquez sur **Supprimer**, puis confirmez. Selon vos droits, la suppression est possible à tout moment.

## Retrouver une demande

* **Filtres** : dates **Du** / **Au**, **Statuts**, **Créé par**, **Acheteurs**, **Fournisseurs**.
* **Colonnes** : numéro, dates de création, de validation, de prise en compte et de traitement, demandeur, statut, acheteur, fournisseur, frais de livraison.
* Le bouton **Exporter au format CSV** exporte les demandes filtrées.
