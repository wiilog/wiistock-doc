---
description: >-
  Les paramétrages des mouvements permettent de créer des champs libres sur les
  mouvements mais aussi de configurer des alertes automatisées.
---

# Mouvements

## Configurations

* **Vider et rester sur la modale de création de mouvement** : si ce paramétrage est coché, lorsque vous créez des mouvements via la supervision, la modale de création de mouvement restera toujours ouverte à la création d'un mouvement et se videra
*   **Afficher le détrompeur sur les mouvements de prise si UL non disponible sur l'emplacement** : si ce paramétrage est coché, lorsque vous réaliser un mouvement de prise d'une Unité Logistique, sur Web ou Nomade, vous aurez un message pour vous prévenir si l'Unité Logistique n'a pas été prise sur un emplacement sur lequel elle avait été déposée.&#x20;

    _Par exemple : Je fais mon arrivage UL sur l'emplacement RECEPTION, si je prends l'UL que je viens de déposer sur un autre emplacement que RECEPTION, alors j'aurais un message pour me prévenir que cette UL n'était pas posée sur cet emplacement._&#x20;

**Mails de relance** :&#x20;

* **Déclencher un mail de relance si colis sur point de livraison dropzone à 7j, 15j, 30j, et 42j** : si un colis reste un certain temps sur un point de livraison et est associé à un destinataire, ce destinataire recevra des mails aux intervalles décrits pour venir récupérer son colis
* Bouton **Déclencher les mails de relance** : ce bouton sert à lancer les mails de relance en un coup sans avoir à cocher le paramétrage

## Champs libres

Il est possible d'ajouter des champs libres sur les mouvements.

Les champs libres se paramètrent dans un tableau avec les informations suivantes :&#x20;

| Colonne                           | Description                                                                                                                                                                                                                                                                                                                                                                                                                                                                                      |
| --------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| **Libellé**                       | Nom du champ libre                                                                                                                                                                                                                                                                                                                                                                                                                                                                               |
| **Typage**                        | <p>Typage du champ libre. 7 types sont possibles : <br>- Texte : champ de saisie libre<br>- Nombre : champ dans lequel il est seulement possible de saisir des nombres<br>- Oui/Non : choix entre 2 choix Oui et Non<br>- Date : le champ ouvrira un calendrier à la selection<br>- Date et heure : le champ ouvrira un calendrier à la sélection et un sélecteur d'heure<br>- Liste : sélection d'un choix parmi une liste<br>- Liste multiple : sélection de plusieurs choix par une liste</p> |
| **Eléments**                      | Eléments de la liste pour les types Liste et Liste multiple                                                                                                                                                                                                                                                                                                                                                                                                                                      |
| **Valeur par défaut**             | Valeur par défaut du champ libre. En fonction du typage choisi, le modèle de choix du valeur par défaut change                                                                                                                                                                                                                                                                                                                                                                                   |
| **Affiché à la création**         | Cochez la case pour que le champ libre apparaisse à la création du mouvement                                                                                                                                                                                                                                                                                                                                                                                                                     |
| **Obligatoire à la création**     | Cochez la case pour que le champ libre soit obligatoire pour valider la création du mouvement                                                                                                                                                                                                                                                                                                                                                                                                    |
| **Obligatoire à la modification** | Cochez la case pour que le champ libre soit obligatoire pour valider la modification du mouvement                                                                                                                                                                                                                                                                                                                                                                                                |
