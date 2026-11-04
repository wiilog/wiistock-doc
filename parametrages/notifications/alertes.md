---
description: >-
  Contenu des emails, SMS et notifications push/web déclenchés par les objets
  connectés.
---

# Alertes

**Chemin :** Paramétrage › Notifications › Alertes

Pour voir un modèle, choisissez-le dans **Nom du modèle**, puis cliquez sur **Modifier** pour le changer. Pour en créer un, cliquez sur **Ajouter** et choisissez le **Type d'alerte\*** : **Email**, **SMS** ou **Notifications Push/Web**. Les modèles s'utilisent ensuite dans les [actionneurs](../../iot/actionneurs.md).

{% tabs %}
{% tab title="Email" %}
| Champ                      | Description                                |
| -------------------------- | ------------------------------------------ |
| **Nom du modèle**          | Pour retrouver le modèle.                  |
| **Destinataires**          | Adresses email, séparées par des virgules. |
| **Objet**                  | Objet du mail.                             |
| **Image de début de mail** | Image ou logo en tête du mail.             |
| **Corps de l'email**       | Texte, avec des variables si besoin.       |
{% endtab %}

{% tab title="SMS" %}
| Champ               | Description                                                                        |
| ------------------- | ---------------------------------------------------------------------------------- |
| **Nom du modèle**   | Pour retrouver le modèle.                                                          |
| **Destinataire(s)** | Indicatif pays et numéro de portable. **Ajouter un destinataire** pour en ajouter. |
| **SMS**             | Texte, avec des variables si besoin.                                               |
{% endtab %}

{% tab title="Notifications Push/Web" %}
| Champ                     | Description                       |
| ------------------------- | --------------------------------- |
| **Nom du modèle**         | Pour retrouver le modèle.         |
| **Texte de notification** | Texte affiché (pas de variables). |
| **Image de notification** | Icône qui accompagne le texte.    |

La notification s'affiche en même temps sur le nomade et sur le web pour tous les utilisateurs (cloche en haut de l'écran). Sur le web, pensez à autoriser les notifications dans Chrome.
{% endtab %}
{% endtabs %}

### Variables (email et SMS)

| Variable       | Valeur                                                    |
| -------------- | --------------------------------------------------------- |
| `@nomcapteur`  | Nom du capteur qui a déclenché l'alerte.                  |
| `@codecapteur` | Code du capteur.                                          |
| `@datealerte`  | Date et heure du déclenchement.                           |
| `@data`        | Donnée qui a déclenché l'alerte (température uniquement). |
