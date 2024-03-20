---
description: Mise en production du 22/11/2023
---

# Mise à jour - Acheminements - Mouvements - Rôles & Association BR

### Amélioration des mouvements et report des urgences

* MOUVEMENTS : Ce projet vous permet de visualiser via un détrompeur les unités logistiques qui n'ont pas été déposées sur votre emplacement de prise. Cela vous permettra de distinguer des erreurs potentielles de scan de QR code.

Pour utiliser ce détrompeur, vous devez activer le paramétrage sur la page **"Paramétrage | Trace | Mouvements | Configurations"** .

_EX : Je réalise une prise de mon unité logistique, j'ai un message d'information pour me prévenir que cette unité logistique n'est pas réellement sur cet emplacement donc votre traçabilité n'est peut être pas correcte._

* ARRIVAGES UL / URGENCES : Ce projet vous permet également de confirmer lors d'un arrivage UL que l'élément porteur de l'urgence est présent dans l'arrivage.

Pour utiliser cette modale supplémentaire, vous devez activer le paramétrage sur la page **"Paramétrages | Trace | Urgences | Configurations - Afficher un pop-up de confirmation de réception de l'urgence via numéro de poste - code article interne et code article fournisseur".**&#x20;

_EX : une urgence est créée sur un numéro de commande. Lors de la création de mon arrivage UL, j'ai plusieurs numéros de tracking pour une seule commande. Je choisi un numéro de tracking puis je positionne un numéro de commande. Si le numéro de tracking n'est pas celui de l'urgence, je peux choisir de refuser l'urgence et de la garder active pour un autre numéro de tracking avec le même numéro de commande._&#x20;

### Amélioration des formulaires de demande d'acheminement&#x20;

* Vous pouvez choisir, pour chaque type créé, les champs fixes que vous souhaitez afficher et remplir dans votre demande. Depuis la page **Paramétrages | Trace | Acheminements | Champs fixes**, vous pouvez maintenant sélectionner le type que vous voulez paramétrer puis cocher les cases pour lesquelles vous voulez faire apparaitre les champs fixes proposés.&#x20;
* Vous pouvez sélectionner la date sur laquelle vous voulez positionner votre filtre sur la page **Demande | Acheminement.** EX : Date de création, date de traitement, date de validation, etc.
* Vous pouvez sélectionner le "type" d'acheminement sur votre filtre de la page **Demande | Acheminement**, qui filtrera le filtre "statut".

### Meilleure segmentation des fonctionnalités nomades sur les rôles

* Les rôles ont été améliorés pour segmenter les fonctionnalités nomades et améliorer les temps de synchronisation. Vous pouvez maintenant :&#x20;
  * Sélectionner dans vos rôles les menus que vous souhaitez afficher sur nomade.

### EDD&#x20;

Pour la mise à jour de l'entrepôt de données, les changements peuvent être légèrement différents sur le renommage en fonction de la version que vous utilisez. Le principe est que la table touchée sera la bonne, il faudra simplement ajouter ou supprimer un pluriel sur la colonne citée ci-dessous. &#x20;

* Mise à jour de la table "dw\_arrivage", la colonne "destinataire" devient "destinataires"
* Mise à jour de la table "dw\_association\_br", la colonne "codes\_ul" devient "code\_ul".
