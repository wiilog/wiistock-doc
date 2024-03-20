---
description: 'Mise en production du 31/07/2023 - Version 6.36.6 #RFID'
---

# Mise à jour - Evolution sur les réserves de l'arrivage camion, les IoT,  et autres

## Evolution des réserves de l'arrivage camion (WEB & NOMADE)

* **Paramétrage | Trace | Arrivage camion :** Nouvelle page de paramétrage des réserves sur numéro de tracking.
  * Possibilité d'associer des libellés de réserve sur numéro de tracking avec des utilisateurs et leurs boite mail pour envoi d'email automatique dès déclenchement d'une réserve.&#x20;
  * Les pièces jointes et photo de la réserve détectée sur WEB ou NOMADE seront en pj du mail.&#x20;
* **Dashboard | Composant "Entrées à effectuer" :**&#x20;
  * Nouvelle case à cocher pour prise en compte du temps de l'arrivage camion dans le délai de traitement de l'UL.&#x20;
  * Possibilité d'ajouter plus de colonnes au composant.&#x20;
* **Entrepôt de données :**&#x20;
  * Ajout de la colonne "Réserve sur numéro de tracking" dans la table "Arrivage\_camion"
  * Ajout de la colonne "Numéro de tracking" dans la table "Arrivage\_camion"
* **Traçabilité | Arrivage camion :**
  * Nouvelle colonne "Réserve sur numéro de tracking" avec la liste des réserves identifiés sur les numéros de tracking de l'arrivage.
  * Ajout de la colonne "Réserve sur numéro de tracking" en gestion des colonnes.&#x20;
  * Possibilité de mettre un type de réserve différent sur les numéros de tracking d'un arrivage camion.&#x20;



## Evolution des demandes d'acheminements

* **Paramétrage | Trace | Acheminements | Types et champs libres** :&#x20;
  * Nouveaux champs Emplacement(s) de prise et Emplacement(s) de dépose suggéré(s).
* **Demande | Acheminement | Détail** :&#x20;
  * Modification d'une UL dans une demande au statut brouillon, nouveaux champs Nature UL, Poids UL, Volume UL, Commentaire UL.



## IoT : Mise en place du type de capteur "Température & Hygrométrie" (WEB)&#x20;

* **IOT | Capteurs | Provisionner un capteur** :&#x20;
  * Nouveau type de capteur " Température & hygrométrie".
* **IOT | Capteurs | Voir les messages** :&#x20;
  * Nouvelle colonne "Type de donnée" avec une ligne par message.&#x20;
* **IOT | Actionneurs | Nouvel actionneur** :&#x20;
  * Ajout des seuils hygrométrie pour un capteur de type "Température & Hygrométrie".
* **IOT | Associations**&#x20;
  * Nouveau filtre "Température & hygrométrie"
  * Nouveau filtre "Hygrométrie"
* **IOT | Associations | Détails**
  * Nouvelle courbe Hygrométrie avec échelle opposée à la courbe Température.

## Dashboard (WEB)

* **Dashboard** : Au clic du composant "Acheminement à traiter" redirection dans **Demande | Acheminement**. Liste des demandes filtrer en fonction du statut et du type paramétrer dans le composant.

## Urgence sur référence (WEB)

* **Stock | Article de référence** : Nouveau champ Quantité d'urgence, affichage sous condition de la coche Urgence. Se décrémente suite aux ordres de réception.
* **Stock | Article de référence** : Augmentation de la longueur du champ Commentaire d'urgence
* **Ordre | Réception | Détail** : Si la quantité réceptionnée est inférieure à la Quantité d'urgence de la référence, la coche Urgence est préservée et la Quantité d'urgence est mise à jour.
* **Mail | Article urgent réception** : Nouvelle ligne "Nombre d'article(s) restant(s) à recevoir "
