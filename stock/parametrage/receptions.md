---
description: Statuts, champs et litiges des réceptions de stock.
---

# Réceptions

**Chemin :** Paramétrage › Stock › Réceptions

## Réceptions - Statuts

Le workflow des réceptions est fixe, mais vous pouvez :

* choisir l'**Emplacement de réception par défaut** : les articles créés à la réception y sont déposés automatiquement ;
* **renommer les 4 statuts** :

| Statut                      | Signification                                                    |
| --------------------------- | ---------------------------------------------------------------- |
| **En attente de réception** | La réception vient d'être créée.                                 |
| **Réception partielle**     | Une partie seulement des quantités attendues a été réceptionnée. |
| **Réception totale**        | La réception est terminée.                                       |
| **Anomalie**                | Une anomalie a été relevée sur la réception.                     |

## Réceptions - Champs fixes

Pour chaque champ, cochez **Afficher** / **Obligatoire** sur le formulaire de création et d'édition, et **Afficher** sur les filtres (case grisée = filtre non disponible).

Champs concernés : Fournisseur, Numéro de commande, Commentaire, Date attendue, Date commande, Utilisateur, Transporteur, Emplacement, Anomalie, Emplacement de stockage, Urgence, Pièces jointes.

## Réceptions - Champs libres

{% stepper %}
{% step %}
#### Créer les champs libres

Dans l'encadré **Champs libres**, cliquez sur **Modifier**, puis sur la ligne **+** :

| Colonne                       | Description                                                            |
| ----------------------------- | ---------------------------------------------------------------------- |
| **Libellé\***                 | Nom du champ (unique dans l'application).                              |
| **Typage\***                  | Texte, Nombre, Oui/Non, Date, Date et heure, Liste ou Liste multiple.  |
| **Éléments**                  | Valeurs de la liste, séparées par des « ; » (Liste et Liste multiple). |
| **Nb caractères (Min / Max)** | Longueur minimale et maximale autorisée.                               |
| **Valeur par défaut**         | Valeur pré-remplie à la création.                                      |
{% endstep %}

{% step %}
#### Les utiliser sur les réceptions

Dans **Utilisation des champs libres**, cliquez sur **Modifier**, ajoutez une ligne avec **+**, choisissez le champ libre et cochez _Affiché / Obligatoire_ à la création et à la modification.
{% endstep %}
{% endstepper %}

{% hint style="danger" %}
Supprimer un champ libre est irréversible : les données saisies sont perdues.
{% endhint %}

## Litiges - Types

Cliquez dans le tableau pour passer en modification, puis ajoutez une ligne avec **+** : **Libellé\*** et **Description**. Un type utilisé sur un litige ne peut pas être supprimé.

## Litiges - Statuts

Les statuts définissent les étapes de résolution d'un litige (communs à tous les types). Cliquez sur **Ajouter des statuts**, ou sur une ligne pour la modifier :

| Colonne                           | Description                                                              |
| --------------------------------- | ------------------------------------------------------------------------ |
| **Libellé\***                     | Nom du statut.                                                           |
| **État\***                        | **À traiter** (litige en cours) ou **Traité** (litige clôturé).          |
| **Commentaire litige**            | Commentaire ajouté automatiquement au litige quand il passe à ce statut. |
| **Statut par défaut**             | Statut appliqué à la création du litige.                                 |
| **Envoi d'emails aux acheteurs**  | Email aux acheteurs au passage à ce statut.                              |
| **Envoi d'emails aux demandeurs** | Email au déclarant du litige au passage à ce statut.                     |
| **Ordre\***                       | Position du statut dans la liste.                                        |

Un statut utilisé sur un litige ne peut pas être supprimé. Cliquez sur **Enregistrer** pour valider.
