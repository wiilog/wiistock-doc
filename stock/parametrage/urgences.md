---
description: Types, champs libres et champs fixes des urgences de stock.
---

# Urgences

**Chemin :** Paramétrage › Stock › Urgences

## Types et champs libres

### 1. Créer les champs libres

Dans l'encadré **Champs libres**, cliquez sur **Modifier**, puis sur la ligne **+** :

| Colonne                       | Description                                                            |
| ----------------------------- | ---------------------------------------------------------------------- |
| **Libellé\***                 | Nom du champ (unique dans l'application).                              |
| **Typage\***                  | Texte, Nombre, Oui/Non, Date, Date et heure, Liste ou Liste multiple.  |
| **Éléments**                  | Valeurs de la liste, séparées par des « ; » (Liste et Liste multiple). |
| **Nb caractères (Min / Max)** | Longueur minimale et maximale autorisée.                               |
| **Valeur par défaut**         | Valeur pré-remplie à la création.                                      |

### 2. Paramétrer les types d'urgence

Dans l'encadré **Types**, cliquez sur un type ou sur **Ajouter un type**, puis sur **Modifier** :

| Champ                                         | Description                                                                                                                                                           |
| --------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **Libellé\*** / **Description** / **Couleur** | Identité du type.                                                                                                                                                     |
| **Par défaut**                                | Type proposé par défaut à la création d'une urgence.                                                                                                                  |
| **Alerte Email**                              | **Acheteur** et/ou **Demandeur** : un email leur est envoyé à chaque nouvelle réception concernant l'urgence (acheteur ou demandeur de l'urgence ou de la référence). |
| **Actif**                                     | Un type inactif n'est plus proposé.                                                                                                                                   |

Dans **Champs pour ce type**, ajoutez les champs libres avec **+** et cochez _Affiché / Obligatoire_ à la création et à la modification.

<figure><img src="../../.gitbook/assets/image (166).png" alt=""><figcaption></figcaption></figure>

## Champs fixes

Choisissez, pour le formulaire de création et pour celui de modification, les champs à **afficher** et ceux **obligatoires** : Commentaire, N° de commande, N° tracking transporteur, Transporteur, Pièces jointes, Emplacement attendu de l'urgence.

<figure><img src="../../.gitbook/assets/image (167).png" alt=""><figcaption></figcaption></figure>

Cliquez sur **Enregistrer** pour valider.
