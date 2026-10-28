---
description: Liste des tables de l'entrepôt de données (EDD) et de leurs colonnes.
---

# Dictionnaire des tables

Cette page complète la [Cartographie des données](cartographie-des-donnees.md). Elle liste les tables disponibles pour vos outils de BI (Power BI, etc.).

### Traçabilité

| Table                | Contenu                                               |
| -------------------- | ----------------------------------------------------- |
| `dw_arrivage`        | Arrivages d'unités logistiques                        |
| `dw_arrivage_camion` | Arrivages camion                                      |
| `dw_acheminement`    | Demandes d'acheminement                               |
| `dw_litige`          | Litiges                                               |
| `dw_nature`          | Natures d'UL : `id`, `libellé`, `code`, `responsable` |

#### `dw_emplacement`

`id`, `nom`, `point_de_livraison`, `delai_max_traçabilité`, `statut`, `signataire`, `nouvelle_nature_prise`, `nouvelle_nature_depose`

#### Délais de traitement

| Table                               | Colonnes                                                                                   |
| ----------------------------------- | ------------------------------------------------------------------------------------------ |
| `dw_calcul_delai_traitement`        | `id`, `date_calcul`, `unite_logistique_id`, `temps_passé`                                  |
| `dw_etapes_calcul_delai_traitement` | `id`, `action`, `date_action`, `emplacement_id`, `nature_id`, `calcul_delai_traitement_id` |

#### Tournées

| Table                      | Contenu                                                                                     |
| -------------------------- | ------------------------------------------------------------------------------------------- |
| `dw_tournee`               | Champs fixes de la tournée                                                                  |
| `dw_tournee_champs_libres` | Champs libres de la tournée                                                                 |
| `dw_tournee_ligne`         | Mouvements et actions de la tournée (mouvement de traçabilité ou litige, emplacement, etc.) |
| `dw_tournee_statuts`       | Statuts de la tournée                                                                       |

### Production

#### `dw_production`

Colonnes ajoutées en version 6.23 de l'EDD : `type`, `date_création`, `date_traitement`, `date_dernier_statut`, `cree_par`, `traitee_par`.
