# Actionneurs

Dans la page **IoT I Actionneurs**, vous retrouvez l'ensemble des capteurs qui sont associés à des modèles d'alertes ou actions. Vous pouvez utiliser les actionneurs pour les capteurs de type Température, Hygrométrie et Action.

Pour créer un nouvel actionneur, cliquez sur <mark style="background-color:blue;">**Nouvel actionneur**</mark>. Choisissez un capteur déjà provisionné via son nom ou son code.

### Pour les capteurs de température et hygrométrie

Renseignez une température dans le champ "**Si température supérieure à \_ °C**" et "**Si température inférieure à \_ °C**". Choisissez le type de modèle qui va se déclencher si ces limites sont atteintes, vous avez le choix entre Alerte ou Demande.&#x20;

* Les **alertes** sont paramétrable dans [paramétrage > Modèles de notification > Alertes](broken-reference), vous avez le choix entre créer une alerte mail, SMS ou web.
* Pour les **demandes**, vous avez 3 choix possibles de demande (vous pouvez créer des modèles qui se retrouveront ici) :&#x20;
  * Livraison : à paramétrer dans [Livraisons - Modèles de demande](../parametrages/stock/demandes/livraisons/modeles-de-demande.md)
  * Collecte : à paramétrer dans [Collectes - Modèle de demande](../parametrages/stock/demandes/collectes/modele-de-demande.md)
  * Services : à paramétrer dans [Services - Modèles de demande](../parametrages/trace/services/modeles-de-demande.md)

Cliquer sur <mark style="background-color:blue;">**Ajouter**</mark> pour enregistrer votre actionneur, il se retrouvera dans la liste.

{% hint style="warning" %}
La demande ou l'alerte ne se déclenchera pas à l'instant T où la température dépasse le seuil. Elle se déclenchera au moment où l'information est reçue.\
Si on veut que la demande ou l'alerte se déclenche à l'instant T, ce paramétrage doit être fait nativement sur le device par Wiilog.
{% endhint %}

{% embed url="https://www.screencast.com/t/h3eCphlgshg" %}

### Pour les capteurs d'action

Sélectionner sur le schéma quel bouton vous voulez paramétrer. Choisissez le type de modèle qui va se déclencher si ce bouton est actionné, vous avez le choix entre Alerte ou Demande.&#x20;

* Les **alertes** sont paramétrable dans [paramétrage > Modèles de notification > Alertes](../parametrages/iot/modeles-de-notifications/alertes.md), vous avez le choix entre créer une alerte mail, SMS ou web.
* Pour les **demandes**, vous avez 3 choix possibles de demande (vous pouvez créer des modèles qui se retrouveront ici) :&#x20;
  * Livraison : à paramétrer dans [Livraisons - Modèles de demande](../parametrages/stock/demandes/livraisons/modeles-de-demande.md)
  * Collecte : à paramétrer dans [Collectes - Modèle de demande](../parametrages/stock/demandes/collectes/modele-de-demande.md)
  * Services : à paramétrer dans [Services - Modèles de demande](../parametrages/trace/services/modeles-de-demande.md)

Cliquer sur <mark style="background-color:blue;">**Ajouter**</mark> pour enregistrer votre actionneur, il se retrouvera dans la liste.
