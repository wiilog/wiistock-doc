# Imports & mises à jour

La fonction d'import et de mise à jour permet soit d'importer de nouvelles données dans l'application ou mettre à jour des données existantes. L'intérêt de cette fonction est un gain de temps important, en l'occurrence la création unitaire d'une importante base de données dans l'application peut être très chronophage.

&#x20;Les types de données concernées par cette fonction sont les suivants :

* Articles
* Références
* Fournisseurs
* Réceptions
* [Articles fournisseurs](imports-and-mises-a-jour.md#article-fournisseur)
* Utilisateurs
* Livraisons
* Emplacements
* [Demandes de transport](imports-and-mises-a-jour.md#demande-de-transport)
## Création d'un nouvel import ou maj

Commencez par cliquer sur le bouton "**Nouvel import"**, cela ouvrira la fenêtre Import d'un fichier. Sur cette fenêtre :

1. Renseignez le nom de l'import souhaité
2. Puis sélectionnez le type de données à importer dans la liste
3. Enfin, ajoutez le fichier au format CSV (délimiteur point virgule, encodage UTF-8 et <2 Mo) contenant les données à importer ou à mettre à jour.
4. Suite à la validation de l'import, une nouvelle fenêtre s'ouvre contenant un tableau avec 3 colonnes, cette étape nous permet d'associer les champs du fichier importé et les champs Follow GT. Une association entre ces 2 champs est déjà faite, vous pouvez néanmoins modifier les champs Follow GT s'il y a des erreurs.

* **Titre de colonne de fichier** : Libellé de chaque colonne, cela correspond aux valeurs de la première ligne de votre fichier d'import, qui pourraient correspondre à des titres de colonnes.
* **Aperçu (ligne 1)** :  Correspond aux valeurs de chaque colonne de la deuxième ligne de votre fichier d'import.
* **Champs Follow GT** : Liste déroulante, qui contient tous les champs (champs libres et fixes) liés au type de données à importer. Les champs avec une astérisque sont des champs obligatoires à la création de l'import ou de la mise à jour.

5\. Enfin cliquez sur "**Valider"** pour lancer l'import ou la mise à jour, si l'import est trop volumineux, il passera au statut "planifié" et sera exécuté plus tard, sinon il sera au statut "en cours", puis passera au statut "terminé" lorsqu'il sera finalisé.

{% hint style="info" %}
**Règle de planification des imports** : Pour les imports de moins de 100 lignes, lancement immédiat. Pour les imports entre 100 et 500 lignes, lancement dans les 30 prochaines minutes. Pour les imports entre 500 et + lignes, lancement à minuit.
{% endhint %}

## Liste des imports et mise à jour

#### Filtres

Pour rechercher plus facilement une information, vous pouvez appliquer un filtre sur les imports. Vous pouvez filtrer sur les dates, le statut et l'utilisateur qui a fait l'import.

#### Le tableau

Les détails de l'import seront visibles sur le tableau de l'historique des imports, il comporte des informations sur les imports ainsi que certaines actions que l'on pourra exécuter :

* **Actions** (les 3 points au début de la ligne) :&#x20;
  * **Bouton Dupliquer l'import** : permet de créer un import en dupliquant les paramètres renseignés sur un import précédemment exécuté.&#x20;
  * **Bouton Fichier trace** : Lorsqu'un import est au statut "Terminé", ce bouton permet de télécharger le fichier de traces au format CSV. En cas d'erreurs d'import, le fichier de trace contient le détail des erreurs par ligne.
* **Statut** : Indique le statut de l'import ou de la mise à jour , soit il peut être "en cours", "planifié", "annulé" ou "terminé"
* **Date début** : Indique la date et l'heure du lancement de l'import ou de la mise à jour
* **Date fin** : Indique la date et l'heure de fin de l'import ou de la mise à jour
* **Nom import** : Indique le nom de l'import renseigné lors de la création de l'import
* **Nvx enreg**. : Indique le nombre de type de données créées
* **Mises à jour** : Indique le nombre de type de données mises à jour
* **Nombre d'erreurs** : Indique le nombre d'erreurs suite à l'import ou à la mise à jour
* **Utilisateur** : Indique le nom de l'utilisateur qui a exécuté l'import ou la mise à jour
* **Type de données importées** : Indique le type de donnée qui à été importé ou mise à jour

### Article fournisseur

Suite à un import de référence vous pouvez importer en masse un ou des fournisseurs pour les sychoniser avec les références.

Le modèle d'import comporte 4 colonnes :&#x20;

| Colonne de l'import                  | Équivalence page référence | Explications                        |
| ------------------------------------ | -------------------------- | ----------------------------------- |
| **Libellé**                          | Label/libellé              | Label de la Ref article fournisseur |
| **Référence\***                      | Ref article fournisseur    |                                     |
| **Référence article de référence\*** | Code de Référence          | Référence de l'article de référence |
| **Référence fournisseur\***          | Code fournisseur           |                                     |

### Demande de transport

Cet import permet de créer en masse des demandes de transport (livraisons et collectes). Chaque ligne du fichier crée une demande, qui suit les mêmes règles qu'une demande créée manuellement (statut, ordre de transport, sous-traitance, mail de validation).

Le modèle d'import comporte 11 colonnes :

| Colonne de l'import                               | Explications                                                                                                                                                                  |
| ------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **Type demande\***                                | « Livraison » ou « Collecte ».                                                                                                                                                |
| **Patient\***                                     | Nom du patient.                                                                                                                                                               |
| **N° dossier\***                                  | Numéro de dossier du patient (uniquement des chiffres).                                                                                                                       |
| **Adresse\***                                     | Adresse de livraison ou de collecte. Elle doit pouvoir être retrouvée par la géolocalisation.                                                                                 |
| **Contact\***                                     | Numéro de téléphone du contact, saisi tel quel (le 0 initial est conservé).                                                                                                   |
| **Personne à prévenir\***                         | Nom de la personne à prévenir.                                                                                                                                                |
| **Remarque**                                      | Remarque libre.                                                                                                                                                               |
| **Service\***                                     | Libellé d'un type de demande de transport existant : un type de livraison si le Type demande est « Livraison », un type de collecte s'il est « Collecte ».                    |
| **Date et heure livraison (jj/mm/AAAA hh:MM)**    | Obligatoire pour une livraison, à laisser vide pour une collecte.                                                                                                             |
| **Date de collecte souhaitée (jj/mm/AAAA)**       | Obligatoire pour une collecte, à laisser vide pour une livraison.                                                                                                             |
| **Urgence**                                       | Uniquement pour une livraison. La valeur doit faire partie des valeurs du champ Urgence paramétrées dans Paramétrage > Track > Demande de transport.                          |

Une ligne est refusée (et le motif est indiqué dans le fichier de trace) dans les cas suivants :

* un champ obligatoire est vide ou le Type demande n'est ni « Livraison » ni « Collecte » ;
* le N° dossier n'est pas numérique ;
* le Service ne correspond à aucun type de livraison ou de collecte (selon le Type demande) ;
* la date est absente, invalide ou ne respecte pas le format attendu ;
* une urgence est renseignée pour une collecte, ou ne fait pas partie des valeurs paramétrées ;
* la date de collecte est dans le passé ;
* une collecte est déjà en cours pour le même N° dossier ;
* l'adresse n'a pas pu être trouvée.

{% hint style="info" %}
Comme pour une création manuelle, une livraison hors des jours et horaires travaillés ou dans le passé est directement « Sous-traitée », et une demande prévue le jour même est « En attente de validation ». Un mail est alors envoyé pour les livraisons du jour.
{% endhint %}
