---
description: >-
  Signaler à l'avance une commande, une référence ou un fournisseur urgent pour
  être alerté dès sa réception.
---

# Urgences

**Chemin :** Traçabilité › Urgences

Une urgence prévient vos équipes dès qu'une marchandise attendue en priorité arrive. Il en existe deux familles, et le **type** choisi à la création détermine laquelle :

| Famille           | Se déclenche sur                                                             | Déclencheur                     | Paramétrage                                                        |
| ----------------- | ---------------------------------------------------------------------------- | ------------------------------- | ------------------------------------------------------------------ |
| **Urgence Trace** | un [arrivage UL](../trace/fonctionnalites-web/arrivages-unites-logistiques/) | le numéro de commande           | [Paramétrage › Trace › Urgences](../trace/parametrage/urgences/)   |
| **Urgence Stock** | une [réception](../stock/fonctionnalites-web/ordres/receptions/)             | une référence ou un fournisseur | [Paramétrage › Stock › Urgences](../stock/parametrage/urgences.md) |

## Créer une urgence Trace

1. Cliquez sur **Nouvelle urgence** et choisissez un **Type** d'urgence Trace.
2. Renseignez la **Date de début**, la **Date de fin** et le **N° de commande** (obligatoires).
3. Complétez si besoin : **N° poste**, **Acheteur**, **Fournisseur**, **Transporteur**, **N° tracking transporteur**, **Code article interne**, **Code article fournisseur** et les champs libres.
4. Cliquez sur **Enregistrer**.

{% hint style="info" %}
**Quand se déclenche-t-elle ?** Lorsqu'un arrivage UL est enregistré entre la date de début et la date de fin, et que ses informations (n° de commande, fournisseur, transporteur, acheteur) correspondent à celles de l'urgence.

Un message signale alors l'arrivage urgent, avec le n° de poste concerné. Les acheteurs reçoivent un mail.
{% endhint %}

## Créer une urgence Stock

1. Cliquez sur **Nouvelle urgence** et choisissez un **Type** d'urgence Stock.
2. Choisissez le **Déclencheur d'urgence** : **Référence** ou **Fournisseur**, puis sélectionnez la référence ou le fournisseur concerné.
3. Choisissez le **Critère de fin d'urgence** :
   * **Quantité restante** : l'urgence se termine quand la quantité attendue a été reçue ;
   * **Durée de validité** : l'urgence se termine à une date donnée ;
   * **Manuelle** : vous clôturez vous-même l'urgence.
4. Complétez si besoin : **N° de commande**, **Emplacement attendu de l'urgence**, **Transporteur**, **N° tracking transporteur**, commentaire, pièces jointes et champs libres.
5. Cliquez sur **Enregistrer**.

## Suivre les urgences

* **Filtres** : dates **Du** / **Au**, **Type**, **N° de commande**, **N° tracking transporteur**, **Transporteur**, **Statut** (Actives / Clôturées) et **Urgences appliquées à** (Trace / Stock).
* **Tableau** : en plus des informations saisies, vous y voyez la **date de clôture**, la **date du dernier déclenchement** et le **numéro du dernier arrivage ou de la dernière réception** concernée.
* La flèche à côté de **Nouvelle urgence** donne accès à **Exporter au format CSV** et à **Gestion des colonnes**.

## Agir sur une urgence

| Action                                                       | Où la trouver     | Résultat                                                 |
| ------------------------------------------------------------ | ----------------- | -------------------------------------------------------- |
| **Modifier**                                                 | Clic sur la ligne | Modifier les informations de l'urgence.                  |
| **Clôturer**                                                 | Menu **⋮**        | Terminer l'urgence.                                      |
| **Aller vers les arrivages** / **Aller vers les réceptions** | Menu **⋮**        | Ouvrir les arrivages ou les réceptions liés à l'urgence. |
