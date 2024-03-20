---
description: Mise en production du 24/01/2024
---

# Mise à jour - IoT Urgences 24h - Demandes en cours - Association BR nomade

### Mouvements automatisés de Prise / Dépose via IoT

      _Ce projet est utilisé pour suivre des unités logistiques sur un flux logistique spécifique. Ces unités logistiques vont être déposées sur une étagère portant un tracker. Lorsque l'étagère va être déplacer dans une zone de traitement : zone spécifique paramétré, des mouvements de prise / dépose de l'ensemble des colis déposés sur l'étagère seront réalisés automatiquement sur Follow._

<figure><img src="../../.gitbook/assets/Capture d&#x27;écran 2024-01-24 110207b.png" alt=""><figcaption><p>Schéma de fonctionnement général</p></figcaption></figure>

* WEB - IoT | Actionneur - Nouvel actionneur
  * Nouveau type de modèle "Dépose sur emplacement".
  * Possibilité d'ajouter des actionneurs de type "Dépose sur emplacement" à la l'"entrée" ou la "sortie" de la zone détectée.&#x20;
* WEB - IoT | Capteurs - Nouveaux capteur&#x20;
  * Nouveaux types de capteurs "Tracer Tracker" et "Zone".
*   WEB - Traçabilité | Mouvements : Mouvements de prise et déposes réalisés par les capteurs.



### Type service sur composant dashboard Demandes en cours

      _Ce projet est utilisé pour afficher spécifiquement des types de services sur le composant dashboard "Demandes en cours"._&#x20;

<figure><img src="../../.gitbook/assets/Capture d&#x27;écran 2024-01-24 114228.png" alt=""><figcaption><p>Image du composant Dashboard "Demandes en cours" filtré par service de type Kit SED</p></figcaption></figure>

### Association BR sur nomade

      _Ce projet permet de réaliser des associations BR depuis un nomade. Vous pourrez donc scanner et associer vos unités logistiques nouvellement créées avec vos numéros de réceptions d'ERP sans ordinateur._&#x20;

<figure><img src="../../.gitbook/assets/Capture d&#x27;écran 2024-01-24 115830.png" alt=""><figcaption><p>Ecrans du nomade pour l'association BR</p></figcaption></figure>

* WEB - Paramétrage | Utilisateurs | Rôles - Opérateur - Nomade - Trace "Accès associations BR"&#x20;
  * Ajout d'une case à cocher pour afficher la fonctionnalité "Association BR" dans le menu Trace du nomade.&#x20;
* NOMADE - Trace | Association BR&#x20;
  * Vous devez scanner votre numéro de réception puis vos unités logistiques qui lui sont associés.&#x20;

### Distinction Recette - Production

      _Ce projet permet d'aider visuellement à discerner les instances de recette et production. Les instances de recette porteront un bandeau aux couleurs de Wiilog (Cyan - violet) et le terme "Recette" sera affiché à côté de la version. La version de production restera telle quelle._&#x20;

<figure><img src="../../.gitbook/assets/Capture d&#x27;écran 2024-01-24 120142.png" alt=""><figcaption><p>Nouveaux design instances de Recette</p></figcaption></figure>
