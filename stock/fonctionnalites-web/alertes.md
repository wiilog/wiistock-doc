---
description: >-
  La page des alertes contient toutes les alertes liées aux références du stock,
  en plus de l'envoi de mail quand il y a des alertes.
---

# Alertes

&#x20;Cette page est disponible dans le menu **Stock**, puis **Alertes**. Cette page contient plusieurs éléments :&#x20;

* Une **barre de filtre**, permettant de filtrer les données qui sont affichées dans le tableau
* Une **recherche rapide**, permettant également de filtrer les données affichées dans le tableau
* Un bouton <mark style="background-color:blue;">**Exporter au format CSV**</mark>, destiné à exporter l'ensemble des données filtrées (suivant les dates renseignées) au format CSV
* Un **tableau**, regroupant les différentes alertes

{% embed url="https://www.screencast.com/t/MoG6il1j0i" %}
Page alertes
{% endembed %}

### Contenu des filtres

| Filtre            | Description                                                                                                            |
| ----------------- | ---------------------------------------------------------------------------------------------------------------------- |
| **Du**            | La tranche basse filtrant sur la date de création de l'alerte                                                          |
| **Au**            | La tranche haute filtrant sur la date de création de l'alerte                                                          |
| **Types**         | Type de la référence, pour afficher seulement les alertes des types de référence choisis                               |
| **Alerte**        | Catégorie de l'alerte                                                                                                  |
| **Gestionnaires** | Gestionnaire de la référence, pour afficher seulement les alertes des références ayant le(s) gestionnaire(s) choisi(s) |

### Contenu du tableau

| Colonne                 | Description                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                      |
| ----------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **Type d'alerte**       | <p>Type de l'alerte. 3 types sont possibles : <br>- <strong>Péremption</strong> : la date de péremption de l'article en alerte est dépassée ou alerte va être dépassée d'ici le délai paramétré (dans Paramétrage | Stock | Alertes)<br>- <strong>Seuil d'alerte</strong> : la quantité de la référence est passée en dessous du seuil d'alerte paramétré sur la référence<br>- <strong>Seuil de sécurité</strong> : la quantité de la référence est passée en dessous du seuil de sécurité paramétré sur la référence. Le seuil de sécurité est inférieur au seuil d'alerte</p> |
| **Date d'alerte**       | Date à laquelle l'alerte s'est déclenchée                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                        |
| **Libellé**             | Libellé de la référence en alerte                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                |
| **Référence**           | Référence en alerte                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                              |
| **Code barre**          | Code barre de l'article ou de la référence en alerte                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                             |
| **Quantité disponible** | Quantité disponible de la référence en article                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                   |
| **Type quantité**       | Gestion quantité de la référence (référence en gestion quantité référence, ou référence en gestion quantité article)                                                                                                                                                                                                                                                                                                                                                                                                                                                             |
| **Seuil d'alerte**      | Niveau du seuil d'alerte de la référence                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                         |
| **Seuil de sécurité**   | Niveau du seuil de sécurité de la référence                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                      |
| **Date de péremption**  | Date de péremption de l'article qui a l'alerte                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                   |
| **Gestionnaire(s)**     | Gestionnaire(s) de la référence                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                  |

Sur le tableau, vous pouvez également :&#x20;

* **Voir si la référence en alerte est dans une demande d'achat ou dans une réception en attente de réception**. Une légende indique les couleurs de chaque ligne en fonction de si la référence est en demande d'achat ou en attente de réception
* **Ajouter la référence au panier**. Un petit logo panier est disponible à gauche de chaque ligne de référence en alerte
* **Aller sur la fiche de la référence**. Cliquez sur<img src="../../.gitbook/assets/3points" alt="" data-size="line">et sur le bouton Aller sur la référence pour arriver sur la fiche de la référence en alerte

### Mails d'alerte de seuil de sécurité et d'alertes

Si le paramétrage est activé ([Paramétrage | Stock | Alertes](../parametrages/alertes.md)), les gestionnaires des références peuvent recevoir des mails lorsqu'une alerte est déclenchée.&#x20;

![Exemple de mail d'alerte de seuil](<../../.gitbook/assets/Seuil de sécurité.PNG>)

Dans le mail vous retrouverez différentes informations :&#x20;

* **Référence** : le nom de la référence
* **Gestion** : si la référence est en gestion quantité par référence ou par article
* **Quantité disponible** : quantité disponible pour les demandes (quantité non présente dans des demandes en cours)
* **Quantité réservée** : quantité réservée sur des demandes en cours
* **Quantité en stock** : quantité totale encore en stock&#x20;
* **Seuil d'alerte** : première quantité d'alerte
* **Seuil de sécurité** : quantité la plus basse d'alerte
* **Champs libres**
* **Fournisseurs** : tableau des fournisseurs de la référence avec le nom de la référence chez le fournisseur

### Mails d'alerte de péremption

Si un délais d'alerte de péremption est paramétré ([Paramétrage | Stock | Alertes](../parametrages/alertes.md)), un mail sera envoyé aux gestionnaires de la référence x jours avant la date de péremption de l'article.

![Mail d'alerte de péremption](<../../.gitbook/assets/seuil péremption.PNG>)

