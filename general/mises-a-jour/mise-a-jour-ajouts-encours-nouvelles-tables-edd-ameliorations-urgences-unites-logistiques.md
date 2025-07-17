---
description: Mise en production du 23/07/2025
---

# Mise à jour - Ajouts Encours, nouvelles tables EDD, améliorations Urgences, Unités logistiques

### Ajouts Traçabilité > Encours

_Objectif: plus de visibilité sur la page des encours de traçabilité avec l'ajout de nouvelles colonnes_

2 nouvelles colonnes ont été ajoutés sur la page Traçabilité > Encours:

* Nature de l'unité logistique
* Opérateur qui a effectué le dernier mouvement

Ces nouvelles colonnes ont également été ajoutées dans le fichier d'export et peuvent être renommées.

<figure><img src="../../.gitbook/assets/image (157).png" alt=""><figcaption></figcaption></figure>

### Nouvelles tables EDD

Dans la nouvelle version **6.23 de l'EDD**, de nouvelles tables et des modifications à venir:

**Nouvelles tables :**

* dw\_emplacement
  * id
  * nom
  * point\_de\_livraison
  * delai\_max\_traçabilité
  * statut
  * signataire
  * nouvelle\_nature\_prise
  * nouvelle\_nature\_depose
* dw\_calcul\_delai\_traitement
  * id
  * date\_calcul
  * unite\_logistique\_id
  * temps\_passé
* dw\_etapes\_calcul\_delai\_traitement
  * id
  * action
  * date\_action
  * emplacement\_id
  * nature\_id
  * calcul\_delai\_traitement\_id
*   dw\_nature

    * id
    * libellé
    * code
    * responsable



**Evolutions tables :**

* dw\_production :
  * Type
  * date\_création
  * date\_traitement
  * date\_dernier\_statut
  * cree\_par
  * traitee\_par



### Améliorations Urgences Stock

_Objectif: plus de flexibilité dans la création et modification des urgences_

* Il est possible de créer plusieurs urgences sur la même Référence
* Pour les références multi-fournisseur, celui affiché sur la page de liste des Urgences est le premier de la liste
* Les notions de Quantité initiale et Quantité restante ont été ajoutées, avec la possibilité de modifier la quantité initiale et mise à jour automatique de la quantité restante

<figure><img src="../../.gitbook/assets/image (156).png" alt=""><figcaption></figcaption></figure>



### Améliorations Traçabilité > Unités logistiques

Sur la page des Unités logistiques, il est maintenant possible de faire des recherches sur les champs libres.



### Ajout nouveau Champ fixe sur Arrivages UL

Un nouveau champ fixe a été ajouté sur les arrivages d'unités logistiques: "Impression UL". Il peut être affiché/ obligatoire à la création et/ ou affiché/ obligatoire à la modification, pour plus de flexibilité.

