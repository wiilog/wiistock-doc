---
description: >-
  Un rôle permet de donner accés aux fonctionnalités de l'application. Un rôle
  permet de manière générale de consulter / modifier / supprimer ou exporter une
  donnée liée à une fonctionnalité.
---

# Rôles

L'application permet de créer un rôle qui pourra être affecté à un ou plusieurs utilisateurs de l'application.

**Les cas d'utilisation des rôles :**

* **Rôle super admin** : Rôle utilisé par les administrateurs de l'application de l'équipe Wiilog ou bien 1 ou 2 personnes de l'équipe portant la responsabilité de key user dans l'application.
* **Rôle opérateur** : Rôle utilisé par les opérateurs permettant d'effectuer toutes les actions et traitements opérationnels dans l'application
* **Rôle client** : Rôle utilisé par les demandeurs de stock ou bien un client acheteur permettant d'effectuer des demandes, création d'urgence et de consulter l'avancement des ordres

### Créer un nouveau rôle&#x20;

Depuis le menu Paramétrage, allez dans **Rôle** (sous-menu d'utilisateur) la liste des rôles déjà créée s'affiche.

Cliquez sur le bouton <mark style="background-color:blue;">**Nouveau rôle**</mark>, vous allez être redirigé vers une nouvelle page. Sur celle-ci vous retrouver une liste de menus à gauche et les informations liées au rôle sur la droite.

Renseignez le **libellé**, cela permet de donner un nom au rôle qui sera créé ou modifié.

\
Si sur votre instance vous utilisez les demandes de livraison et/ou de collecte, choisissez **l'ajout quantité** :

* **Article** : lorsqu'un utilisateur effectuera une demande, il devra choisir précisément l'article à se faire livrer ou à collecter. L'opérateur qui traitera la demande devra prendre précisément l'article choisit pour clôturer la demande
* **Référence** : l'utilisateur ne choisira pas précisément l'article à se faire livrer ou a collecter lorsqu'il effectuera sa demande. Il demandera seulement une quantité de la ou des références souhaitées. C'est l'opérateur qui sélectionnera précisément l'article lorsqu'il traitera la demande

La coche **Réception mail création nouveau compte** vous permet de recevoir un mail à chaque fois qu'un utilisateur se créer un compte sur l'instance.

Il faut ensuite choisir les droits à attribuer à ce rôle en allant cocher les droits dans les différents menus. Nous détaillerons dans des sous-menus de cette section l'impact de chaque droit.

### Supprimer un rôle

Dans la liste des rôles, vous pouvez en supprimer un, en cliquant sur l'icône corbeille.

{% hint style="info" %}
Lorsqu'un rôle est déjà associé à un ou plusieurs utilisateurs , il ne peut pas être supprimé, pour cela il faut préalablement dissocier tous les utilisateurs de ce rôle.
{% endhint %}

### Modifier un rôle

Pour modifier un rôle, cliquez sur la ligne du rôle à modifier pour passer en mode édition.

