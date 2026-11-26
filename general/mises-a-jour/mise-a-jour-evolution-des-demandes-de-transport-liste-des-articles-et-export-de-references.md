---
description: Mise en production du 09/12/2026
---

# Mise à jour - Evolution des demandes de transport, liste des articles et export de références

### Demandes de transport - Nature des UL facultative à la création

**Problématique** : _Au moment de la saisie d'une demande de transport, le contenu exact à livrer ou à collecter n'est pas toujours connu. Rendre la nature obligatoire forçait une saisie approximative, à corriger ensuite._

**Fonctionnement** : La sélection d'une nature n'est plus obligatoire à la création d'une demande de transport. Les natures peuvent être choisies plus tard, au moment du colisage :

* **Si au moins une nature a été cochée** sur la demande, seules les natures sélectionnées sont proposées lors du clic sur « Imprimer les étiquettes ».
* **Si aucune nature n'a été cochée**, une modale permet de sélectionner les natures concernées puis, pour chacune, la quantité d'étiquettes et la plage de température (facultative).

Les natures proposées dans cette modale sont filtrées selon le type de livraison ou de collecte (service) de la demande : seules les natures autorisées pour ce service sont affichées.

### Demandes de transport - Nouvel import

**Problématique** : _Les demandes de livraison et de collecte sont souvent préparées en masse à partir d'une liste extraite d'un autre outil. Leur saisie une par une dans Follow représentait une double saisie chronophage._

**Fonctionnement** : Un nouvel import « Transport » permet de créer une liste de demandes de transport (sans nature) à partir d'un fichier CSV. Une ligne correspond à une demande.

| Colonne                    | Obligatoire                | Format attendu                                                            |
| -------------------------- | -------------------------- | ------------------------------------------------------------------------- |
| Type demande               | Oui                        | `Livraison` ou `Collecte`                                                 |
| Patient                    | Oui                        | Texte (prénom nom)                                                        |
| N° dossier                 | Oui                        | Numérique                                                                 |
| Adresse                    | Oui                        | Adresse complète (rue, CP, ville)                                         |
| Contact                    | Oui                        | N° de téléphone au format texte (pour conserver le 0 initial)             |
| Personne à prévenir        | Oui                        | Texte                                                                     |
| Remarque                   | Non                        | Texte libre                                                               |
| Service                    | Oui                        | Libellé d'un type de livraison ou de collecte paramétré (ex. HAD, Chimio) |
| Date et heure livraison    | Si Livraison               | `JJ/MM/AAAA HH:MM`                                                        |
| Date de collecte souhaitée | Si Collecte                | `JJ/MM/AAAA`                                                              |
| Urgence                    | Non (Livraison uniquement) | Valeur prédéfinie dans le paramétrage                                     |
| Nature1, Nature2…          | Non                        | Quantité informative (entier)                                             |
| Champs libres              | Selon paramétrage          | Valeur du champ libre du type de demande                                  |

L'import reproduit les règles de la création manuelle d'une demande de transport :

* **Livraison** : création de l'ordre de transport automatique dans le cas nominal ; passage **En attente de validation** pour une livraison le jour même ; passage en **Sous-traitée** pour un jour non travaillé ou un horaire non ouvré.
* **Collecte** : date indicative sans heure ni urgence ; une date passée est refusée ; une collecte le jour même passe **En attente de validation**.
* Le **Service** doit correspondre à un type existant pour le type de demande de la ligne.
* Une ligne est rejetée si une colonne obligatoire est vide, si une valeur n'est pas reconnue, ou si une collecte est déjà en cours pour le même N° dossier.

À la fin de l'import, un message indique le nombre de demandes créées, accompagné d'un rapport d'erreurs ligne par ligne (n° de ligne, colonne et motif).

### Tournées - Livraisons non préparées au démarrage

**Problématique** : _Lorsqu'une tournée démarrait alors qu'une des livraisons n'avait pas d'étiquettes (colis non préparés), cette livraison était écartée de la tournée mais restait « Affectée » : elle n'était ni livrée, ni replanifiable._

**Fonctionnement** : Au démarrage d'une tournée, une livraison dont les colis ne sont pas préparés est exclue de la tournée. Sa demande repasse au statut **À préparer** et son ordre au statut **À affecter**. Elle n'apparaît plus comme affectée dans le planning et peut être replanifiée sur une autre tournée.

### Stock - Liste des articles : impression des étiquettes et organisation des colonnes

**Problématique** : _Lorsque les articles sont créés automatiquement par l'interface avec l'ERP, aucune étiquette n'est imprimée au moment de leur création. Les opérateurs devaient retrouver un par un les nouveaux articles dans la liste pour imprimer leurs étiquettes, sans savoir lesquels avaient déjà été étiquetés._

**Fonctionnement** : La page Stock | Articles évolue :

* **Nouvelle colonne « Imprimer »** : un bouton est affiché sur chaque article dont l'étiquette n'a pas encore été imprimée. Au clic, l'étiquette est générée, l'article est marqué comme imprimé et le bouton disparaît sans recharger la page. Les articles existants avant la mise à jour sont considérés comme déjà imprimés.
* **Tri sur la date d'entrée en stock** : le tri fonctionne dans les deux sens, les articles sans date restent toujours en fin de liste. Le tri choisi est mémorisé d'une visite à l'autre.
* **Réorganisation des colonnes** : les colonnes peuvent être déplacées par glisser-déposer de leur en-tête. L'ordre est enregistré pour chaque utilisateur.

Pour en savoir plus, consultez la page [Articles](../../stock/fonctionnalites-web/articles.md).

### Données - Filtres sur l'export des références

**Problématique** : _Sur les bases contenant un très grand nombre de références, l'export complet des références pouvait ne pas aboutir en raison du volume de données._

**Fonctionnement** : Dans Paramétrage | Données | Exports CSV, l'export des **Références** propose deux nouveaux filtres facultatifs pour alléger le fichier :

* **Date de création (Du / Au)** : seules les références créées entre ces deux dates sont exportées ;
* **Statuts** : seules les références dans les statuts sélectionnés sont exportées.

Sans filtre, l'export reste complet. Pour en savoir plus, consultez la page [Export CSV](../../parametrages/donnees/export-csv.md).
