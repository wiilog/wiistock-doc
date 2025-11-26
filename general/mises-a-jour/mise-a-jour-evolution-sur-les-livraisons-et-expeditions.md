---
description: 29/05/2023
---

# Mise à jour - Evolution sur les Livraisons et Expéditions

## SORTIE MAGASIN

### Partie web &#x20;

* Paramétrage | Stock | Demandes | Livraisons  - Renommage du paramétrage « Réaliser une demande de livraison sans quantité en stock » par « Faire le contrôle de la quantité au lancement de préparation » - Nouveau paramétrage « Ne pas gérer les quantités en stock » - Nouveau paramétrage « La livraison est directement préparée à sa validation »&#x20;
* Paramétrage | Stock | Demandes | Livraisons | Champs Fixes : Nouveaux champs pour paramétrer par défaut la Destination, le Type et le Destinataire dans une demande de livraison. - Le paramétrage « Emplacement de livraison par défaut » a été déplacé par le champ Destination dans la page de Paramétrage | Stock | Demandes | Livraisons | Champs Fixes &#x20;
* Paramétrage | Stock | Demandes | Livraisons | Types et champs libres : Nouveau champ libre « Envoi d’un email au destinataire »&#x20;
* Paramétrage | Terminal mobile | Livraisons : Nouveaux paramétrages  - Paramétrage autoriser la dépose des articles sur un emplacement libre- Paramétrage « Afficher le code référence et le rendre scannable. Enlever le code article. »&#x20;
* Demande | Livraison : Au clic du +, création automatique d’une demande de livraison si tous les champs obligatoires par défaut sont saisis&#x20;
* Demande | Livraison | Détail | Ajouter référence via un datatable modifiable. Le nouveau champ Projet associé à une référence, est géré dans Paramétrage | Stock | Demandes | Livraisons | Champs Fixes, il est affiché sous condition en fonction du type de la référence. &#x20;
* Demande | Livraison | Liste : Nouveau filtre et nouvelle colonne Destinataire&#x20;

### Partie nomade &#x20;

* Nomade | Stock | Livraison : Application des nouveaux paramétrages de Paramétrage | Terminal mobile | Livraisons &#x20;

## EXPEDITIONS

**+ (**_**Demande**_**) | Expédition :**&#x20;

* Créer des demandes d'expédition : choisir un ou plusieurs demandeurs, un ou plusieurs numéros de téléphone, un numéro de commande client, des cases à cocher "Livraison à titre gracieux" et "Articles conformes", Des informations liées au destinataire depuis le référentiel Client (client, téléphone, adresse de livraison), des informations sur l'expédition (date de prise en charge souhaitée, transporteur, envoi national / international, payé ou dû et un champ commentaire final.<br>
* Remplir des demandes d'expédition : Ajouter des références déjà existantes ou créer de nouvelles références à intégrer dans la demande d'expédition, avec les quantités, les prix unitaires, le poids net.
* Planifier des demandes d'expédition (Colisage) : Intégrer le nombre de colis, le transporteur, le numéro de tracking, les références dans chaque colis et la date d'enlèvement.
* Clôturer des demandes d'expéditions : Bouton Expédier pour finaliser le flux de la demande d'expédition.

**Demande | Expédition :**&#x20;

* Visualiser toutes les demandes d'expéditions, les filtrer via les dates de création de la demande, date de prise en charge souhaitée, date de validation, date de planification, date d'enlèvement prévu, date d'expédition, demandeur, statut, numéro commande client ou transporteur.
* Exporter les demandes d'expéditions avec l'ensemble des détails contenus dans chaque demande (une ligne par référence dans chaque demande d'expédition).&#x20;
* Demande | Expédition | Détails : Nouvelle timeline de statut pour une demande d'expédition (Brouillon, A traiter, Planifiée, Expédiée) Un encart d'informations "Transport" :  le nombre de colis, le poids brut, la valeur totale des prix, le poids net total, le nom du transporteur et le numéro de tracking
* Exporter des demandes d'expédition
* Stock | Références | Créer un article de référence : Ajout section "Données sécurités"
* Référentiel | Clients : Nouveau champ textuel "Destinataire"
* Dashboard : Modification du compostant Demande à traité avec un compteur des demandes d'expéditions

**Paramétrage**

* Paramétrage | Stock | Demandes | Expéditions : Paramétrage des valeurs par défaut pour les champs obligatoires lors de la création d'une référence dans une demande d'expédition  Paramétrage des emplacements par défaut (emplacement d'expédition et quai d'expédition)Paramétrage des envois d'email au statut à traiter et passage au statut expédié
* Paramétrage | Utilisateurs | Rôle | Demande | Expéditions : nouvelle partie Expéditions avec les droits associés
* Paramétrage | Utilisateur | Langue : Nouvelles personnalisations pour les Expéditions
* Paramétrage | Modèles de document | Expédition : Nouveau modèle de document par défaut le Bordereau de livraison, possibilité de charger un modèle personnalisé, voir les variables disponibles

**Entrepôt de donnée :**

* Nouvelle table dw\_demande\_expedition Nouvelle colonne dans la table dw\_reference\_article avec les nouveaux champs
