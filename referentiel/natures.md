---
description: Les natures d'UL classent les marchandises par catégorie.
---

# Natures

**Chemin :** Référentiel › Nature

## Créer une nature

Cliquez sur **Ajouter une nature** et renseignez :

| Champ                                                           | Description                                                                                                                                                                  |
| --------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **Libellé\*** / **Code\*** / **Description**                    | Identité de la nature.                                                                                                                                                       |
| **Couleur\***                                                   | Couleur sur les dashboards et le nomade.                                                                                                                                     |
| **Préfixe**                                                     | Préfixe du numéro d'UL généré à l'arrivage.                                                                                                                                  |
| **Températures**                                                | Plages de température de la nature (définies dans [Températures](../track/parametrage/temperatures.md)).                                                                     |
| **Quantité par défaut de l'arrivage\*** / **de l'acheminement** | Nombre d'UL pré-rempli sur ces formulaires.                                                                                                                                  |
| **Synchronisation nomade ?**                                    | La nature peut être choisie sur le nomade pour une UL inconnue scannée.                                                                                                      |
| **Nature par défaut**                                           | Nature donnée aux UL sans nature connue ajoutées à un acheminement.                                                                                                          |
| **Affichage sur les formulaires ?**                             | Formulaires où la nature est proposée : **Arrivage**, **Transport - Collecte**, **Transport - Livraison** (en choisissant les types de demande concernés), **Acheminement**. |

### Délais de traitement (suivi des encours)

| Champ                                        | Description                                                 |
| -------------------------------------------- | ----------------------------------------------------------- |
| **Délai de traitement de la nature**         | Temps dans lequel une UL de cette nature doit être traitée. |
| **Responsable de la nature**                 | Personne alertée en cas de dépassement.                     |
| **Délai de traitement de la nature dépassé** | Couleur d'affichage des UL en retard (encours, dashboards). |
| **Segments horaires**                        | Tranches de retard affichées dans les dashboards.           |

Cliquez sur **Enregistrer**.

## Modifier, supprimer

* **Modifier** : cliquez sur la ligne.
* **Supprimer** : menu **⋮** de la ligne. Une nature déjà utilisée ne peut pas être supprimée.
