---
description: Mise en production du 11/06/2026
---

# Mise à jour - Améliorations diverses, projet détrompeur & EDD

## Améliorations UX

#### 1.  Possibilité de rendre inactif un type d'urgence pour ne plus afficher les urgences Stock ou Trace - WEB

Depuis la mise en place de paramétrages des Urgences Trace et Stock, il était nécessaire d'avoir au moins un type d'urgence actif par catégorie Trace et Stock, ce qui vous obligeait a afficher un type inutile chez vous. Aujourd'hui, vous pouvez rendre inactif les types qui ne vous sont pas utiles. Ainsi, vous n'affichez à vous utilisateurs que les types d'urgences qui leurs sont pertinents.&#x20;

<figure><img src="../../.gitbook/assets/image (182).png" alt=""><figcaption></figcaption></figure>



#### 2.  Lien de redirection des emails de litige amélioré - Emails

Les liens de redirection placés dans les emails de changement de statut des litiges ont étés améliorés. Ils redirigent maintenant vers la liste des litiges préfiltrée sur le numéro de litige concerné. L'utilisateur devra d'abord être connecté à follow pour ensuite visualiser le litige.&#x20;

<figure><img src="../../.gitbook/assets/image (184).png" alt=""><figcaption></figcaption></figure>

#### 3.  Numéro de projet redescend de l'arrivage UL sur l'UL - WEB

Le numéro de projet est un champ fixe que vous pouvez renseigner lors de l'arrivage UL. Il est maintenant directement intégré dans la page de liste des UL, dans la gestion des colonnes et dans la page de détails de l'UL.&#x20;

#### 4.  Amélioration du visuel du détail des acheminements - WEB

Afin d'améliorer le visuel des pages de détails des acheminements, nous avons rassemblé les champs fixes et les champs libres dans un seul encart "Informations". D'un point de vue utilisateurs, il est plus facile de retrouver l'ensemble des données au même endroit que de devoir distinguer des champs libres ou fixes qui sont des notions propres à FollowGT.&#x20;



## Détrompeurs sur mouvements de traçabilité - Nomade

Depuis la page Paramétrage | Mouvements | Détrompeurs, vous pouvez créer des détrompeurs pour prévenir vos opérateurs ou les bloquer lors de mouvements de traçabilité nomade.&#x20;

Vous pouvez : Bloquer ou Faire confirmer la prise selon les conditions suivantes :&#x20;

* Le code de l'UL commence par "xxx", "xxx"&#x20;
* Le code de l'UL ne commence pas par "xxx", "xxx"&#x20;
* L'UL existe&#x20;
* L'UL n'existe pas&#x20;
* L'UL est présente sur l'emplacement de prise
* Le code de l'UL ne contient pas entre min et max inclus de caractères
* L'UL a une nature autorisée
* L'UL n'a pas une nature autorisée

<figure><img src="../../.gitbook/assets/image (183).png" alt=""><figcaption></figcaption></figure>

Vous pouvez également choisir les rôles ainsi que les fonctionnalités qui seront impactées. Le message affiché à l'utilisateur lors du déclenchement du critère est personnalisable. Si plusieurs détrompeurs se déclenchent, l'affichage fonctionnera comme suivant :&#x20;

* Blocage & Confirmation ⇒ Message de blocage uniquement affiché
* Confirmation & Confirmation ⇒ Message en liste avec les deux messages dans une pop-up et un seul bouton de confirmation
* Blocage & Blocage ⇒ Message en liste avec les deux messages dans une pop-up et un seul bouton de OK.&#x20;



## Evolution de l'entrepôt de données - Tournées

Mise en place de l'entrepôt de donnée lié à la fonctionnalité Tournée.&#x20;

Vous pouvez maintenant appeler les données de tournées depuis un outil de BI avec l'aide des tables suivantes :&#x20;

* dw\_tournee : table de visualisation des champs fixes de la tournée
* dw\_tournee\_champs\_libres : table de visualisation des champs libres de la tournée
* dw\_tournee\_ligne : table de correspondance des mouvements et actions dans la tournée : mouvement de traçabilité ou litige, emplacement de l'action, etc.&#x20;
* dw\_tournee\_statuts : table de visualisation des statuts de la tournée

D'autres ajustements sur les autres tables ont été fait pour assurer les connexions entre les tables.

<figure><img src="../../.gitbook/assets/image (185).png" alt=""><figcaption></figcaption></figure>

