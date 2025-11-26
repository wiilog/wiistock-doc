# Tournée

La demande de Tournée permet d'attribuer à un opérateur, un ordre de passage précis sur des emplacements pré-définis. Il peut, sur ces emplacements, faire des prises/déposes d'UL ou passage à vide si besoin.&#x20;

Cette fonctionnalité est disponible dans le menu Demande puis Tournée. Ou via le bouton + puis Tournée.&#x20;

Cette page contient :

* Une **barre de filtre**, permettant de filtrer les données qui sont affichées dans le tableau
* Une **recherche rapide**, permettant également de filtrer les données affichées dans le tableau
* Un bouton **Exporter au format CSV**, destiné à exporter l'ensemble des données filtrées (suivant les dates renseignées) au format CSV
* Un **tableau**, regroupant les différentes demandes de Tournées créées

### Contenu des filtres

<table><thead><tr><th width="251.52720639646054">Filtre</th><th>Description</th></tr></thead><tbody><tr><td><strong>Du</strong></td><td>La tranche basse filtrant sur la date de création de la demande de tournée</td></tr><tr><td><strong>Au</strong></td><td>La tranche haute filtrant sur la date de création de la demande de tournée</td></tr><tr><td><strong>Statut</strong></td><td>Le(s) statut(s) des demandes de tournée à filtrer</td></tr><tr><td><strong>Type</strong></td><td>Le type des demandes de tournée à filtrer</td></tr><tr><td><strong>Emplacement de la tournée</strong></td><td>Filtrer la demande par l'emplacement de la tournée. Cet emplacement est pré-défini lors du paramétrage de la tournée. C'est l'emplacement sur lequel l'opérateur viendra faire sa tournée </td></tr></tbody></table>

### Contenu du tableau

| Colonne                                | Description                                                                                                                                                            |
| -------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **Numéro**                             | Numéro de la demande de tournée généré par l'application Wiilog. Il est constitué du préfixe TO, de l'année, du mois, du jour, de l'heure et de la minute de création. |
| **Date de création**                   | Date de création de la demande de tournée                                                                                                                              |
| **Date et heure de démarrage attendu** | Date et heure auxquelles l'opérateur doit démarrer la tournée. Elles sont indiquées lors de la création d'une tournée.                                                 |
| **Date de traitement**                 | Date et heure auxquelles la tournée a été terminée.                                                                                                                    |
| **Statut**                             | Statut de la demande de tournée                                                                                                                                        |
| **Type**                               | Type de la demande de tournée                                                                                                                                          |
| **Traité par**                         | L'utilisateur qui à traité la demande de tournée                                                                                                                       |
| Demandeur                              | Le demandeur de la demande de tournée                                                                                                                                  |
| Urgence                                | Si la demande est classée urgence et sous quel délai                                                                                                                   |
| Commentaire                            | Le commentaire associé à la demande de tournée                                                                                                                         |
| Emplacement de la tournée              | L'emplacement sur lequel l'opérateur va faire sa tournée (ex: chariot\_01)                                                                                             |

### Créer une demande de tournée

#### Via le bouton "+"



<div align="left"><figure><img src="../../../.gitbook/assets/Capture d’écran 2025-11-26 à 14.46.18.png" alt=""><figcaption></figcaption></figure></div>

Au clic sur la tournée une modale "Nouvelle demande de tournée" s'ouvrira comprenant :



* **Type**&#x20;
* **Statut**
* **Date et heure de démarrage attendu**
* **Emplacement de la tournée**
* **Urgence**
* **Champs libres**

{% hint style="info" %}
Le choix des statuts est conditionné par le champ **Type**. Il s'agit d'un paramétrage modifiable dans le menu Paramétrages > Trace > tournées
{% endhint %}

### Passer les statuts d'une demande de tournée

Cliquer sur la ligne de la demande de tournée concernée.&#x20;

Ci-dessous une vidéo explicative avec vue WEB + vue NOMADE.&#x20;

Ici, comme exemple, l'opérateur va faire des prises, déposes et passage à vide sur les emplacements de sa tournée. Les UL "Cadeau1" ou "Surprise1" sont créées manuellement mais peuvent être scannées par l'opérateur.

De même pour sélectionner un emplacement, il doit le scanner.

{% file src="../../../.gitbook/assets/Vidéo Tournée.mov" %}

