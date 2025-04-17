---
description: >-
  Vous pouvez venir déclencher des mails, sms, ou notification web et push avec
  des objets connectés. Ce paramétrage sert à définir le contenu de ces alertes.
---

# Alertes

Pour visualiser les informations d'un modèle déjà existant sélectionner le via la liste déroulante sous "Nom du modèle", selon le type du modèle les informations seront différentes. Si vous souhaitez le modifier cliquer sur le bouton **Modifier.**

### Créer un modèle

Pour créer un modèle, cliquer sur le bouton **Ajouter un modèle d'alerte.** Ensuite sélectionner le type (notification Push/web, SMS ou Mail).

#### Notification Push/web

Les notifications déclenchées par les objets connectés apparaitront sur le nomade et la supervision en même temps pour tous les utilisateurs. Vous pouvez cliquer sur la notification de la supervision pour voir l'historique, cela revient aussi à cliquer sur la cloche dans l'entête. Les variables ne sont pas disponibles pour cette catégorie d'alerte.

{% hint style="info" %}
Sur la supervision, elles apparaîtront en haut droite de votre écran, pensez à activer les notifications sur Chrome.
{% endhint %}

| Champs                    | Description                                                                                                                                     |
| ------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------- |
| **Type d'alerte**         | Vous avez le choix entre les SMS, les mails ou les notifications push et web. Votre choix conditionnera les informations à remplir par le suite |
| **Nom du modèle**         | Donner un nom à ce modèle de notification pour le retrouver par la suite                                                                        |
| **Texte de notification** | Texte qui apparaîtra dans la notification                                                                                                       |
| **Image de notification** | Image/icône qui accompagnera le texte dans la notification                                                                                      |

#### SMS

Les notifications déclenchées par les objets connectés apparaitront sur le nomade en même temps pour tous les utilisateurs.

<table><thead><tr><th width="204.89452060193764">Champs</th><th>Description</th></tr></thead><tbody><tr><td><strong>Type d'alerte</strong></td><td>Choix du type que vous voulez, cela conditionnera les informations à remplir par le suite</td></tr><tr><td><strong>Nom du modèle</strong></td><td>Donner un nom à ce modèle de notification pour le retrouver par la suite</td></tr><tr><td><strong>Destinataire(s)</strong></td><td>Choisissez le bon indicatif pays et saisissez le numéro de téléphone du portable devant recevoir le sms d'alerte. Cliquez sur "<strong>Ajouter</strong> <strong>un destinataire</strong>" pour ajouter un autre numéro de téléphone.</td></tr><tr><td><strong>Sms</strong></td><td>Ecrivez le contenu du votre Sms. Vous pouvez y inclure des variables tel que le nom du capteur ayant déclenché l'alerte et la donnée qui a déclenché l'alerte. Pour le moment, cette donnée peut seulement être une donnée température.</td></tr></tbody></table>

#### Mail

<table><thead><tr><th width="199.0829487012462">Champs</th><th>Description</th></tr></thead><tbody><tr><td><strong>Type d'alerte</strong></td><td>Choix du type que vous voulez, cela conditionnera les informations à remplir par le suite</td></tr><tr><td><strong>Nom du modèle</strong></td><td>Donner un nom à ce modèle de notification pour le retrouver par la suite</td></tr><tr><td><strong>Destinataire(s)</strong></td><td>Saisissez la ou les adresse(s) mail des personnes qui vont recevoir cette notification</td></tr><tr><td><strong>Objet</strong></td><td>Renseignez l'objet du mail</td></tr><tr><td><strong>Image de début de mail</strong></td><td>Image/icône qui accompagnera le corps du mail</td></tr><tr><td><strong>Corps du mail</strong></td><td>Ecrivez le contenu du votre mail. Vous pouvez y inclure des variables tel que le nom du capteur ayant déclenché l'alerte et la donnée qui a déclenché l'alerte. Pour le moment, cette donnée peut seulement être une donnée température.</td></tr></tbody></table>

**Les variables :**

* `@nomcapteur` : Nom du capteur qui a déclenché l'alerte&#x20;
* `@codecapteur` : Code du capteur qui a déclenché l'alerte&#x20;
* `@datealerte` : Date et heure du déclenchement de l'alerte&#x20;
* `@data` : Fonctionne seulement pour un capteur de type température. La température ayant déclenché l'alerte sera alors la donnée remontée
