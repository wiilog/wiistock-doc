---
description: Mise en production du 25/06/2025
---

# Mise à jour - IOT GPS, Prise & Dépose simultanée NOMADE, Améliorations Référentiel

### Nouveaux IOT GPS

**Objectif** : Suivre les trajets de véhicules.\
Nous avons intégré sur Follow de nouveau capteurs GPS équipés de carte SIM et branchés sur prise OBD du véhicule.

![](<../../.gitbook/assets/image (152).png>)\
Les capteurs remontent des coordonnées GPS permettant de suivre le chemin des véhicules sur lesquels ils sont branchés sur Follow.

<figure><img src="../../.gitbook/assets/image (153).png" alt=""><figcaption></figcaption></figure>

### Changement de la liste des unités logistiques et groupage

**Objectif** : Centraliser les informations des unités logistiques sur la page liste des UL et faciliter la création d'UL via des mouvements de traçabilité nomade rapides.

* WEB - Liste des unités logistiques :
  * Les champs libres des mouvements de traçabilité et des arrivages UL sont maintenant visibles depuis la liste des UL et sur le détail de chaque UL.
* WEB & NOMADE - Mouvements :&#x20;
  * Il est maintenant possible de transformer une UL en groupe tant que celle-ci a été générée à partir de mouvements de traçabilité (pas d'arrivage ou autre).
* NOMADE - Mouvements :&#x20;
  * Un nouveau menu de prise et dépose en une page est disponible. Pour activer l'affichage de ce nouveau menu nomade, vous devrez l'afficher dans le paramétrage des rôles.

<figure><img src="../../.gitbook/assets/image (155).png" alt=""><figcaption></figcaption></figure>

### Nouveau fonctionnel Référentiel Projet

**Objectif** : Faire porter aux articles lors des réceptions un projet provenant du référentiel projet.

* Paramétrage | Stock | Articles | Champs fixes - Ajout d’un nouveau champ fixe “Projet” qui peut être affiché et/ou obligatoire sur le formulaire de création et de modification.
* Ordre | Réception : Réception de références gérées à l’article : le champs projet si affiché via paramétrage peut être rempli dans la réception des articles.

<figure><img src="../../.gitbook/assets/image (154).png" alt=""><figcaption></figcaption></figure>

* Stock | Articles | détails : Le champs projet doit être rempli avec la donnée renseigné lors de la réception



### Améliorations / mise en conformité référentiels

Référentiel Emplacements: ajout de colonnes au fichier d'import et nouvel export des Emplacements.
