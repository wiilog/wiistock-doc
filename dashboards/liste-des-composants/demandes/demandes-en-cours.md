# Demandes en cours

Ce composant présente sous forme d'une étiquette par demande, les demandes qui sont en brouillon ou en cours avec une visiblement sur l'état de chaque demande.&#x20;

Les paramétrages suivant sont disponibles :&#x20;

* **Demande\*** : champ obligatoire. Pour sélectionner quelle entité de demande il faut afficher sur le composant. Selon l'entité choisie, les informations sur chaque vignette ne seront pas les mêmes
* **Afficher** : sur ce champ vous avez 2 possibilités :&#x20;
  * **seulement les demandes de l'utilisateur en cours** : si vous choisissez cette possibilité, lorsqu'un utilisateur se connecter à l'application et arrive sur le dashboard qui contient ce composant, il ne verra que les demandes en brouillon ou en cours dont il est le demandeur.
  * **toutes les demandes** : l'utilisateur verra toutes les demandes en brouillon ou en cours de tous les demandeurs confondus.&#x20;

Ce composant possède également un élément de personnalisation propre à lui :&#x20;

* **Couleur fond étiquette** : contrairement à _Couleur fond composant_ qui viendra coloré toute la cellule derrière chaque étiquette, ce paramétrage sert à choisir la couleur de fond de chaque étiquette qui représente une demande. Attention, si vous mettez une couleur, vous n'aurez plus la distinction entre les demandes encore en brouillon et les autres

{% hint style="info" %}
Sur le dashboard, si la couleur de fond étiquette n'a pas été modifiée, les demandes en brouillon auront un fond gris.
{% endhint %}

Chaque étiquette est cliquable et permet d'accéder à :&#x20;

* la liste des ordres de livraison associés à la demande pour les livraisons,&#x20;
* le détail de l'ordre de collecte lié à la demande pour les collectes
* le détail de la demande de service pour les services
* le détail de la demande d'acheminement pour les acheminements
* le détail de la demande de transfert pour les transferts

Sur chaque étiquette vous avez comme informations :&#x20;

* En haut à gauche : date et heure d'estimation du traitement de la demande. Cette estimation se base sur la moyenne du temps de traitement pour ce type de demande ajoutée à la date de création de la demande
* plus bas : barre de progression de la demande avec le statut en cours de la demande en dessous
* au milieu : nombre d'articles contenus dans la demande pour les livraisons, collectes et transferts, objet de la demande pour les services, et nombre de colis dans la demande pour les acheminements, suivi du type de la demande (sauf pour les transferts)
* au milieu, après le logo localisation : emplacement de livraison, ou de transfert final ou de collecte, ou de dépose
* en bas à gauche, première ligne : numéro de la demande
* en bas à gauche, deuxième ligne : date et heure de création de la demande
* en bas à droite : demandeur

{% embed url="https://www.screencast.com/t/r0jQLk1X" %}
