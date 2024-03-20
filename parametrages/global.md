---
description: >-
  Le paramétrage global regroupe tout ce qui peut être lié à des généralités sur
  l'application ou à une gestion du temps de travail
---

# Global

Ce paramétrage est ainsi structuré :

* Apparence du site
* Étiquettes
* Heures travaillées
* Jours non travaillés
* Serveur mail

### Apparence du site

Dans un premier temps, vous pouvez personnaliser les logos sur des différents documents et application, notamment celui de l'en-tête, des mail et sur le terminal mobile. Des logos de base vous sont proposés.

Dans un second temps, le choix de police vous est proposé, vous avez le choix entre Myriad (typo par défaut), Tahoma et Montserra.

Pour finir, vous pouvez déterminer le temps d'inactivité maximum en minutes avant que l'utilisateur ne soit déconnecté. (Le paramétrage ne prendra effet qu'à la prochaine connexion de l'utilisateur.)

### Étiquettes

La configuration des étiquettes est commune aux étiquettes d'article et d'arrivage. Ici, vous paramétrer le type les dimensions et le logo sur les étiquettes. Les paramètres spécifiques à l'étiquette d'article et d'arrivage se retrouvent respectivement dans le menu stock et trace.

**Le type d'étiquette** : Permet de spécifier le type de code barre généré sur les étiquettes, il y a 2 choix possibles : CODE128 \[1D] ou QR Code \[2D]

**Hauteur et largeur (mm)** : spécifie la hauteur et la largeur en millimètre de l'étiquette (entier)

**Logo sur l'étiquette** : Permet de charger une image de type .png ou .jpg qui sera superposée en haut à gauche de toutes les étiquettes générées.

### Heures travaillées

Le paramétrage des heures travaillées a une incidence sur le calcul des en-cours et du délai sur emplacement. En l'occurrence le délai positionné sur les emplacements sera en heures ouvrées en fonction de ces plages horaires.

Dans le tableau, vous retrouvez les jours de la semaine, les horaires de travail et si c'est un jour travaillé. Pour ajouter ou modifier les informations, cliquer sur la ligne que vous voulez modifier, une fois fini n'oubliez pas d'enregistrer.

**Horaires de travail** : 2 plages horaires sont à paramétrer par jour, 1 plage horaire le matin et 1 plage horaire l'après midi sous le format : HH:MM-HH:MM;HH:MM-HH:MM (exemple : 08:00-12:00;13:30-17:30)

**Travaillé** : la coche permet de d'activer ou de désactiver la journée

{% embed url="https://www.screencast.com/t/Gpn7BSO9AIJ" %}
Modification horaires de travail
{% endembed %}

**Créneaux horaires** : ce paramétrage à un impact sur les heures estimées des demandes de transport. Notamment pour les demandes de collecte, les créneaux horaires vont servir à renseigner un créneau de passage chez un client.

{% embed url="https://www.screencast.com/t/Ebf1eoyxcMX" %}
Création et modification des créneaux horaires
{% endembed %}

### Jours non travaillés

Le paramétrage des jours non travaillés a une incidence sur le calcul des en-cours et du délai sur emplacement.

Dans ce paramétrage indiquer les jours où votre entreprise ne travaille pas (exemple : jours fériés, vacances...). Vous pouvez facilement les supprimer en cliquant sur la corbeille au début de la ligne, et faire une recherche.

\
Pour ajouter des jours cliqué sur le bouton **Ajouter** et à l'aide d'un calendrier indiquer les jours qui vous conviennent. Pour en ajouter plusieurs à la fois appuyer sur la touche "Entrée" de votre clavier ou sur la ligne vide avec le plus, une fois fini n'oubliez pas d'**enregistrer**.

{% embed url="https://www.screencast.com/t/njGGDDfF33X7" %}
Ajouter des jours non travaillés
{% endembed %}

### Serveur mail

La configuration du serveur mail permet de renseigner les paramètres SMTP pour tous les envois des mails.

{% hint style="info" %}
Pour toutes les instances, merci de demander à Wiilog son paramétrage.
{% endhint %}

Le paramétrage comporte les champs suivants :

* Adresse du serveur SMTP
* Nom d'utilisateur
* Mot de passe
* Port => A préciser avec Wiilog si autre que 587 ou 25 pour ouverture du firewall sur l'infrasctructure
* Protocole
* Nom de l'expéditeur
* Adresse email de l'expéditeur

Une fois fini n'oubliez pas <mark style="background-color:blue;">d'</mark><mark style="background-color:blue;">**enregistrer**</mark>.
