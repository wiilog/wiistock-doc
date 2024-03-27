---
description: Mise en production du 27/03/2024
---

# Mises à jour - Collecte manuelle nomade, Encours de stock & évolution des demandes d'achats

### Collectes manuelles&#x20;

      _Ce projet permet d'entrer en stock rapidement des articles consommés. Vous devez sélectionner un type de collecte, puis scanner un emplacement de prise, scanner le code barre de l'article et enfin scanner l'emplacement sur lequel vous déposez l'article dans le stock. Des mouvements de stocks seront générés et votre article passera en "Disponible".  Si vous scanner un code barre de référence, un article sera créé automatiquement. Pour voir apparaitre cette fonctionnalité, pensez à activer le droit nomade "Collecte manuelles" sur votre rôle._&#x20;

* WEB | Paramétrages | Utilisateurs | Rôles - Nomade | Stock | Afficher les collectes manuelles
  * Nouvelle case à cocher pour le droit d'utilisation des collectes manuelles.&#x20;
* NOMADE | Stock | Collectes manuelles&#x20;
  * Nouveau menu Collectes manuelles
* WEB | Demande | Collecte
  * Génération de demande de collecte au statut "Collecté"
* WEB | Ordre | Collecte&#x20;
  * Génération d'ordre de collecte au statut "traité"

<figure><img src="../../.gitbook/assets/Capture d&#x27;écran 2024-03-27 121407.png" alt=""><figcaption></figcaption></figure>

### Evolution des demandes d'achats pour intégration de prix unitaire et frais de livraison

      _Ce projet permet de créer des demandes d'achats en intégrant le prix de livraison mais aussi les prix unitaires des articles de la demande._&#x20;

* WEB | Paramétrages | Stock | Demandes | Achats - statuts :&#x20;
  * Nouvelle case à cocher pour activer un blocage de passage de statut si "frais de livraison" non rempli.&#x20;
* WEB | Demande | Achat :&#x20;
  * Ajout du champ fixe "Frais de livraison" qui redescend sur l'ordre de réception.&#x20;
  * Ajout du champ par référence "prix unitaire" qui redescend sur l'ordre de réception, sur les mouvements de stock et les articles.&#x20;
  * Ajout des champs frais de transport et prix unitaire dans l'exports CSV.
* WEB | Ordre | réception :&#x20;
  * Ajout des champs frais de transport et prix unitaire dans l'exports CSV.
* EDD : Ajout des champs frais de transport et prix unitaire dans l'entrepôt de données.

<figure><img src="../../.gitbook/assets/Capture d&#x27;écran 2024-03-27 121935.png" alt=""><figcaption></figcaption></figure>

### Encours de traçabilité sur les références gérées à l'article

      _Ce projet permet de visualiser des encours d'articles sur chaque emplacement._ &#x20;

*   WEB | Traçabilité | Encours&#x20;

    * Nouveau bouton "Gestion des colonnes" pour afficher les colonnes références et libellé.&#x20;
    * Le drag and drop des colonnes permet de sélectionner l'ordre des colonnes sur l'encours.



<figure><img src="../../.gitbook/assets/Capture d&#x27;écran 2024-03-27 121715.png" alt=""><figcaption></figcaption></figure>

### Export des acheminements avec choix des colonnes

&#x20;           _Ce projet permet d'exporter les demandes d'acheminements de façon planifié avec les colonnes dont vous avez besoin uniquement. L'ordre des colonnes sera l'ordre de sélection de celles-ci dans le filtre._&#x20;

* WEB | Paramétrage | Imports et mises à jour | Imports uniques et planifiés
  * Nouveau filtre pour les colonnes d'imports.
  * Nouvelle colonne "Date statut partiel" qui prend la dernière date du dernier statut partiel passé sur les demandes d'acheminements.&#x20;

<figure><img src="../../.gitbook/assets/Capture d&#x27;écran 2024-03-27 121840.png" alt=""><figcaption></figcaption></figure>
