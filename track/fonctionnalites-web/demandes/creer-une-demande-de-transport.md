---
description: >-
  Créer une demande de livraison, de collecte ou de livraison/collecte à
  domicile.
---

# Créer une demande de transport

**Chemin :** **+** › Transport · ou Demande › Transport

## Demande de livraison

{% stepper %}
{% step %}
### Informations Patient

**Livraison** est sélectionné par défaut. Renseignez le **Patient\***, le **N° dossier\***, l'**Adresse\***, le **Contact\***, la **Personne à prévenir\*** et, si besoin, une **Remarque**.
{% endstep %}

{% step %}
### Service

Cliquez sur le type de livraison (voir [paramétrage](../../parametrage/demandes/livraison-types-and-champs-libres.md)) : les natures possibles pour ce service s'affichent. Activez **Faire une collecte en même temps que la livraison** pour une livraison/collecte (voir plus bas).
{% endstep %}

{% step %}
### Date

**Date et heure de livraison\*** et, si besoin, niveau d'**Urgence**.
{% endstep %}

{% step %}
### Unité logistique

Cochez les natures à livrer. Selon la nature, choisissez la température de conservation.

* UL déjà préparées : activez **Imprimer les étiquettes** pour indiquer le nombre d'UL par nature et imprimer les étiquettes tout de suite.
* UL pas encore préparées : laissez désactivé, vous imprimerez les étiquettes plus tard.
{% endstep %}

{% step %}
### Autres informations et enregistrement

Complétez les champs libres du type, puis cliquez sur **Enregistrer**.
{% endstep %}
{% endstepper %}

Selon la date choisie, un message peut s'afficher :

* **Livraison le jour même** : la demande est _en attente de validation_. Les destinataires paramétrés reçoivent un mail pour la valider ou la sous-traiter.
* **Horaire non travaillé** (ou date passée, si la livraison a été faite directement par un sous-traitant) : la demande n'a pas de suivi en temps réel. Le message se paramètre dans les [configurations](../../parametrage/demandes/configurations.md).

## Demande de collecte

Sélectionnez **Collecte** en haut du formulaire. Les étapes sont les mêmes, avec ces différences :

* **Date** : date indicative, à confirmer avec le patient. Pas d'heure ni d'urgence, pas de date passée.
* **Éléments à collecter** : cochez les natures. Un compteur permet d'indiquer la quantité si vous la connaissez, sinon laissez-le vide.

À l'enregistrement :

* **Collecte le jour même** : la demande est _en attente de validation_.
* **Collecte déjà en cours pour ce patient** (même n° de dossier) : un message vous demande de confirmer ou d'annuler.

## Livraison et collecte en même temps

1. Créez une demande de livraison et activez **Faire une collecte en même temps que la livraison**.
2. Cliquez sur **Enregistrer** : le formulaire de collecte s'ouvre avec les informations patient et la date de la livraison (non modifiables).
3. Complétez la collecte et cliquez sur **Enregistrer**.

{% hint style="info" %}
Vos demandes apparaissent ensuite dans **Demande › Transport**.
{% endhint %}
