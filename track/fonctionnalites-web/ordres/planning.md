---
description: >-
  Cette page permet de planifier une tournée et de suivre l'évolution des
  demandes affectées sur des tournées
---

# Planning

Pour accéder à la page, vous devez aller dans le menu **Ordre**, puis choisir **Planning**.

La page contient plusieurs éléments :&#x20;

* Une **barre de filtre**, permettant de filtrer les données qui sont affichées dans le tableau
* Une **recherche rapide**, permettant également de filtrer les données affichées dans le tableau
* Un bouton <mark style="background-color:blue;">**Planifier une tournée**</mark>, destiné à la la création d'une tournée
* Un **tableau**, affichant le jour en cours et le lendemain regroupant les différents demandes créés.

{% embed url="https://www.screencast.com/t/ebaF2KsZ6X" %}

**Contenue filtre**

* Un bouton <mark style="background-color:blue;">**Aujourd'hui**</mark> : pour pouvoir revenir facilement aux demandes du jour
* Deux boutons **flèches** pour pouvoir naviguer sur le planning
* Trois boutons filtre, vous pouvez filtrer sur les **statuts des demandes**, par défaut ils sont tous sélectionnés :&#x20;
  * **À affecter** : La demande n'est pas encore positionnée sur une tournée
  * **Affecté** : La demande est positionnée sur une tournée
  * **En cours** : la demande est en cours de traitement, le livreur a démarré la tournée

**Contenue tableau/planning**

Sur le planing on affiche par défaut le jour en cours et J+1. Pour chaque jour il y a 2 colonnes, une pour les livraisons et une pour les collectes. Les vignettes de couleur correspondent à une demande.

Sur les vignettes on affiche :&#x20;

{% embed url="https://www.screencast.com/t/J5QRjaPk" %}
Vignette de transport au statut affecté
{% endembed %}

| Libellé                   | Description                                                                                                     |
| ------------------------- | --------------------------------------------------------------------------------------------------------------- |
| Médicament & DMS          | Type de la livraison ou de la collecte                                                                          |
| Emmanuelle Breton         | Patient à livrer                                                                                                |
| N°134577                  | N°de dossier patient                                                                                            |
| 09:20 ou Matin/Après-midi | <p>Horaire de passage souhaité (livraison)<br>Créneau de passage renseigné avec le patient (collecte)</p>       |
| T230202-01                | Si le transport est affecté sur une tournée, il y a le N°de la tournée, il renvoie vers le détail de la tournée |
| Xavier Francois           | Si le transport est affecté sur une tournée, le livreur en charge de celle-ci est renseigné                     |

## Planifier une tournée

Une modale s’ouvre. Vous avez le choix entre créer une nouvelle tournée ou l’ajouter à une tournée existante. Pour l’ajouter à une tournée existante, sélectionnez « Ajouter à la tournée ». Il vous est proposé les numéros des tournées qui ne sont pas « En cours ».

Pour créer une nouvelle tournée, sélectionnez « Créer une nouvelle tournée pour le ». Par défaut, la date est à J+1. Sélectionnez la date à laquelle la tournée doit s’effectuer et cliquez sur <mark style="background-color:blue;">**Suivant**</mark>.

{% embed url="https://www.screencast.com/t/R8ino06YbM" %}
Page de planification de tournée
{% endembed %}

Sur la nouvelle page qui s’affiche, vous avez trois sections :

* **Transports à affecter** : contient les transports à faire pour la journée sélectionnée non planifiée sur une tournée. Les transports sont classés par heure à faire : du plus tôt dans la journée au plus tard
* **Transports affectés** : liste des transports qui seront à faire dans cette tournée et ordre des transports
*   **Nouvelle tournée** : carte des transports et paramétrage de la tournée

    Pour passer un transport dans la colonne « Transports affectés », vous pouvez glisser-déposer les vignettes de la colonne « Transports à affecter » à « Transports affectés ».

Vous avez aussi la possibilité de cliquer sur les pins sur la carte dans la section « Nouvelle tournée » pour passer un transport en affecté.

Si vous passez la souris sur une vignette, le point est mis en valeur sur la carte. Les points sur la carte contiennent le nom du patient et l’horaire a laquelle il faut passer chez le patient.

Si vous voulez enlever un point de la colonne « Transports affectés », cliquez sur la croix à droite de la vignette.

Vous pouvez aussi changer l’ordre de passage en glissant une vignette entre deux autres vignettes dans cette colonne.

{% embed url="https://www.screencast.com/t/qy5QEjShv0ui" %}
Affecter des transport à une tournée
{% endembed %}

Dans la partie « Nouvelle tournée », vous avez différents éléments essentiels pour avoir la planification de la tournée et les estimations :

* **Point de départ** : ce point de départ sert à calculer le kilométrage de la tournée dès le départ du livreur au dépôt
* **Point de départ calcul horaire** : Ce point correspond au moment où le livreur débute réellement la tournée après avoir chargé les colis. C’est à partir de ce point que les estimations de passage chez les patients sont calculées
*   **Point d’arrivée** : point finale de la livraison pour le calcul du kilométrage. Cela peut correspond au dépôt si le livreur rentre directement au dépôt après être passé chez le dernier patient.

    _Ces 3 adresses peuvent être paramétrées par défaut dans le paramétrage pour ne pas avoir à la saisir systématiquement_.
* **Livreur** : livreur qui va effectuer la tournée. Attention à bien avoir associé un véhicule à votre livreur dans la page Référentiel | Véhicules. Si vous avez effectué le paramétrage, la sélection du livreur renseigner automatiquement l’heure de départ
* **Heure de départ** : à la sélection du livreur, le champ se déverrouille et se renseigne si une heure de départ par défaut a été renseigné pour le livreur dans le paramétrage. Si vous n’avez pas fait ce paramétrage, renseignez l’heure de départ du livreur. Cet horaire correspond à l’heure à laquelle le livreur quitte le dépôt pour effectuer sa tournée.

Avec tous ces champs remplis, le bouton <mark style="background-color:blue;">**Calculer les horaires**</mark> est disponible. Cliquez dessus pour voir toutes les estimations d’heure de passage chez les patients et avoir le kilométrage estimé et le temps estimé. Vous pouvez ainsi remodeler la tournée si les horaires ne sont pas corrects.

Si la tournée vous convient, cliquez sur <mark style="background-color:blue;">**Valider la tournée**</mark> pour créer la tournée. Tous les ordres que vous avez placé dans cette tournée passe alors en « Affecté » et le demendeur pourra voir sur les demandes l’estimation du créneau de passage de la demande.

{% embed url="https://www.screencast.com/t/bHeF7vhOJ" %}
Estimation d'une tournée
{% endembed %}

À la validation de la tournée vous êtes renvoyé vers le détail de la tournée. Voir détails de la tournée.
