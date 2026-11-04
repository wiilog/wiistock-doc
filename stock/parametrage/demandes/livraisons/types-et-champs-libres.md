---
description: Types de demandes de livraison et champs libres associés.
---

# Types et champs libres

**Chemin :** Paramétrage › Stock › Demandes › Livraisons - Types et champs libres

Les types distinguent vos flux de livraison. Les champs libres ajoutent des informations propres à chaque flux.

### 1. Créer les champs libres

Dans l'encadré **Champs libres**, cliquez sur **Modifier**, puis sur la ligne **+** :

| Colonne                       | Description                                                            |
| ----------------------------- | ---------------------------------------------------------------------- |
| **Libellé\***                 | Nom du champ (unique dans l'application).                              |
| **Typage\***                  | Texte, Nombre, Oui/Non, Date, Date et heure, Liste ou Liste multiple.  |
| **Éléments**                  | Valeurs de la liste, séparées par des « ; » (Liste et Liste multiple). |
| **Nb caractères (Min / Max)** | Longueur minimale et maximale autorisée.                               |
| **Valeur par défaut**         | Valeur pré-remplie à la création.                                      |

### 2. Paramétrer les types

Cliquez sur un type ou sur **Ajouter un type**, puis sur **Modifier** :

| Champ                                | Description                                                      |
| ------------------------------------ | ---------------------------------------------------------------- |
| **Libellé\*** / **Description**      | Nom (visible partout dans l'application) et description du type. |
| **Notifications push**               | Notifications sur le terminal mobile pour ce type.               |
| **Envoi d'un email au demandeur**    | Email au demandeur quand la demande est traitée.                 |
| **Envoi d'un email au destinataire** | Email au destinataire de la livraison.                           |
| **Actif**                            | Un type inactif n'est plus proposé.                              |

Dans **Champs pour ce type**, ajoutez les champs libres avec **+** et cochez _Affiché / Obligatoire_ à la création et à la modification. Cliquez sur **Enregistrer**.

{% hint style="warning" %}
Un type utilisé sur des livraisons ne peut pas être supprimé. Le typage d'un champ libre ne peut plus être modifié après création.
{% endhint %}
