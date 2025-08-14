# Configurations

## Configurations

### Création d'un acheminement

Cette section sert à paramétrer le comportement de création d'un acheminement et lors de l'ajout de colis dans un acheminement.

* **Obliger la signature groupée pour traiter les acheminements:** paramétrage à activer si vous souhaitez utiliser la fonctionnalité de Signature groupée
* **Pré-remplir la date du jour dans le champ à échéance Du et échéance Au** : même si vous n'avez pas paramétré d'afficher le champ fixe Date d'échéance sur le formulaire de création d'acheminement, la date d'échéance sera automatiquement remplie avec la date du jour, que cela soit pour la borne basse ou la borne haute des dates d'échéances
* **Ajouter le numéro d'acheminement en préfixe de l'UL lors de l'UL :** lorsque vous ajoutez un colis sur un acheminement, le colis aura automatiquement en préfixe le numéro d'acheminement
* **L'UL ajouté dans l'acheminement ne peut pas exister en base (doit être nouveau) :** lorsque vous ajouter un colis dans un acheminement, celui-ci doit être nouveau, il ne doit pas déjà être dans la liste des colis.
* **Garder la fenêtre modale ouverte après validation et vider les champs pour les rôles: rôle(s) à sélectionner** - paramétrage qui permet de garder la modale de création de l'acheminement tout le temps ouverte, de vider les champs après chaque saisie et d'attribuer ce fonctionnement uniquement à des rôles spécifiques
*   **Format du numéro d'acheminement** : Vous allez définir le format de vos numéros d'acheminement selon les choix suivants :

    * aaaammjjxxxx : année-mois-jour-numéro d'ordre
    * aaaammjjhhmmss-xxxx : "année-mois-jour-heure-minute-seconde-numéro d'ordre
    * aammjjhhmmssxx : année sur deux chiffres-mois-jour-heure-minute-seconde-numéro d'ordre



### Création de référence :&#x20;

Lors de l'ajout d'une référence à une unité logistique vous avez la possibilité de créer une référence avec des valeurs par défaut pour les champs obligatoires.

**Sélection du Type :**

* Vous devez sélectionner le type de référence à partir du menu déroulant qui vous proposera en choix les types de références déjà créées sur votre instance.

**Définition de l'État de la Référence :**

L'utilisateur doit choisir l'état de la référence parmi les options "Brouillon", "Actif" et "Inactif". Ce choix détermine si la référence est prête à être utilisée ou non.

* L'option "Brouillon" paramètre l'état de la référence créée dans l'acheminement en tant que brouillon. Cette référence devra être validée par un utilisateur possédant les droits de validation avant de pouvoir être manipulée.
* L'option "Actif" paramètre l'état de la référence créée dans l'acheminement en tant qu'active dès sa création. Cette référence pourra être manipulée directement par l'utilisateur.
* L'option "Inactif" paramètre l'état de la référence créée dans l'acheminement en tant qu'inactive. Cette référence ne pourra pas être manipulée avant qu'un utilisateur possédant les droits nécessaires ne la passe en état actif.

**Gestion de la Quantité :**

* L'utilisateur doit définir comment la quantité de la référence créée dans l'acheminement sera gérée. Les options disponibles sont "Référence" et "Article".



### **Filtres via champs fixes sur la page demande**

Dans ce champ vous allez pouvoir paramétrer les filtres sur les champs fixes qui seront utilisables sur la page Demande | Acheminement  (Liste).



### Validation d'un acheminement

Le paramètre "Validation d'un acheminement => Créer automatiquement un mouvement de dépose sur l'emplacement de prise de l'acheminement à sa validation pour les types" permet de définir les types d'acheminement pour lesquels un mouvement de dépose sera automatiquement créé sur l'emplacement de prise de l'acheminement à sa validation.



### Bon de surconsommation

**Logo du bon de surconsommation**

\
Le paramètre "Logo des bons de surconsommation" vous permet de définir le logo qui sera affiché en en-tête des bons de surconsommation générés par Wiilog/Follow GT. Pour cela, vous devez sélectionner une image dans l'un des formats de fichiers suivants : .png, .jpeg, .jpg, .svg ou .gif.

Il est important de noter que l'image ne doit pas dépasser la taille maximale de 1000px\*1000px



## Groupage

L'option : Dégroupage automatique à la dépose sur l'emplacement de dépose de l'acheminement pour les types : choisir les types

permet de dégrouper les UL d'un groupe lorsqu'il est déposé sur un emplacement de dépose d'acheminement de type "sélectionner le type que vous souhaitez".

