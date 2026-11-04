---
description: Déclencher une alerte ou une demande à partir d'un capteur.
---

# Actionneurs

**Chemin :** IoT › Actionneurs

Un actionneur relie un capteur (Température, Hygrométrie ou Action) à un modèle d'**alerte** ou de **demande** qui se déclenche automatiquement.

## Créer un actionneur

Cliquez sur **Nouvel actionneur**, puis choisissez un capteur déjà provisionné (par son **nom** ou son **code**).

{% tabs %}
{% tab title="Température / hygrométrie" %}
Renseignez les seuils **Si température supérieure à … °C** et/ou **inférieure à … °C**, puis le modèle déclenché si un seuil est franchi.
{% endtab %}

{% tab title="Bouton (Action)" %}
Sur le schéma, sélectionnez le bouton à paramétrer, puis le modèle déclenché quand il est actionné.
{% endtab %}
{% endtabs %}

Types de modèle possibles :

* **Alerte** (email, SMS ou notification push/web) : voir [Alertes](../parametrages/notifications/alertes.md) ;
* **Demande** : [livraison](../stock/parametrage/demandes/livraisons/modeles-de-demande.md), [collecte](../stock/parametrage/demandes/collectes/modele-de-demande.md) ou [service](../trace/parametrage/services/modeles-de-demande.md), à partir d'un modèle de demande.

Cliquez sur **Ajouter** : l'actionneur apparaît dans la liste (nom du capteur, modèle, type de modèle, type de seuil, date du dernier déclenchement).

{% hint style="warning" %}
L'alerte ou la demande se déclenche quand l'information est **reçue**, pas à l'instant exact où le seuil est franchi.
{% endhint %}
