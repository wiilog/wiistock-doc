---
description: 25/07/2022
---

# Mise à jour - Projets multiples

**Brique TRACK**

Cette nouvelle partie de l’application correspond à tous les développements qui ont été effectués pour sur la brique Track.

Cette nouvelle partie permet de :

* Faire des **demandes de transport** (dans le sens Client vers prestataire) de livraison et/ou de collecte
* Côté prestataire, recevoir les **ordres de transport** résultant des demandes à traiter
* Planifier les ordres de transport sur des **tournées** via un outil de création de tournée
* Traiter les tournées sur le terminal mobile
* Suivre **l’avancement** des demandes de transport, avec un **suivi GPS et de température** si paramétré

Vous trouverez donc des nouvelles sections dans le paramétrage pour cette partie, une évolution du paramétrage des natures de colis et des emplacements, une nouvelle page _Véhicules_ dans le référentiel, ainsi que les nouvelles pages _Demande | Transport_, _Ordre | Transport_, _Ordre | Planning_, _Ordre | Tournée_, _Ordre | Sous-traitance_. Le paramétrage du GPS et capteurs de température s’appuie sur la brique IoT livrée l’année dernière.

Ces nouvelles fonctionnalités sont de la traçabilité et n’incluent pas de gestion de stock.



**Brique STOCK**

**Nouveau process de demande de livraison avec lancement des préparations et prévision de stock:**

Ce nouveau développement consiste à :

* Pouvoir faire une demande de livraison sur des références sans contrôle du stock disponible (nouveau paramétrage permettant cela)
* Positionner une date attendue sur une demande de livraison (ajout de la gestion de champ fixe sur demande de livraison pour ajouter la date attendue)
* Envoyer les ordres de préparation résultant de ces demandes de livraisons sur un planning
* A partir du planning, faire un lancement de préparation qui vient contrôler le stock des références demandées à ce moment là
* Sur le détail des fiches références, vous pouvez voir le stock prévisionnel de la référence. Le calcul se base sur les demandes de livraison qui ont une date attendue, et les attendues de réception (réception avec une date attendue)



**Autres fonctionnalités STOCK:**

* _Ordre | Réception | Détails_ - **Nouveau design du conditionnement** des réceptions permettant d’éviter de saisir sur chaque article des informations communes à tous
* _Ordre | Réception | Détails_ – _Stock | Articles_ – Ajout de la **date d’entrée en stock sur les étiquettes** article (paramétrable dans Paramétrage | Stock | Articles | Etiquettes)
* _Paramétrage | Stock | Demandes | Livraisons_ : Nouveaux paramétrages pour gérer le **comportement d’une demande de livraison créée suite à une réception**
* _Paramétrage | Terminal mobile | Gestion des validations_ : ajout d’un paramétrage pour **enlever la validation de sélection d’emplacement pour la livraison manuelle**
* _Paramétrage | Stock | Inventaires | Gestion des missions_ – Nouveau paramétrage pour **paramétrer la génération automatique de mission d’inventaire** en fonction des catégories d’inventaire attribuées aux références : tous les dimanches soirs, les missions d’inventaire se créent selon les caractéristiques paramétrées avec dedans les références et articles qui ont leur date de dernier inventaire dépassée par rapport à leur catégorie
* _Stock | Références | Articles de référence_ – Pour les références gérées à l’article, le champ « Date de denier inventaire » est modifié en « **Inventaire à jour** » : toutes les nuits, un algorithme regarde si toutes les dates de denier inventaire de tous les articles de la référence ne sont pas supérieures à la fréquence d’inventaire paramétrée. Si une des dates est supérieure, l’inventaire est marqué comme n’étant pas à jour. Si toutes les dates sont inférieures, l’inventaire est à jour
* _Stock | Inventaire_ – Ajout d’un **libellé de mission** lors d’une création de mission d’inventaire
* _Nomade – Inventaire_ : **amélioration ergonomique** du traitement d’un inventaire + ajout d’une **vue des missions** d’inventaire
* _Nomade – Stock_ : **réorganisation** des menus de la partie Stock et **nouveaux logos**
* _Nomade – Stock_ : nouveau menu **Livraison manuelle**. Ce menu permet de réaliser des sorties de stock via le nomade sans passer par un ordre de livraison. Ce menu fonctionne seulement pour des articles. Flashez l’article que vous sortez du stock et ensuite l’emplacement de sortie de stock. Un mouvement de sortie de stock sera créé pour l’article et un ordre de livraison au statut traité sera créé



**Dashboard**

* Ajout d’un paramétrage sur les dashboard pour **mettre en valeur** 1 ou 2 composants de type « Quantité en cours sur n emplacement(s) » qui ont les **délais les plus courts**



**Brique TRACE**

* _Traçabilité | Mouvements_ – Ajout d’un droit dans le paramétrage afin de pouvoir **modifier tous les champs de la modale de modification de mouvement**
* _Nomade – Acheminement_ : Ajout de la possibilité d’associer des **photos sur un colis dans un acheminement**. Les photos remontent dans les pièces-jointes de la demande d’acheminement et dans les pièces-jointes des mouvements résultants de l’acheminement
