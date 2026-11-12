---
description: >-
  Un rôle définit les fonctionnalités accessibles : consulter, créer, modifier,
  supprimer ou exporter.
---

# Rôles

### Créer un nouveau rôle

Cliquez sur le bouton <mark style="background-color:blue;">**Nouveau rôle**</mark>, vous allez être redirigé vers une nouvelle page. Sur celle-ci vous retrouver une liste de menus à gauche et les informations liées au rôle sur la droite.

* **Article** : lorsqu'un utilisateur effectuera une demande, il devra choisir précisément l'article à se faire livrer ou à collecter. L'opérateur qui traitera la demande devra prendre précisément l'article choisit pour clôturer la demande
* **Référence** : l'utilisateur ne choisira pas précisément l'article à se faire livrer ou a collecter lorsqu'il effectuera sa demande. Il demandera seulement une quantité de la ou des références souhaitées. C'est l'opérateur qui sélectionnera précisément l'article lorsqu'il traitera la demande

**Chemin :** Paramétrage › Utilisateurs › Rôles

Un rôle est attribué à un ou plusieurs utilisateurs. Exemples courants :

* **Administrateur** : équipe Wiilog ou 1-2 key users ;
* **Opérateur** : toutes les actions opérationnelles ;
* **Client / demandeur** : faire des demandes, créer des urgences, suivre l'avancement.

## Créer un rôle

Cliquez sur **Nouveau rôle**. La page affiche les menus à gauche et les droits à droite.

{% stepper %}
{% step %}
### Informations du rôle

| Champ                | Description                                                                                                                                                            |
| -------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **Libellé\***        | Nom du rôle.                                                                                                                                                           |
| **Ajout quantité\*** | **Article** : le demandeur choisit l'article précis à livrer ou collecter. **Référence** : il demande une quantité, et l'opérateur choisit les articles au traitement. |
| **Accueil\***        | Page d'accueil après connexion : **Dashboard**, **Planning** ou **Demande de transport**.                                                                              |
{% endstep %}

{% step %}
### Droits généraux

Dans **Général** : Afficher les notifications, Afficher le panier, Choisir la langue, Réception email de demande de création de compte, Afficher la documentation, Afficher le support.
{% endstep %}

{% step %}
### Droits par menu

Cochez les droits de chaque menu : Production, Traçabilité, Qualité & Urgences, Demande, Ordre, Stock, Référentiel, IoT, Nomade, Paramétrage, Dashboard. Le détail est dans les sous-pages.
{% endstep %}

{% step %}
### Enregistrer

Cliquez sur **Enregistrer**.
{% endstep %}
{% endstepper %}

## Modifier, supprimer

* **Modifier** : cliquez sur la ligne du rôle.
* **Supprimer** : poubelle de la ligne. Un rôle attribué à des utilisateurs ne peut pas être supprimé : retirez-le d'abord de ces utilisateurs.
