---
description: Mise en production du 17/04/2024
---

# Mises à jour - Génération de bon de commande, demande de devis via email et dépose multiple sur web

### Génération d'un bon de commande depuis une demande d'achat&#x20;

      _Ce projet permet de générer un bon de commande depuis une demande d'achat. Vous pourrez intégrer votre propre modèle de bon de commande en utilisant les variables proposées. La génération du bon de commande peut également vous faire passer sur un statut suivant._&#x20;

* WEB | Paramétrages | Utilisateurs | Rôles :
  * Nouvelle case à cocher pour le droit "Afficher achats"
* WEB | Paramétrages | Modèle de document | Achats - Bon de commande :&#x20;
  * Liste des variables qui peuvent être affichées et intégration d'un modèle de document personnalisable.
* WEB | Demande | Achat : &#x20;
  * Nouveau bouton "Générer bon de commande" et passage de statut automatisé.
* WEB | Paramétrage | Stock | Demande | Achat - statut :&#x20;
  * Nouvelle case à cocher pour le passage automatique du statut à la génération du bon de commande.



### Demande de devis depuis email de seuil d'alerte et seuil de sécurité

      _Ce projet permet de créer des emails depuis un email de seuil d'alerte ou de sécurité d'une référence. Les informations concernant la référence seront préremplies ainsi que l'email au fournisseur._  &#x20;

* WEB | Email : Nouveau bouton "Demander un devis au fournisseur"
  * Génération d'un nouvel email avec pré remplissage des informations du devis. &#x20;
* WEB | Référentiel | Fournisseur :
  * Nouvelles colonnes pour le référentiel fournisseur : email, destinataire, téléphone, adresse.

### Dépose multiple sur web

      _Ce projet permet de créer des mouvements de dépose depuis le web de façon multiple._&#x20;

*   WEB | Traçabilité | Mouvements - Nouveau mouvement "Dépose" :&#x20;

    * Possibilité de mettre plusieurs unités logistiques sur la dépose sur emplacement.&#x20;

    \
