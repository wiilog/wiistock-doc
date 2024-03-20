# Stock | Inventaire RFID

## Configuration RFID

Pour préparer votre inventaire en RFID, nous avons intégré un espace de Configuration dans **Paramétrage | Stock | Inventaire**, dédié à la RFID.

<figure><img src="../../.gitbook/assets/image (32).png" alt=""><figcaption></figcaption></figure>

Il est important de remplir le <mark style="background-color:blue;">**Préfixe**</mark>** de tag RFID** visible sur vos étiquettes RFID transmises par votre fournisseur, cela permet au lecteur de filtrer les résultat suivant ce préfixe.

On peut également saisir une <mark style="background-color:blue;">**Tranche pourcentage KPI**</mark> **mettant en avant les emplacements à rescanner en RFID.** Par exemple, si l’on détermine une tranche entre 0% et 70%, lors du premier balayage RFID de votre inventaire il apparaîtra uniquement le pourcentage de chaque emplacement ayant un indicateur inférieur à 70%, c'est à dire pour lesquelles il manque des articles.

Une fois la configuration RFID effectuée, il vous faut préparer vos zones, emplacements et références.

## Article sur emplacement

L’application d’un inventaire RFID sur notre application s’applique sur **un inventaire de type Article sur Emplacement**. Il s’appuie sur le **principe de règle de stockage** appelé également **couple référence sur emplacement.**&#x20;

Le fait de définir un couple référence sur emplacement, c’est-à-dire une **référence indiquée présente sur un emplacement ciblé**,  apportera une bonne qualité du travail de l’inventaire. Lors de votre balayage RFID pour un inventaire, s’il manque des articles, dans l’affichage de votre résultat d’inventaire on verra apparaître la liste des références manquantes qu’on doit retrouver sur cette emplacement. L’opérateur se verra obliger à vérifier et éventuellement re scanner l’emplacement. Après re scan, dans le cas où les références sont toujours manquantes, lorsque vous validerez votre inventaire, les **articles absents passeront du statut disponible à consommé**, car cela signifie qu’ils ont été prélevés pour usage.

## Etape 1 : Créer des zones et des emplacements

Dans un premier temps, dans **Référentiel | Emplacement**, il vous faut **créer des zones** et pour chacune, il vous faudra indiquer l’<mark style="background-color:blue;">**Indicateur d'inventaire sur emplacement RFID**</mark>. L’objectif de l’inventaire c’est d’avoir un indicateur d’emplacement à 100% ou plus. S’il apparaît 100% cela signifie qu’il y a au moins un article en moyenne par règle de stockage de cette emplacement avec un indicateur d’inventaire égal à 1. Si l’on augmente l’inventaire, on augmente alors la moyenne d’articles par règle de stockage.&#x20;

<figure><img src="../../.gitbook/assets/image (31).png" alt="" width="241"><figcaption></figcaption></figure>

Après avoir défini vos zones il vous faut ajouter un ou plusieurs emplacements sur celles-ci.

## Etape 2 : Définir des règles de stockage

Passons maintenant à l’étape d’établissement de règle de stockage Référence sur emplacement. Lorsque vous créer vos articles en RFID, ils sont donc associés à une référence. Pour chaque référence, en passant par la modification de sa fiche référence dans **Stock | Article de référence | Modifier**, il y a un encart **Règles de stockage** avec trois champs obligatoires :&#x20;

* Emplacement
* Quantité de sécurité&#x20;
* Quantité de conditionnement. &#x20;

L’inscription d’une règle de stockage sur une référence n’implique pas que le fonctionnel des inventaires mais également le fonctionnel de **Demandes d’achats planifiée**s (_nous en reparleront un peu plus tard_). Le champ <mark style="background-color:blue;">**Emplacement**</mark> fait appel au **Référentiel | Emplacemen**t, et donc **atteste que cette référence doit être présente sur cet emplacement défini**. **Une référence peut avoir plusieurs règles de stockage**, par conséquent elle peut être présente sur plusieurs emplacements. Définir une quantité de sécurité et une quantité de conditionnement permet de définir un seuil de quantité qui une fois est inférieure à celui défini, déclenche une demande d’achat au fournisseur.

La saisie des règles de stockage peut se faire **manuellement** ou **via l’import de vos références** dans **Paramétrage | Données | Import & mises à jour.**

<figure><img src="../../.gitbook/assets/image (22).png" alt=""><figcaption></figcaption></figure>

## Etape 3 : Créer une mission d'inventaire

Deux possibilités pour créer des missions d’inventaire :

### Stock | Inventaire - Ajouter une mission

En passant par la modale <mark style="background-color:blue;">**Ajouter une mission**</mark>, il vous faut remplir les champs standards obligatoires :&#x20;

* **Libellé\***
* **Date prévue de début\***&#x20;
* **Date prévue de fin\***&#x20;
* **Description\***
* **Demandeur\*** : Par défaut c'est complété par l'utilisateur connecté.&#x20;
* **Type de mission\*** : Sélectionner <mark style="background-color:blue;">**Aticle sur emplacement**</mark>.

<figure><img src="../../.gitbook/assets/image (14).png" alt="" width="283"><figcaption></figcaption></figure>

<figure><img src="../../.gitbook/assets/image (11).png" alt="" width="375"><figcaption></figcaption></figure>

Passer cette étape, vous pouvez soit ajouter des zones à inventorier et/ou sélectionner des emplacements. Puis cliquer sur <mark style="background-color:blue;">**Enregistrer**</mark>, votre mission d’inventaire est créée, dans **Stock | Inventaire** vous pouvez voir apparaître le **Pourcentage du taux d’avancement** de votre mission et entrer dans le détail de celle-ci qui affiche par ligne les emplacements à inventorier.

Sur votre TC, dans Stock | Inventaire | Mission, la mission d’inventaire créer sur le web sera visible et prête à être exécuter dans le cas où vous avez paramétrer une date de début imminente.

### Paramétrage | Stock | Inventaires | Planification d'inventaire

En passant par la modale <mark style="background-color:blue;">**Planificateur d'inventaire**</mark>, vous aurez également la possibilité de planifier vos missions d’inventaire de type Article sur emplacement (_le type Quantité article existait déjà_).

<figure><img src="../../.gitbook/assets/image (15).png" alt="" width="375"><figcaption></figcaption></figure>

## Etape 4 : L'inventaire

&#x20;

Exemple : Nous avons créé la zone « Zone 3.0 » avec un emplacement « Bordeaux sud » sur lequel nous avons 4 références qui ont une règle de stockage : 8171-011 ; 3809-922 ; 9047.

Sur ces trois références, un article RFID a été créé pour chaque :

\-        ART230600000056 / Tag RFID : DLFP00001168 / Référence article : 8171-011&#x20;

\-        ART230600000055 / Tag RFID : DLFP00001165 / Référence article : 3809-922

\-        ART230600000057 / Tag RFID : DLFP00001164 / Référence article : 9047

Ayant été tout juste créé ils ont fait donc l’objet d’**une dépose** sur l'emplacement Bordeaux sud, d’une **entrée de stock**, et sont au **statut disponible**.

### L'inventaire sur nomade

Dans le menu **Stock | Inventaire**, appuyer sur <mark style="background-color:blue;">**Mission**</mark>, et sélectionner la mission concernée et l'emplacement à inventorier. Dans cet exemple si, il n'y a qu'un seul emplacement sur la Zone 3.0, l'emplacement Bordeaux sud.&#x20;

<figure><img src="../../.gitbook/assets/image (86).png" alt=""><figcaption></figcaption></figure>

Suite à la sélection vous serez dirigé sur l’écran **Stock | Inventaire** avec une page vierge du résultat de l'inventaire.&#x20;

<figure><img src="../../.gitbook/assets/image (88).png" alt=""><figcaption></figcaption></figure>

Dès lors de l’appuie de la gachette sur votre lecteur RFD40 ou en appuyant sur le bouton ![](<../../.gitbook/assets/image (87).png>) <mark style="background-color:blue;">**Play**</mark>, votre inventaire démarre. Au relâchement de la gachette ou en appuyant sur pause, les résultats s’afficheront.

#### Premier cas&#x20;

<figure><img src="../../.gitbook/assets/image (89).png" alt=""><figcaption></figcaption></figure>

Pour rappel, nous avons inventorié l’emplacement Bordeaux sud sur lequel il y trois articles de trois références différentes. Premier cas de figure, nous avons isolé les 3 articles (étiquettes RFID). Voici le résultat d’inventaire, plusieurs informations sont visibles :

\-        0 objet scanné : Signifie que votre lecteur n’as pas trouvé d’articles assignés à cet emplacement

\-        Attention références manquantes : 3 références sont manquantes sur cet emplacement

\-        Indicateur d’emplacement avant validation : Indique le pourcentage d’articles présents sur cet emplacement, ici 0% car aucuns articles n'a été détectés.

#### Second cas

<figure><img src="../../.gitbook/assets/image (90).png" alt=""><figcaption></figcaption></figure>

Nous avons rappuyé sur la gachette et intégré deux articles (étiquettes RFID). Le résultat d’inventaire s'est mis à jour :

\-        2 objet scannés : Signifie que le lecteur a trouvé deux articles assignés à cet emplacement

\-        Attention références manquantes : 1 référence manquante sur cet emplacement

\-        Indicateur d’emplacement avant validation : 51% de présence d’article sur cet emplacement. Voici le calcul de cette indicateur d’emplacement qui s’appuie sur les couples référence / emplacement :&#x20;

**Nombre d’articles trouvés / ( Nombre de couple \* Indicateur emplacement RFID de la zone) \* 100**

\= 2 / (3\*1.3) \* 100

\= 51%

#### Troisième cas

Après pression sur la gachette, et nous avons intégré le troisième article (étiquette RFID). Le résultat d’inventaire s'est mis à jour :

\-        3 objet scannés : Signifie que le lecteur a trouvé trois articles assignés à cet emplacement

\-        Attention références manquantes : 0 référence manquante sur cet emplacement

\-        Indicateur d’emplacement avant validation : 76% de présence d’article sur cet emplacement. = 3 / (3\*1.3) \* 100

\= 76 %

Puis appuyer sur <mark style="background-color:blue;">**Valider**</mark>, et vous pourrez retrouver votre résultat d'inventaire sur le web dans **Stock | Inventaire** avec un **taux d’avancement** à 100%. Dans le détail de celle- ci par ligne d’emplacement vous pourrez retrouver l’indicateur d’emplacement, ainsi que la **liste des articles scannés**.

<figure><img src="../../.gitbook/assets/image (92).png" alt=""><figcaption></figcaption></figure>

#### Quatrième cas

Exemple : Nous effectuons un second inventaire RFID sur nomade, et à l’issu de celui-ci, il manque des articles, nous validons la mission comme étant terminée. Le résultat de cet inventaire implique que **les articles ont été épuisés**, et passent donc du **statut disponible à consomm**é.

Après réapprovisionnement, si l'on effectue un nouvel inventaire, les articles seront pris en compte et repasseront au **statut disponible**.
