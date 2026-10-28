# Capteurs

{% hint style="info" %}
Un capteur doit d'abord être paramétré par Wiilog avant de pouvoir être ajouté dans Follow GT.
{% endhint %}

Les capteurs sont consultables dans le menu **IoT | Capteurs**. La page contient une recherche rapide, le bouton **Provisionner un capteur** et le tableau des capteurs de l'instance.

{% embed url="https://www.screencast.com/t/A2l5mOXmgRd" %}
Page capteurs
{% endembed %}

### Types de capteurs

| Type            | Usage                                                                                                                                       |
| --------------- | ------------------------------------------------------------------------------------------------------------------------------------------- |
| **Action**      | Capteur qui déclenche une action                                                                                                            |
| **Température** | Suivi de la température                                                                                                                     |
| **Hygrométrie** | Suivre l'humidité. Des capteurs température et hygrométrie **étalonnables** (Symes) sont disponibles sur commande.                          |
| **GPS**         | Suivre le trajet d'un véhicule. Le capteur, équipé d'une carte SIM, se branche sur la prise OBD du véhicule et remonte ses coordonnées GPS. |

<figure><img src="https://806097355-files.gitbook.io/~/files/v0/b/gitbook-x-prod.appspot.com/o/spaces%2Fid6mpmGgIXZ3CFWUO3AX%2Fuploads%2FugJjg9oXsF0p6jVVX5DQ%2Fimage.png?alt=media&#x26;token=a2df5922-a6b5-4b33-b63a-ad46a4e0be06" alt="Trajet d&#x27;un véhicule suivi par capteur GPS"><figcaption><p>Trajet d'un véhicule suivi par capteur GPS</p></figcaption></figure>

### Contenu du tableau

| Colonne                | Description                                                                                             |
| ---------------------- | ------------------------------------------------------------------------------------------------------- |
| **Type**               | Type de capteur (voir ci-dessus)                                                                        |
| **Profil**             | Dépend du type de capteur et du fabricant                                                               |
| **Nom**                | Nom unique donné au capteur                                                                             |
| **Code**               | Code du capteur (non modifiable)                                                                        |
| **Dernière remontée**  | Date et heure du dernier message reçu                                                                   |
| **Niveau de batterie** | Niveau de batterie du capteur                                                                           |
| **Gestionnaire**       | Utilisateur prévenu par email en cas de batterie faible ou d'absence de message depuis un certain temps |

Le menu ⋮ d'une ligne propose :

* **Voir les messages** : toutes les remontées d'information du capteur ;
* **Voir les objets associés** : éléments associés au capteur, avec dates de début et de fin d'association. Le menu ⋮ d'un objet donne accès à l'**historique des données** ;
* **Modifier** : nom ou gestionnaire ;
* **Supprimer**.

### Provisionner un capteur

1. Cliquez sur **Provisionner un capteur**.
2. Choisissez le capteur dans la liste du champ **Code** : son type et son profil s'affichent.
3. Renseignez le **Nom**, le **Gestionnaire** et, si besoin, les champs libres.
4. Cliquez sur **Enregistrer**.

{% embed url="https://www.screencast.com/t/S7ok9OPI6t" %}
