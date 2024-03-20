---
description: Mise en production du 09/10/2023
---

# Mise à jour - Sortie de stock autonome & champ supplémentaire étiquette

**Champ supplémentaire sur étiquette**

Cette version contient les développements pour la demande spéciale "Champ supplémentaire sur étiquette"

* Paramétrages | Trace | Arrivages UL | Etiquettes : Afficher la date et l'heure d'un arrivage UL.



**Sortie de stock autonome / Caisse automatique**

Cette version contient également les développements pour le projet "Sortie de stock autonome via tablette"

* Paramétrages | Stock | Borne tactile :
  * Nouvelle page "Demande livraison rapide"
    * Possibilité de créer des liens externes de sortie de stock avec le duo "Type de livraison" - "Groupe de visibilité" unique.
    * Possibilité d'ajouter 3 filtres parmi les champs libres des articles ou références.
    * Possibilité de positionner des utilisateurs qui recevront un mail récapitulatif de la sortie de stock effectuée.
    * Possibilité de personnaliser le message d'accueil.
* Via le lien externe, redirection vers le flux tablette en 5 étapes :
  * Connexion de l'utilisateur via scan ou entrée manuelle de la clé nomade.
  * Recherche d'une référence avec les filtres paramétrés, via un scan de code barre de référence ou en tapant la référence, le libellé ou la référence fournisseur.
  * Affichage de la photo de la référence si renseignée sur le web, de son libellé, de la quantité disponible, des codes fournisseurs et de l'emplacement de stockage (en FIFO ou FEFO pour gestion à l'article)
    * L'utilisateur doit scanner le code barre article ou référence en fonction de la gestion choisie et entrer une quantité prise (message d'erreur si quantité prise supérieure à la quantité disponible
  * Affichage des champs libres du type à remplir.
  * Page récapitulative pour confirmation de la sortie de stock.
* Suite à la sortie de stock, un mail est envoyé avec le contenu de la demande.
* Suite à la sortie de stock, les pages suivantes sont créés :
  * Demande de livraison au statut livré
  * Ordre de préparation au statut préparé
  * Ordre de livraison au statut livré
* Suite à la sortie de stock, les mouvements suivants sont créés
  * Mouvement de transfert : Pour la préparation
  * Mouvement de sortie : Pour la livraison
