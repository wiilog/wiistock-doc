# Wiilog/Follow GT : Les principes fondamentaux



<figure><img src=".gitbook/assets/site industriel-vidéo (1).jpg" alt=""><figcaption></figcaption></figure>

## Lexique

{% hint style="info" %}
Pendant nos échanges, il est primordial que nous utilisions un vocabulaire cohérent afin d'assurer une compréhension mutuelle. Pour ce faire, nous adopterons le terme "interface web" ou "supervision" lorsque nous discuterons de l'utilisation de Follow-GT sur un ordinateur. En revanche, nous utiliserons le terme "environnement nomade" pour désigner l'utilisation de Follow-GT sur un terminal Android. Cette uniformité dans notre terminologie facilitera grandement la communication et évitera toute confusion.&#x20;
{% endhint %}

En ce qui concerne les instances (les pages web qui donnent accès à l'application et à ses fonctionnalités), celles-ci sont créées par Wiilog. Chacun aura à sa disposition une instance de production ainsi qu'une instance de recette. Vous pourrez aisément identifier l'environnement en examinant l'URL de l'instance. Les instances de production comportent le terme "prod" dans leur URL, tandis que les instances de recette contiennent "rec".&#x20;

L'URL est structurée de la manière suivante : **https://{nom de l'instance}-{environnement}.follow-gt.fr**. Dans ce contexte, le terme "environnement" peut prendre les valeurs "prod" pour la production ou "rec" pour la recette.&#x20;

## Follow-gt c’est quoi ?&#x20;

&#x20;\
Follow-gt est une application que vous allez utiliser pour tracer stocker ou gérer vos opérations de livraison au dernier kilomètre.&#x20;

Pour ce faire vous pourrez utiliser selon vos besoins un ou plusieurs modules de l’application.&#x20;

* **Traçabilité** : Ce module vous permet de localiser et d'identifier vos produits. Vous pouvez également ajouter vos informations et règles métiers associés pour une gestion optimale.
* **Stock** : Le module Stock offre une solution complète pour gérer l'ensemble du processus de stockage, de la réception à la livraison sur les lignes de production. Il simplifie la préparation des commandes et leur expédition, tout en optimisant les mouvements de marchandises. Cette approche vise à améliorer l'efficacité et la précision des opérations de stockage et de distribution, renforçant ainsi la performance globale de la chaîne logistique.&#x20;
* **Track** : Le module Track offre une solution complète pour la gestion des opérations de livraison. Il vous permet de localiser vos transports, de les acheminer de manière optimale, tout en vous permettant de consulter en temps réel l'avancement de ces opérations. En utilisant ce module, vous pourrez suivre et contrôler l'état de vos transports de façon précise et efficace. Il facilite également la gestion des rendez-vous et permet de mettre en place des workflows adaptés à vos besoins spécifiques. Cela contribue à une gestion globale et optimisée de vos opérations de livraison, améliorant ainsi votre efficacité opérationnelle. <br>

## Instances de Production et de Recette dans l'Écosystème de l'Application

Les instances de production et de recette sont des environnements distincts au sein d'une application ou d'un système informatique, conçus pour différents stades du processus de développement et de déploiement. Leur rôle principal est de garantir la stabilité, la qualité et la performance des fonctionnalités avant leur mise en production pour les utilisateurs finaux.

### Comprendre leur Fonctionnement et leur Rôle

Les instances de production et de recette constituent des environnements essentiels dans le cycle de développement et de déploiement d'une application. Leur rôle fondamental est d'assurer que les nouvelles fonctionnalités et les mises à jour répondent aux normes de qualité et de performance requises avant d'être déployées auprès des utilisateurs finaux.&#x20;

### Instance de Production  &#x20;

L'instance de production est l'environnement dans lequel l'application est accessible aux utilisateurs finaux ou clients. C'est l'endroit où les utilisateurs interagissent avec l'application pour accomplir leurs tâches et atteindre leurs objectifs. Les mises à jour déployées dans l'instance de production doivent être soigneusement testées et validées dans l'instance de recette avant d'être diffusées. L'objectif principal de l'instance de production est de fournir une expérience fluide et fiable aux utilisateurs tout en minimisant les interruptions et les dysfonctionnements.&#x20;

### Instance de Recette  &#x20;

L'instance de recette, quant à elle, sert de terrain d'essai pour évaluer et valider les nouvelles fonctionnalités, les corrections de bugs et les améliorations avant qu'elles ne soient introduites dans l'instance de production. C'est un environnement contrôlé où les tests complets sont effectués pour s'assurer que les changements n'affectent pas négativement les performances de l'application ou ne provoquent pas de dysfonctionnements. Cette phase de test rigoureux permet de repérer et de résoudre les problèmes avant qu'ils n'impactent les utilisateurs finaux.&#x20;

### Fonctionnement  &#x20;

Lorsque de nouvelles fonctionnalités ou mises à jour sont développées, elles sont d'abord implémentées dans l'instance de recette. Les tests approfondis sont alors effectués, y compris les scénarios d'utilisation réelle, pour identifier tout problème potentiel. Une fois que les tests sont satisfaisants, les changements sont déployés dans l'instance de production, où ils deviennent accessibles aux utilisateurs finaux.&#x20;

### Importance &#x20;

La distinction entre les instances de production et de recette est cruciale pour maintenir la stabilité et la fiabilité de l'application. En testant les nouvelles fonctionnalités dans l'instance de recette, les équipes de développement et de qualité s'assurent que les utilisateurs finaux bénéficieront d'une expérience sans faille. Les instances de recette jouent un rôle vital dans l'amélioration continue de l'application en détectant et en corrigeant les problèmes potentiels avant qu'ils ne parviennent aux utilisateurs finaux.&#x20;

## En résumé  &#x20;

Les instances de production et de recette sont des éléments clés du processus de développement et de déploiement, garantissant une expérience utilisateur de haute qualité et la stabilité de l'application. Leur interaction coordonnée contribue à l'efficacité, à la fiabilité et à l'innovation continue dans le domaine des applications professionnelles.&#x20;
