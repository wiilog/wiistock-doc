---
description: Champs fixes de l'entête et des lignes des demandes de livraison.
---

# Champs fixes

**Chemin :** Paramétrage › Stock › Demandes › Livraisons - Champs fixes

Les champs fixes ne peuvent être ni ajoutés ni supprimés. Le paramétrage se fait en deux parties.

### Entête

Pour chaque champ (Date attendue, Destination, Type, Destinataire, Projet), cochez **Afficher** / **Obligatoire** sur le formulaire de création et d'édition, et **Afficher** sur les filtres (case grisée = non disponible). Le champ **Projet** va chercher ses valeurs dans le référentiel projet.

Les champs **soulignés** se paramètrent en cliquant dessus :

* **Destination** : emplacement par défaut **par type** de livraison. Ajoutez autant d'associations _Type - Emplacement_ que de types ;
* **Type** : type de livraison proposé par défaut ;
* **Destinataire** : destinataire par défaut, ou option **Le destinataire est égal au demandeur**.

<figure><img src="../../../../.gitbook/assets/image (125).png" alt=""><figcaption><p>Emplacement par défaut pour un type de demande de livraison</p></figcaption></figure>

### Références/Articles (tableau d'ajout)

Pour les champs des lignes (Projet, Commentaire, Remarques) :

* **Afficher** et **Obligatoire** ;
* **Afficher sous condition** (Projet) : le champ n'apparaît que si un champ fixe (ex. : **Type**) a une **Valeur** donnée.

Cliquez sur **Enregistrer** pour valider.

<figure><img src="../../../../.gitbook/assets/image (123).png" alt=""><figcaption><p>Les champs fixes des demandes de livraison</p></figcaption></figure>
