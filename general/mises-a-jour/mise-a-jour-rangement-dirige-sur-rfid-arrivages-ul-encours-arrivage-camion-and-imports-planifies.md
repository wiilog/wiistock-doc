---
description: Mise en production du 20/12/2023
---

# Mise à jour - Rangement dirigé sur RFID - Arrivages UL - Encours arrivage camion & Imports planifiés

### Rangement dirigé sur nomade pour article RFID "Poka Yoke"

      _Ce projet est utilisé pour le rangement dirigé d'articles créées via RFID sur des emplacements gérées dans les règles de stockage de chaque référence. Lorsqu'une référence portera une règle de stockage, et si le paramétrage est activé, alors, lors de la création d'un article RFID depuis le nomade, l'opérateur devra forcément scanner l'emplacement de stockage correspondant à la référence pour valider la création de l'article RFID._&#x20;

* WEB - Paramétrages | Stock | Articles - Création nomade RFID :&#x20;
  *   Ajout d'une case à cocher "Activation du blocage de la dépose sur un des emplacements des règles de gestion de la référence".&#x20;


* NOMADE -  Stock | Créer article - Validation de l'article :&#x20;
  * Ajout d'une page de scan avec vérification de l'existence d'un emplacement dans les règles de stockage lié à la référence.&#x20;
    * Si scan d'un emplacement non indiqué comme règle de stockage, message d'erreur avec précision des emplacements de règles de stockage.&#x20;
    * Si scan d'un emplacement indiqué comme règle de stockage, alors création de l'article sur cet emplacement.&#x20;



### Changement de statut automatique sur Acheminement via génération de bon de surconsommation

Ce développement permet de paramétré les statuts qui sont à passé de façon automatique sur les demandes d'acheminemnets pour lesquelles un bon de surconsommation&#x20;

* WEB - Paramétrage | Trace | Acheminement - Changement paramétrage sur bon de surconsommation
  * &#x20;Le paramétrage sur le changement de statut automatique à la génération d'un bon de surconsommation est maintenant situé au niveau de la création des statuts des acheminements.
* La page "Paramétrage | Trace | Acheminement - Bon de surconsommation" a donc été supprimée.&#x20;
* Le logo du bon de surconsommation peut être choisi dans la page "Paramétrage | Trace | Acheminement - Configurations".



### Distinction des types d'arrivage UL

      _Ce projet est utilisé pour catégoriser des flux d'arrivages UL et de faciliter la distinction des flux sur les étiquettes d'unités logistiques via des icônes. Les opérateurs, en un coup d'œil, pourront connaître le flux de l'unité logistique devant eux._&#x20;

* WEB - Paramétrage | Trace | Arrivage UL - Types et champs libres :&#x20;
  * Ajout d'un bouton pour l'import d'icone sur type d'arrivage UL.
* WEB - Paramétrage | Trace | Arrivage UL - Etiquettes :&#x20;
  * Ajout d'une case à cocher "Afficher l'icone du type".
*   MAIL - Ajout du numéro de camion sur les mails de réserves sur numéro de tracking

    * Sur le mail de réserve d'un numéro de tracking, ajout du numéro de camion sur lequel la réserve a été identifiée.&#x20;



### Encours avec temps d'arrivage camion

      _Ce projet permet de challenger les temps de gestion des colis dès le process d'arrivage camion. Vos délais d'encours peuvent être enrichi avec le temps d'arrivage camion et suit donc l'ordre chronologique de vos arrivages camion et UL._&#x20;

* WEB - Traçabilité | Encours :&#x20;
  * Ajout d'une case à cocher "Prise en compte des arrivages camion" qui ajoute au délai sur emplacement de votre colis le délais entre l'arrivage camion et l'arrivage UL.&#x20;
  * Sur les tableaux, le tri des colonnes par défaut est sur le délai de façon descendante. (Du plus en retard au moins en retard).&#x20;
* WEB - Dashboard | Entrées à effectuer :&#x20;
  * Si vous avez coché les cases "Prendre en compte le temps d'arrivage camion" et "rediriger au clic sur la page d'encours", alors vous serez rediriger sur la page des Encours avec les filtres de la page préselectionnés.&#x20;



### Imports planifiés

      _Ce projet est utilisé pour importer des référentiels ou données de façons récurrentes en allant chercher dans un dossier sur un serveur les fichiers à récupérer ont été mis à jour. Vous pouvez donc importer tous les matins à 7h vos mises à jour d'utilisateurs, projets, emplacements, références, articles, etc. Cette fonctionnalité vous permettra un interfaçage de premier niveau avec votre ERP par exemple. En prérequis, pour utiliser cette fonctionnalité, il vous faudra les accès à un serveur ftp sur lequel les csv à importer seront déposés._&#x20;

* WEB - Paramétrage | Données | Imports et mises à jours - Ajouter un import :&#x20;
  * Nouveau bouton "Import planifié" qui affiche les données à remplir pour paramétrer le nouvel import planifié.&#x20;
  * Nouveau type d'import dans le tableau avec la fréquence d'exécution.&#x20;
    * Une ligne sera créée à l'ajout d'un import planifié puis une ligne à chaque occurrence d'import automatique créé.
