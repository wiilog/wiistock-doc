---
description: Mise en production du 11/09/2023 - Version 7.0.2
---

# Mise à jour - Demandes d'achats sur références & évolution des demandes d'acheminements

## \[STOCK] Visualisation des demandes d'achats sur référence (Web)

* Si le paramétrage du rôle "<mark style="background-color:blue;">**Afficher les demandes d'achats**</mark>" est coché, alors :&#x20;
  * Depuis la **page Stock | Références**, au clic des 3 points à droite de la ligne de la référence, nouveau bouton pour afficher les demandes d'achats liées à cette référence.

## \[TRACE] Evolution des demandes d'acheminements (Web)

* **Paramétrages | Trace | Acheminements | Champs fixes** - Nouveaux champs fixes liés au référentiel Client.
  * Client
  * A l'attention de
  * Téléphone client
  * Adresse de livraison\

*   **Paramétrages | Trace | Acheminements | Champs fixes** - Nouveaux champs fixes liés au Unités logistiques

    * Hauteur (m)
    * Largeur (m)
    * Longueur (m)
    * Volume (m3) ==> Calculé automatiquement à partir des données précédentes
    * Poids (Kg)
    * Commentaire
    * Date dernier mouvement
    * Dernier emplacement
    * Opérateur
    * Statut


* **Demande | Acheminement** - Création d'une demande d'acheminement : Au clic sur le numéro d'acheminement, celui-ci est copié dans le presse-papier.
* **Demande | Acheminement** - Création d'une demande d'acheminement : Au statut "Partiel", possibilité de faire apparaître un bouton "Générer une étiquette" qui imprimera le contenu de l'acheminement (1 étiquette par UL d'acheminement) unqiuement si paramétrage du rôle coché sur Paramétrage | Rôles | Demande | Acheminement - Générer une étiquette"
* **Paramétrage | Données | Exports CSV :** Possibilité d'exporter les demandes d'acheminements via export CSV unique et planifié.&#x20;
