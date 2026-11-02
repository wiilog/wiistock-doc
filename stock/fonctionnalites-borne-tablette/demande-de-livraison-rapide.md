---
description: >-
  Sortir un article du stock en autonomie depuis une tablette, sans passer par
  une demande de livraison classique.
---

# Demande de livraison rapide

**Où :** sur une tablette, depuis le lien externe créé dans [Paramétrage › Stock › Borne tactile](../parametrage/borne-tactile.md)

La tablette permet à un utilisateur de prendre lui-même un article ou une référence en stock. Follow GT enregistre automatiquement la demande, la préparation, la livraison et les mouvements de stock.

## Faire une sortie de stock

{% stepper %}
{% step %}
### Se connecter

Scannez ou saisissez votre **clé de connexion nomade**, puis appuyez sur **Connexion**.
{% endstep %}

{% step %}
### Rechercher la référence

Scannez le code-barres de la référence, ou tapez sa référence, son libellé ou sa référence fournisseur. Les filtres paramétrés sur le lien aident à affiner la recherche.
{% endstep %}

{% step %}
### Prendre l'article

La tablette affiche la photo de la référence (si elle est renseignée sur le web), son libellé, la quantité disponible, les codes fournisseurs et l'emplacement où la prendre. Pour une gestion à l'article, l'emplacement suit la règle FIFO ou FEFO.

Scannez le code-barres de l'article ou de la référence, selon le mode de gestion, puis saisissez la **quantité prise**.
{% endstep %}

{% step %}
### Compléter les informations

Renseignez les champs libres demandés pour le type de livraison.
{% endstep %}

{% step %}
### Confirmer

Vérifiez le récapitulatif, puis confirmez la sortie de stock.
{% endstep %}
{% endstepper %}

{% hint style="warning" %}
Vous ne pouvez pas prendre plus que la quantité disponible : un message d'erreur s'affiche.
{% endhint %}

## Ce que Follow GT crée automatiquement

| Élément                                  | Statut  |
| ---------------------------------------- | ------- |
| Demande de livraison                     | Livrée  |
| Ordre de préparation                     | Préparé |
| Ordre de livraison                       | Livré   |
| Mouvement de **transfert** (préparation) | —       |
| Mouvement de **sortie** (livraison)      | —       |

Un mail récapitulatif part vers les utilisateurs définis sur le lien.
