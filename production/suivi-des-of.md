---
description: >-
  Créer, suivre et faire avancer les demandes de production (ordres de
  fabrication).
---

# Suivi des OF

**Chemin :** Production › Liste des OF · ou **+** › Production

La brique Production aide les ordonnanceurs à répartir les ordres de fabrication (OF) dans un atelier. Une demande de production peut être créée à la main, ou importée (import unique ou planifié depuis un fichier Excel).

## Créer une demande de production

{% stepper %}
{% step %}
### Choisir le type

Cliquez sur **+** › **Production**, puis choisissez le **Type\*** et le **Statut\***. Les champs du type s'affichent.
{% endstep %}

{% step %}
### Remplir la demande

Selon le paramétrage des [champs fixes](parametrage/champs-fixes.md) : Numéro d'OF, Code produit/article, Date attendue, Emplacement de dépose, Emplacement de destination, Quantité, Nombre de lignes, Numéro projet, Urgence, Commentaire, Pièces jointes. Puis les champs libres du type.
{% endstep %}

{% step %}
### Enregistrer

La demande apparaît dans la liste des OF et, selon le paramétrage des statuts, dans le [planning](vue-planning.md).
{% endstep %}
{% endstepper %}

<figure><img src="../.gitbook/assets/image (95) (1).png" alt=""><figcaption><p>Création d'une demande de production</p></figcaption></figure>

## Faire avancer une demande

Cliquez sur une ligne pour ouvrir le détail (informations, champs libres, pièces jointes, **Historique** de chaque changement). Cliquez sur **Avancer la demande**, choisissez le nouveau **Statut\*** et ajoutez si besoin un commentaire. Selon le statut, une pièce jointe peut être obligatoire.

<figure><img src="../.gitbook/assets/image (97).png" alt=""><figcaption></figcaption></figure>

## Actions

| Action                                                | Où                                          | Effet                                                                                                                                                                                        |
| ----------------------------------------------------- | ------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **Modifier** / **Supprimer**                          | Menu **⋮** de la ligne ou du détail         | Modifie ou supprime la demande.                                                                                                                                                              |
| **Dupliquer**                                         | Menu **⋮** de la ligne                      | Crée jusqu'à 10 copies. Tous les champs sont modifiables sauf le type. Les pièces jointes ne sont pas copiées. Droit à activer dans les rôles.                                               |
| **Acheminer**                                         | Flèche à côté de **Exporter au format CSV** | Cochez les demandes puis **Valider production à acheminer** : une demande d'acheminement est créée pour ces productions. Les demandes déjà acheminées (icône ⇄) ne sont pas sélectionnables. |
| **Exporter au format CSV** / **Gestion des colonnes** | En haut du tableau                          | Export et choix des colonnes.                                                                                                                                                                |

## Demande d'acheminement depuis un statut

Si le [statut](parametrage/statuts.md) le prévoit (**Proposition de générer une demande d'acheminement**), le passage à ce statut propose de créer une demande d'acheminement. Choisissez **créer une nouvelle demande** ou **ajouter à une demande existante**, puis renseignez les UL à acheminer dans la **Liste des UL**. Voir [Acheminements](../trace/fonctionnalites-web/demandes/acheminements/).

<figure><img src="../.gitbook/assets/Capture d’écran 2025-03-12 à 12.17.32.png" alt=""><figcaption></figcaption></figure>

<details>

<summary>Filtres et colonnes</summary>

**Filtres :** Du / Au (date de création ou date attendue), Type, Statuts, Créé par, Urgence, Code produit/article, Emplacement de dépose, Numéro d'OF, Pièces jointes. Les filtres disponibles se choisissent dans la [configuration](parametrage/configurations.md).

**Colonnes :** Numéro, Date de création, Créé par, Traité par, Type, Statut, Date attendue, Emplacement de dépose, Nombre de lignes, Numéro d'OF, Code produit/article, Quantité, Urgence, Numéro projet, Commentaire, et les champs libres. Une ligne en rouge signale une urgence.

</details>
