---
description: >-
  Notifications reçues sur le terminal mobile quand une demande ou un ordre est
  à traiter.
---

# Notifications push

**Chemin :** Paramétrage › Notifications › Notifications push

Une notification arrive sur le terminal mobile quand une demande est validée (passage de _Brouillon_ à _À traiter_). En appuyant dessus, l'opérateur ouvre directement la demande. Les demandes urgentes ont une indication visuelle en plus.

{% stepper %}
{% step %}
### Activer les notifications sur les types

Dans le paramétrage des types (livraisons, collectes, transferts, services, acheminements), cliquez sur **Modifier** puis activez **Notifications push**. Pour les livraisons, collectes et transferts, cela vaut pour la demande et pour l'ordre qui en découle.

Pour les **acheminements** et les **services**, trois choix : **Désactiver**, **Activer**, ou **Activer seulement si urgence** (en choisissant les valeurs d'urgence concernées).
{% endstep %}

{% step %}
### Donner le droit aux utilisateurs

Dans [Rôles](../utilisateurs/roles/), menu **Nomade**, activez le droit **Activer les notifications**. Vérifiez aussi que l'utilisateur a bien les types concernés dans ses champs **Type de livraison**, **Type d'acheminement** et **Types de service**.

{% hint style="info" %}
L'utilisateur doit se déconnecter puis se reconnecter au nomade pour que les changements soient pris en compte.
{% endhint %}
{% endstep %}

{% step %}
### Personnaliser le texte

Dans **Notifications push**, cliquez sur la ligne d'une demande ou d'un ordre pour modifier son texte. Les variables disponibles sont proposées, et une zone d'exemple montre le rendu (qui peut varier selon le terminal).
{% endstep %}
{% endstepper %}

<details>

<summary>Variables disponibles</summary>

{% tabs %}
{% tab title="Préparation / Livraison" %}
`@numordrepreparation` ou `@numordrelivraison`, `@typelivraison`, `@destination`, `@demandeur`, `@datevalidation`
{% endtab %}

{% tab title="Collecte" %}
`@numordrecollecte`, `@typecollecte`, `@destination` (mise en stock ou destruction), `@demandeur`, `@pointdecollecte`, `@objet`, `@datevalidation`
{% endtab %}

{% tab title="Transfert" %}
`@numordretransfert`, `@origine`, `@destination`, `@demandeur`, `@datevalidation`
{% endtab %}

{% tab title="Acheminement" %}
`@numacheminement`, `@typeacheminement`, `@statut`, `@empprise`, `@empdepose`, `@demandeur`, `@datevalidation`, `@dateecheance`, `@numcommande`, `@nbcolis`
{% endtab %}

{% tab title="Service" %}
`@numservice`, `@typeservice`, `@statut`, `@chargement`, `@dechargement`, `@demandeur`, `@datecreation`, `@dateattendue`, `@objet`, `@nboperations`
{% endtab %}
{% endtabs %}

</details>
