---
description: >-
  Paramètres des tournées : calcul des kilomètres et horaires, motifs,
  conditions de fin de tournée et emplacements de retour.
---

# Tournées

**Chemin :** Paramétrage › Track › Tournées

### Calcul kilométrage et durée

| Paramètre                               | Description                                                                                                |
| --------------------------------------- | ---------------------------------------------------------------------------------------------------------- |
| **Point de départ km**                  | Adresse à partir de laquelle on compte les kilomètres de la tournée.                                       |
| **Point de départ calcul des horaires** | Adresse à partir de laquelle on calcule les horaires de passage.                                           |
| **Point d'arrivée**                     | Dernier point de la tournée.                                                                               |
| **Heure(s) de départ**                  | Heure (HH:MM) et livreur(s) associés : sert à estimer les heures de passage. Ajoutez une ligne avec **+**. |
| **Temps de passage moyen (minutes)**    | Temps passé chez le patient, pour une livraison, une collecte et une livraison/collecte.                   |

{% hint style="info" %}
Les 3 adresses peuvent être identiques ou différentes (utile pour la facturation).
{% endhint %}

### Motifs

| Paramètre                                    | Effet                                                                                                     |
| -------------------------------------------- | --------------------------------------------------------------------------------------------------------- |
| **Motifs d'écartement**                      | Raisons proposées au livreur quand il écarte une UL au chargement (ex. : mauvais état, manque étiquette). |
| **Motifs de non livraison**                  | La livraison passe au statut _Non livrée_.                                                                |
| **Motifs de non collecte**                   | La collecte repasse en _Patient à contacter_ pour être replanifiée.                                       |
| **Fin du workflow collecte pour les motifs** | Pour ces motifs, la collecte passe au statut _Non collectée_ (pas de replanification).                    |

### Fin de tournée

| Paramètre                                       | Effet                                                                                            |
| ----------------------------------------------- | ------------------------------------------------------------------------------------------------ |
| **Emplacements de fin de tournée**              | Le livreur doit flasher l'un de ces emplacements pour terminer la tournée.                       |
| **Natures obligatoires à déposer**              | Natures d'UL non livrées que le livreur doit déposer à son retour pour pouvoir finir la tournée. |
| **Emplacements de dépose des objets collectés** | Où le livreur dépose les objets collectés.                                                       |
| **Emplacements de retour des UL non livrées**   | Où le livreur dépose les UL non livrées.                                                         |

Cliquez sur **Enregistrer** pour valider.
