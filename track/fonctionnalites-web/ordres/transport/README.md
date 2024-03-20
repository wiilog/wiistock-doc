---
description: >-
  Les ordres de transport servent à traiter les demandes de livraison et de
  collecte de colis.
---

# Transport

Cette page permet de récapituler toute les demandes de transport faites. Elle regroupe les demandes de livraison et de collecte. À noter que ces demandes de livraison et collecte sont différentes de celle présentés dans la partie Stock.

Lorsqu'une demande de transport est créé, un ordre est automatiquement créé (excepté dans le cas de la sous-traitance ou d’une demande en attente de validation). Les ordres sont différents des demandes car ils ne contiennent pas les mêmes informations et permettant d’agir dessus pour la planification de tournée.

Cette fonctionnalité est disponible dans le menu <mark style="background-color:blue;">**Ordre**</mark>, puis <mark style="background-color:blue;">**Transport**</mark>. Cette page contient plusieurs éléments :&#x20;

* Une **barre de filtre**, permettant de filtrer les données qui sont affichées dans le tableau
* Un bouton **Exporter au format CSV**, destiné à exporter l'ensemble des données filtrées (suivant les dates et le transport renseignés) au format CSV
* Un **tableau** sous forme d'étiquette, regroupant les différents ordres de transports créées

{% embed url="https://www.screencast.com/t/BbDhM36iF" %}
Page Ordre de transport
{% endembed %}

## Conrenu des filtres

Les filtres que vous mettez dans cette zone sont gardés en mémoire. C’est-à-dire que si vous filtrez la page, que vous quittez la page, que vous vous déconnectez, et que vous revenez sur la page, le filtre sera toujours présent

| Filte                  | Description                                                                                                                                                                                                         |
| ---------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **Du - Au**            | Filtre sur la date à faire des ordres de transport. Par défaut, le filtre Du est à la date du jour.                                                                                                              |
| **Demandeurs**         | Filtre sur les personnes ayant créées la demande de transport                                                                                                                                                     |
| **Dossier du patient** | Numéro de dossier du patient à livrer                                                                                                                                                                               |
| **Patient**            | Filtre sur le nom et prénom du patient. Le filtre est de type « Contient », c’est-à-dire qu’il va chercher si le champ Patient contient une partie de la chaîne de caractère que vous avez saisi dans le filtre |
| **Statut**             | Filtre sur le statut de la demande de transport. Vous pouvez mettre plusieurs statuts. Une partie des statuts sont différents entre les demandes et les collectes.                                                 |
| **Transport**          | Afficher seulement les livraisons ou seulement les collectes. En sélectionnant un transport, les types se filtrent automatiquement en fonction du transport                                                        |
| **Type**               | Voir seulement un type de transport                                                                                                                                                                                 |

## Contenu du tableau

La date en bleu, est la date de demande renseignée lors de la création de la demande. Puis il y a un récap du nombre de demandes de livraison et de collecte par jour.

Un bouton <mark style="background-color:blue;">**Exporter au format CSV**</mark>, destiné à exporter l'ensemble des données filtrées (suivant les dates et le transport renseignés) au format CSV.

Une liste d'étiquettes des demandes, le détail d'une étiquette de livraison et collecte est détaillés par la suite.

### Livraisons

{% embed url="https://www.screencast.com/t/VcjMLD3MR1ox" %}
Vignette d'un ordre de livraison
{% endembed %}

<table><thead><tr><th width="240.5">Information</th><th>Description</th></tr></thead><tbody><tr><td><strong>Livraison, Livraison/collecte</strong></td><td>Indication du choix du transport</td></tr><tr><td><strong>OTR220901-03</strong></td><td>Numéro de l'ordre de transport au format <br>(OTRaammjj-N) (OTR pour Ordre de TRansport)</td></tr><tr><td><strong>En cours</strong></td><td>Statut de l'ordre de transport. Le statut évolue automatiquement en fonction de l’avancée de l'ordre</td></tr><tr><td><strong>À faire à :</strong> </td><td>Heure à laquelle la demande doit être faite. Si l’heure est suivant d’un logo warning, c’est que la demande a été qualifiée d’urgente.</td></tr><tr><td><strong>Estimé à : (ou) Faite à :</strong> </td><td>Estimation de l’heure de traitement de la demande. Une fois que la demande a été planifiée sur une tournée, l’heure d’estimation apparaîtra à ce niveau.<br>Quand la demande est terminée, ce texte est remplacé par « Faite à : », ce qui correspond à l’heure de réalisation de la demande.</td></tr><tr><td><strong>Médicament</strong></td><td>Type de la demande (Pour le cas d’une livraison/collecte, vous ne verrez que le type de la livraison à ce niveau.)</td></tr><tr><td><strong>Patient (Didier Grenier)</strong></td><td>Nom du partient à livrer</td></tr><tr><td><strong>N° de dossier</strong></td><td>Numéro de dossier du patient renseigné sur la demande</td></tr><tr><td><strong>Créer le :</strong></td><td>Date de création de la demande</td></tr><tr><td><strong>Par :</strong></td><td>Personne qui à créé la demande</td></tr></tbody></table>

{% hint style="info" %}
Les Livraison/collecte ont les mêmes informations que les livraisons
{% endhint %}

Sur une étiquette vous pouvez aussi retrouver 2 icones :&#x20;

* Indication de colis écarté <img src="../../../../.gitbook/assets/colis-écarté.png" alt="" data-size="original">: La livraison contient des colis qui ont été rejetés par le livreur car non trouvés ou abîmés par exemple
* Indication livraison rejetée :<img src="../../../../.gitbook/assets/livraion-rejetée.png" alt="" data-size="original">une livraison peut être rejetée pour 2 raisons:
  * Tous les colis de la demande ont été écartés, aucun ne peut être livré en l’état. Dans ce cas, le statut de la demande qui était à «A livrer» passe à «A préparer» et il vous faut ré imprimer des étiquettespour qu’elle soit planifier ensuite sur une autre tournée
  * La livraison n’était pas préparée: aucun colis n’était disponible pour cette livraison. La demande reste alors au statut «A préparer». Il faudra la planifier sur une autre tournée dans la journée
* Indication de l'urgence <img src="../../../../.gitbook/assets/urgence.png" alt="" data-size="original">: Le triangle rouge indique que la livraion à été qualifiée d’urgente&#x20;

### Collecte

{% embed url="https://www.screencast.com/t/cOTF2ZoDhl2" %}
Vignette d'un ordre de collecte
{% endembed %}

Les éléments sont les mêmes, excepté la partie « Planifiée le ». Cette partie sert à savoir quand est-ce que la collecte a été planifiée avec le patient. Si aucune date n’apparaît, cela signifie que vous n’avez pas encore appelé le patient pour convenir d’une date de passage avec lui. L’estimation fonctionne pareil que sur la livraison.

## Exporter les données

Vous avez la possibilité d’exporter toutes les demandes et leurs données en format CSV (lisible sous excel).

Pour cela, renseignez d’abord des filtres de dates dans les filtres, et sélectionnez **Livraison** ou **Collecte**, pour exporter soit les ordres de livraison, soit les ordres de collecte. Cliquez ensuite sur <mark style="background-color:blue;">**Exporter au format CSV**</mark>. Vous obtiendrez les ordres de livraison ou de collecte créées entre les bornes de dates sélectionnées.
