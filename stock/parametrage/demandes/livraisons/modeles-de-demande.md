---
description: >-
  Modèles qui créent automatiquement une demande de livraison (bouton connecté
  ou alerte stock dormant).
---

# Modèles de demande

**Chemin :** Paramétrage › Stock › Demandes › Livraisons - Modèle de demande

Un modèle de demande crée automatiquement une demande de livraison (en _À traiter_, avec son ordre de préparation en _À traiter_) :

* à l'appui sur un **bouton connecté** (IoT) ;
* ou depuis un email d'[alerte stock dormant](../../articles/alerte-stock-dormant.md).

### Créer un modèle

Cliquez sur **Ajouter un modèle de demande**, puis renseignez :

| Champ                     | Description                                                                    |
| ------------------------- | ------------------------------------------------------------------------------ |
| **Nom du modèle\***       | Nom affiché lors de l'association.                                             |
| **Type de livraison\***   | Type de la demande créée.                                                      |
| **Utilisation du modèle** | **Actionneur** (bouton connecté) ou **Stock dormant**. Non modifiable ensuite. |
| **Destination\***         | Emplacement de livraison.                                                      |
| **Commentaire**           | Commentaire de la demande.                                                     |

Ajoutez ensuite les références avec **+** : **Référence\*** (libellé et emplacement se remplissent seuls) et **Quantité à livrer\***. Cliquez sur **Enregistrer**.

{% hint style="info" %}
Les références sont toujours ajoutées « par référence », même si elles sont gérées par article : le choix des articles se fait à la préparation.
{% endhint %}

### Modifier ou supprimer

Choisissez le modèle dans **Modèle de la demande**, puis cliquez sur **Modifier** ou sur la poubelle. Un modèle associé à un objet connecté ne peut pas être supprimé.
