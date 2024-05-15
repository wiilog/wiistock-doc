---
description: >-
  Dans la continuité du fonctionnel RFID, la planification des demandes d’achat
  a été mis en place. Le principe émane des règles des stockage défini sur les
  références.
---

# Achat planifié

## Règles de stockage

Dans **Stock | Référence | Article de référence,** lorsqu’on attribue une règle de stockage à une référence sur un emplacement, on saisit une <mark style="background-color:blue;">**Quantité de sécurité**</mark> qui **correspond à la quantité minimale d’articles disponibles en stock** et une <mark style="background-color:blue;">**Quantité de conditionnement**</mark> qui **représente le nombre d’article contenu dans un conditionnemen**t. La quantité de sécurité va permettre de déterminer un **seuil de quantité disponible qui ne doit pas être inférieur**, auquel cas il déclenchera une demande d’achat planifiée.

<figure><img src="../../../../.gitbook/assets/image (6) (1).png" alt=""><figcaption></figcaption></figure>

## Paramétrage | Stock | Demande | Achats - Planification

Le fonctionnel de demande d’achat planifié repose donc sur des **règles de déclenchement par référence après avoir effectué un inventaire.**&#x20;

Dans la modale de planification il vous faudra remplir les informations suivantes : &#x20;

* le ou les **Zones\*** que vous allez inventorier
* **Fournisseur\*** des références présentes sur la zone,&#x20;
* **Statut\***
* **Objet du mail\***
* **Fréquence**

<figure><img src="../../../../.gitbook/assets/image (7) (1).png" alt=""><figcaption></figcaption></figure>

Pour chaque demande d’achat planifié vous recevrez un **email** concernant votre demande d'achat avec un tableau des références à réapprovisionner et le détail de celle-ci :&#x20;

* &#x20;**Référence** à réapprovisionner
* **Libellé** de la référence
* **Emplacement (Zone)** de la référence
* **Quantité demandée**
* **Quantité en stock**&#x20;

**La Quantité demandée que vous ferez appel à l’issu de votre demande d’achat correspondra à la Quantité de sécurité définie sur le couple référence sur emplacement.**

La règle de gestion pour ajouter des référence repose sur ce calcul :

·       **\[(Somme de toutes quantité article d’une référence sur un emplacement) – (La quantité maximum d’un article inventorié parmi toutes les quantités)] > Quantité de sécurité**. _Pas de demande d’achat générée._

·        **\[(Somme de toutes quantité article d’une référence sur un emplacement) – (La quantité maximum d’un article inventorié parmi toutes les quantités)] = Quantité de sécurité.** _Pas de demande d’achat générée._

·      **\[(Somme de toutes quantité article d’une référence sur un emplacement) – (La quantité maximum d’un article inventorié parmi toutes les quantités)] < Quantité de sécurité.** _Génération d’une demande d’achat._

**Si la référence est présente sur plusieurs emplacements, la quantité demandée pour une demande d’achat sera la somme des quantités de sécurité par couple référence sur emplacement** qui nécessitent un réapprovisionnement.

**Exemple :**&#x20;

<figure><img src="../../../../.gitbook/assets/image (93).png" alt=""><figcaption></figcaption></figure>
