---
description: Suivre une tournée en détail, l'ajuster et générer les bons de transport.
---

# Détails d'une tournée

**Chemin :** Ordre › Tournée › clic sur une vignette

Le détail d'une tournée a 3 zones : **Tournée**, **Transports** et **Données**.

<figure><img src="../../../../.gitbook/assets/Formations CLB12.png" alt=""><figcaption><p>Détails d'une tournée</p></figcaption></figure>

## Zone Tournée

* **Numéro**, créateur, **date** de la tournée et **livreur**.
* **Historique des statuts** (En attente livreur, En cours, Terminée) avec leur horodatage : vert = statut actuel, bleu = passé, gris = pas encore atteint.
* **Temps estimé / réel** : l'estimation va du point de départ du calcul des horaires jusqu'à la fin de tournée, avec le temps de passage moyen du [paramétrage](../../../parametrage/tournees.md). Le temps réel va du passage _En cours_ au passage _Terminée_.
* **Kilomètres estimés / réels** : l'estimation suit le trajet point de départ km › point de départ horaires › points de passage › retour. Le réel utilise les positions GPS du boîtier connecté, si le livreur en a un.
* **Éléments rejetés** (si besoin) : UL **écartées** par le livreur (introuvables ou non conformes) et livraisons **rejetées** (toutes les UL écartées ou aucune UL préparée), à replanifier sur une autre tournée.

## Zone Transports

La liste des points de passage dans l'ordre : numéro, **nom du patient** (cliquable vers le [détail de l'ordre](../transport/details-dun-ordre-de-transport.md)), livraison ou collecte, heure **estimée** et heure **réelle**.

* Couleur : vert = en cours, gris = à venir, bleu = traité.
* Icône UL écartée : des UL ont été écartées au chargement (motif visible dans le détail de l'ordre). Croix rouge : transport annulé.

<figure><img src="../../../../.gitbook/assets/Capture d’écran 2023-02-03 à 16.55.40.png" alt=""><figcaption></figcaption></figure>

Le menu **⋮** à côté de **Transports** propose, selon le statut :

| Statut             | Actions                                                                                                                                                             |
| ------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Tous               | **Générer un bon de transport** : un PDF avec un bon par livraison.                                                                                                 |
| En attente livreur | **Ajouter un transport** : ajouter des livraisons ou collectes, changer l'ordre des points, le livreur et recalculer les estimations (pas de suppression de point). |
| En cours           | **Ajouter une collecte** : seules des collectes peuvent être ajoutées.                                                                                              |

## Zone Données

<figure><img src="../../../../.gitbook/assets/Formations CLB15.png" alt=""><figcaption><p>Détails d'une tournée, partie Données</p></figcaption></figure>

* **Carte** : point de départ et d'arrivée, point de départ du calcul des horaires, points de passage numérotés et, si la tournée est en cours, dernière position du livreur.
* **Courbe de température** : une courbe par frigo équipé d'une sonde, avec le nom de la sonde, les bornes haute et basse et les relevés du début à la fin de la tournée.

## Modifier une tournée

Pour une tournée **non démarrée** : menu **⋮** › **Ajouter un transport**, ou [Ordre › Planning](../planning.md) › **Planifier une tournée** › **Ajouter à la tournée**. Vous pouvez alors modifier l'ordre et les points de passage, les points de début et de fin, le livreur et l'heure de départ, puis cliquer sur **Valider la tournée**.

{% hint style="info" %}
Sur une tournée **en cours**, seules des collectes peuvent être ajoutées. Pour de nouvelles livraisons, créez une nouvelle tournée.
{% endhint %}
