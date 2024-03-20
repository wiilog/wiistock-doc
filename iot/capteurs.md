# Capteurs

{% hint style="info" %}
Afin d'ajouter un capteur dans Wiilog, il doit au préalable avoir été paramétré par notre service informatique.
{% endhint %}

Une fois le capteur paramétré par wiilog vous pouvez les provisionner, ces derniers sont consultables dans l'onglet **Iot**, puis **Capteurs**. Cette page contient plusieurs éléments :&#x20;

* Une **recherche rapide**, permettant de filtrer les données affichées dans le tableau
* Un bouton <mark style="background-color:blue;">**Provisionner un capteur**</mark>, pour ajouter un capteur
* Un **tableau**, regroupant l'ensemble des capteurs disponible sur une instance

{% embed url="https://www.screencast.com/t/A2l5mOXmgRd" %}
Page capteur
{% endembed %}

## Contenu tableau

<table><thead><tr><th width="258.5">Colonne</th><th>Description</th></tr></thead><tbody><tr><td><strong>Type</strong></td><td>Type de capteur : Action / Température / GPS </td></tr><tr><td><strong>Profil</strong></td><td>Le profil dépend du type du capteur et du device maker</td></tr><tr><td><strong>Nom</strong></td><td>Nom que vous donnez au capteur (il doit être unique)</td></tr><tr><td><strong>Code</strong></td><td>Code du capteur (non modifiable)</td></tr><tr><td><strong>Dernière remontée</strong></td><td>Date et heure de la dernière remontées d'information du capteur</td></tr><tr><td><strong>Niveau de batterie</strong></td><td>Information sur la baterie du capteur</td></tr><tr><td><strong>Gestionnaire</strong></td><td><p>Utilisateur de l'application, Envoi de mails à ce gestionnaire si :<br>• batterie faible</p><p>• pas d'envoi de message depuis x temps</p></td></tr></tbody></table>

Vous avez accès à plusieurs actions depuis les ![](<../.gitbook/assets/Capture d’écran 2023-02-06 à 12.07.16 (1).png>) d'une ligne de capteur :&#x20;

* **Voir les messages** : renvoi vers une nouvelle page pour consulter toutes les remonté d'information du capteur
* **Voir les objets associés** : Ensemble des éléments associés au capteur avec la date de début et de fin d'association
  * Depuis les ![](<../.gitbook/assets/Capture d’écran 2023-02-06 à 12.07.16 (1).png>) d'un objet vous pouvez voir **l'historique des données**
* **Modifier :** pour modifier le nom ou le gestionnaire d'un capteur
* **Supprimer :** pour supprimer un capteur de la liste

## Provisionner un capteur

Cliquer sur <mark style="background-color:blue;">**Provisionner un capteur**</mark>.  Une modale s'ouvre, cherchez votre capteur dans la liste déroulante du champ Code, les informations sur son type et profil s'affiche, ensuite renseignez son Nom, le Gestionnaire et si besoin un champ libre. <mark style="background-color:blue;">**Enregistrer**</mark>.

{% embed url="https://www.screencast.com/t/S7ok9OPI6t" %}
