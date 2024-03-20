---
description: 27/02/2023
---

# Mise à jour - Projet Signatures Groupées

Cette version contient des nouvelles fonctionnalités de signature groupée. Une évolution des acheminements a été mise en place. Cette version contient :&#x20;

* _Nomade | Demande | Création acheminement_ : Faire une **demande d’acheminement depuis le nomade** &#x20;
* &#x20;_Nomade | Demande | Acheminement_ : **Générer une lettre de voiture depuis le nomade** via à un formulaire&#x20;
* _Nomade - Web| Demande | Acheminement_ : Ajouter une référence existante à une UL, possibilité de **pré remplir les champs d’informations d’une référence déjà existante**&#x20;
* _Nomade – Web | Demande | Acheminement_ : **Créer une nouvelle référence** à une UL &#x20;
* _Nomade | Traçabilité | Acheminements | Signature groupée_ : **Sélectionner des acheminements via le scan d’une unité logistique** dans un acheminement. Le scan d’une UL d’un acheminement permettra de sélectionner toutes les UL présentes dans le même acheminement et donc l’acheminement en lui-même.
* _Web | Traçabilité | Acheminements | Signature groupée_ : **Sélectionner plusieurs demandes d’acheminement pour faire une signature groupée** via l'association d'un utilisateur et d'un code signataire. Dans le cas où vous avez besoin d’une validation de plusieurs acheminements à l’envoie ou en livraison par autrui, cette fonctionnalité vous évitera de valider un par un chaque acheminement.
* _Paramétrage | Utilisateur_ : **Nouveau champ Code signataire** pour faire des signatures groupées d’acheminement. Ce code signataire est semblable à un mot de passe avec minium 4 caractères et il est associé à l’utilisateur.
* _Référentiel | Emplacement_ : **Nouvelle colonne Signataire (multi signataire),** un ou plusieurs utilisateurs peuvent être associés à un emplacement. Ce qui signifie que pour la fonctionnalité Signature groupée, une demande d’acheminement ne pourra être signée que par le(s) signataire(s) associé(s) à l’emplacement. Les signataires pourront également **recevoir un compte rendu par mail du détail d’un acheminement.**
* _Stock | Article_ : **Nouvelle partie Description**, avec des nouveaux champs (Matériel hors format, ADR, Code fabricant). Possibilité de **calculer le volume d’un article** en entrant les champs longueur, largeur, hauteur. Fonctionnalité également présente à l’étape Demande | Acheminement | Ajouter un référence à une UL : création d’une référence.
* _Paramétrage | Traçabilité | Acheminements | Statut_ : Nouvelle colonnes :&#x20;
  * **Signature groupée** qui prend comme valeurs : vide ; prise ou dépose. En fonction de l’état du statut, on peut définir si on est en processus de prise ou de dépose.&#x20;
  * **Envoi compte rendu** par mail avec le format en PDF en pièce jointe
  * **Couleur signature groupée** :  Possibilité d’avoir des entêtes avec des couleurs différentes pour les demandes d’acheminements en fonction des statuts sur la partie _Nomade |Traçabilité | Demande | Acheminement | Signature groupée_&#x20;
  * **Commentaire obligatoire** (uniquement pour la signature groupée)&#x20;
* _Paramétrage | Modèles de document |Acheminement | Compte rendu_ : Possibilité de recevoir par mail, une **version PDF d’un « compte rendu » via un modèle word**, avec le détail d’un acheminement en fonction du paramétrage du statut. &#x20;
* _Demande | Acheminent | Urgence_ : Si la notion d’urgence est attribuée à un acheminement, l’objet du compte rendu par mail différera d’un compte rendu sans urgence avec pour **objet d’email « Urgence »**
