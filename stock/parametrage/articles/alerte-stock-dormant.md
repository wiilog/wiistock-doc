---
description: >-
  Relancer automatiquement les gestionnaires par email sur les articles stockés
  depuis trop longtemps.
---

# Alerte stock dormant

**Chemin :** Paramétrage › Stock › Articles › Alerte stock dormant

Pour chaque référence qui a un gestionnaire, FollowGT envoie un email à la fréquence choisie. Le gestionnaire y choisit une action sur les articles dormants, via des boutons.

### 1. Boutons d'action de l'email

Dans **Informations de la demande de livraison**, ajoutez une ligne par bouton avec **+** :

* **Modèle de la demande de livraison** : modèle utilisé quand le gestionnaire clique sur le bouton (créé dans [Modèles de demande](../demandes/livraisons/modeles-de-demande.md)). Choisissez **Aucune demande de livraison** pour un bouton sans sortie de stock (ex. : « Garder ») ;
* **Libellé du bouton d'action\*** : texte du bouton dans l'email (ex. : « Garder », « Sortie »).

Le bouton **Déclencher les emails de relance** envoie les emails tout de suite, sans attendre la prochaine échéance.

### 2. Règles par type de référence

Dans **Fréquence d'interrogation des gestionnaires**, cliquez sur un type de référence, puis :

| Champ                                         | Description                                                                                                                                          |
| --------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------- |
| **Actif**                                     | Active l'alerte pour ce type.                                                                                                                        |
| **Temps d'immobilisation (j)**                | Nombre de jours depuis la dernière entrée en stock à partir duquel le gestionnaire est relancé. Il peut encore choisir de **prolonger** le stockage. |
| **Durée de stockage maximal (j)**             | Durée au-delà de laquelle le gestionnaire n'a plus le choix : l'article doit sortir du stock (ex. : être jeté).                                      |
| **Fréquence d'interrogation du gestionnaire** | **Chaque semaine** : date de début, toutes les X semaines, heure et jours. **Chaque mois** : date de début, mois et jours (1, 15 ou dernier jour).   |

Cliquez sur **Enregistrer** pour valider.
