---
description: >-
  Générer automatiquement des demandes d'achat à partir des règles de stockage
  des références, après inventaire RFID.
---

# Planification

**Chemin :** Paramétrage › Stock › Demandes › Achats - Planification

### Principe

Sur une référence (**Stock › Références › Article de référence**), chaque règle de stockage sur un emplacement porte :

* une **Quantité de sécurité** : quantité minimale d'articles disponibles en stock ;
* une **Quantité de conditionnement** : nombre d'articles par conditionnement.

Après un inventaire, si la quantité disponible passe sous la quantité de sécurité, une demande d'achat est générée.

<figure><img src="../../../../.gitbook/assets/image (6) (1).png" alt=""><figcaption></figcaption></figure>

### Planifier un achat

Cliquez sur **Planifier un achat** et renseignez :

* **Zone\*** : zone(s) à inventorier ;
* **Fournisseur\*** des références de la zone ;
* **Demandeur\*** ;
* **Statut\*** de la demande d'achat créée ;
* **Objet du mail\*** ;
* **Fréquence** : une fois, chaque heure, chaque jour, chaque semaine ou chaque mois.

<figure><img src="../../../../.gitbook/assets/image (7) (1).png" alt=""><figcaption></figcaption></figure>

### Email reçu

Pour chaque demande d'achat planifiée, un email liste les références à réapprovisionner : **Référence**, **Libellé**, **Emplacement (Zone)**, **Quantité demandée** et **Quantité en stock**.

<details>

<summary>Règle de calcul</summary>

La **quantité demandée** est égale à la quantité de sécurité du couple référence / emplacement.

Calcul : (somme des quantités des articles de la référence sur l'emplacement) − (quantité maximale d'un article inventorié parmi ces articles).

* Résultat **supérieur ou égal** à la quantité de sécurité : pas de demande d'achat.
* Résultat **inférieur** à la quantité de sécurité : une demande d'achat est générée.

Si la référence est sur plusieurs emplacements, la quantité demandée est la somme des quantités de sécurité des couples référence / emplacement à réapprovisionner.

<figure><img src="../../../../.gitbook/assets/image (93).png" alt=""><figcaption><p>Exemple</p></figcaption></figure>

</details>
