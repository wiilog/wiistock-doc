---
description: Configuration RFID, fréquences, catégories et planification des inventaires.
---

# Inventaires

**Chemin :** Paramétrage › Stock › Inventaires

## Configuration

| Paramètre                     | Description                                                                                                 |
| ----------------------------- | ----------------------------------------------------------------------------------------------------------- |
| **Préfixe RFID**              | Si rempli, les scans RFID du module inventaire ne gardent que les étiquettes qui commencent par ce préfixe. |
| **Tranche pourcentage KPI 1** | Seuil (en %) qui met en avant les emplacements à rescanner en RFID.                                         |

## Fréquences

Une fréquence indique tous les combien de mois une référence ou un article doit être inventorié. Cliquez dans le tableau, puis ajoutez une ligne avec **+** :

* **Libellé\*** ;
* **Nombre de mois\*** (chiffres uniquement).

Une fréquence utilisée par une catégorie ne peut pas être supprimée.

## Catégories

Les catégories (ex. : classement ABC) sont associées à une fréquence. Elles permettent de générer automatiquement les missions d'inventaire selon la date du dernier inventaire de la référence ou de l'article.

* **Libellé\*** : catégorie à associer aux références ;
* **Fréquence\*** : à choisir parmi les fréquences paramétrées.

Une catégorie utilisée sur une référence ne peut pas être supprimée.

## Planificateur d'inventaire

Le planificateur crée automatiquement des missions d'inventaire. Cliquez sur **Planifier un inventaire** :

| Champ                                         | Description                                                                                                                                                                                                                                          |
| --------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **Type de mission\***                         | **Quantité article** : inventaire des références/articles des **Catégories\*** choisies. **Article sur emplacement** : inventaire d'emplacements, ajoutés par zone (**Ajout des emplacements des zones**) ou un par un (**Ajout des emplacements**). |
| **Libellé de la tâche\*** / **Description\*** | Nom et description de la mission.                                                                                                                                                                                                                    |
| **Durée\***                                   | Durée de la mission.                                                                                                                                                                                                                                 |
| **Créé par\***                                | Auteur de la planification.                                                                                                                                                                                                                          |
| **Fréquence**                                 | Une fois, chaque heure, chaque jour, chaque semaine ou chaque mois.                                                                                                                                                                                  |

Le tableau liste les planifications (type, périodicité, catégories, durée, dernière exécution, actif). Les **⋮** en début de ligne donnent accès aux actions.

Cliquez sur **Enregistrer** pour valider.
