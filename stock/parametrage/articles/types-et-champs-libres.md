---
description: >-
  Créer les champs libres des articles et références, puis les rattacher aux
  types de références.
---

# Types et champs libres

**Chemin :** Paramétrage › Stock › Articles › Types et champs libres

Un **type** classe vos références (ex. : Consommables, Matériel informatique). Un **champ libre** ajoute une information propre à votre activité. La page se lit en deux temps : on crée d'abord les champs libres, puis on choisit lesquels s'affichent pour chaque type.

### 1. Créer les champs libres

Dans l'encadré **Champs libres**, cliquez sur **Modifier**, puis sur la ligne **+** pour ajouter un champ.

| Colonne                       | Description                                                                                                             |
| ----------------------------- | ----------------------------------------------------------------------------------------------------------------------- |
| **Libellé\***                 | Nom du champ (unique).                                                                                                  |
| **S'applique à**              | **Référence article** (le champ est sur la référence) ou **Article** (le champ est sur chaque article de la référence). |
| **Typage\***                  | Texte, Nombre, Oui/Non, Date, Date et heure, Liste ou Liste multiple.                                                   |
| **Éléments**                  | Valeurs de la liste, séparées par des « ; » (types Liste et Liste multiple uniquement).                                 |
| **Nb caractères (Min / Max)** | Longueur minimale et maximale autorisée.                                                                                |
| **Valeur par défaut**         | Valeur pré-remplie à la création (sauf Liste multiple).                                                                 |

<details>

<summary>Formats des typages</summary>

| Typage         | Format           | Exemple                                |
| -------------- | ---------------- | -------------------------------------- |
| Texte          | Texte libre      | Couleur : bleu                         |
| Nombre         | NNNN             | 12345                                  |
| Oui/Non        | Case à cocher    | Fragile : Oui                          |
| Date           | JJ/MM/AAAA       | 25/03/2026                             |
| Date et heure  | JJ/MM/AAAA HH:MM | 25/03/2026 17:53                       |
| Liste          | Choix unique     | En import/export : « Valeur »          |
| Liste multiple | Choix multiple   | En import/export : « Valeur1;Valeur2 » |

</details>

{% hint style="danger" %}
Supprimer un champ libre (poubelle en début de ligne) est **irréversible** : les données saisies dans ce champ sont perdues. Exportez vos données avant.
{% endhint %}

### 2. Paramétrer les types

Dans l'encadré **Types**, cliquez sur un type pour l'afficher, ou sur **Ajouter un type** pour en créer un.

{% stepper %}
{% step %}
#### Informations du type

Cliquez sur **Modifier**, puis renseignez le **Libellé\***, la **Description** et la **Couleur** (affichée dans les références et le panier).
{% endstep %}

{% step %}
#### Champs pour ce type

Ajoutez une ligne avec **+**, choisissez un **champ libre** dans la liste, puis cochez :

* **Affiché à la création** / **Obligatoire à la création**
* **Affiché à la modification** / **Obligatoire à la modification**
{% endstep %}

{% step %}
#### Enregistrer

Cliquez sur **Enregistrer**. Le bouton **Traduction des libellés** permet de traduire le libellé du type dans les autres langues.
{% endstep %}
{% endstepper %}

{% hint style="warning" %}
Un type ne peut pas être supprimé s'il est utilisé par des références.
{% endhint %}
