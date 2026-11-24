---
description: Liste des tables de l'entrepôt de données (EDD) et de leurs colonnes.
---

# Dictionnaire des tables

Cette page complète la [Cartographie des données](cartographie-des-donnees.md). Elle liste les tables disponibles pour vos outils de BI (Power BI, etc.).

## Arrivages, unités logistiques et mouvements

| Table | Contenu | Colonnes |
| --- | --- | --- |
| `dw_arrivage_camion` | Arrivages camion, numéros de tracking et réserves. Un camion peut apparaître sur plusieurs lignes. | `id`, `no_arrivage_camion`, `no_tracking`, `date_creation`, `transporteur`, `chauffeur`, `immatriculation`, `emplacement`, `cree_par_id`, `nb_tracking_total`, `reserve_generale`, `reserve_quantite`, `reserve_tracking_type` |
| `dw_numero_tracking` | Lignes de tracking camion, réserve qualité, retard calculé selon le paramétrage et numéro d'arrivage UL associé. | `no_tracking`, `no_arrivage_camion`, `reserve_qualite`, `retard`, `no_arrivage_UL` |
| `dw_arrivage` | Arrivages d'unités logistiques (UL), transport, statut, réception et camion liés. | `id`, `no_arrivage`, `date`, `nb_ul`, `fournisseur`, `transporteur`, `chauffeur`, `no_tracking_transporteur`, `no_commande_bl`, `type`, `urgence`, `douane`, `congele`, `statut`, `commentaire`, `cree_par_id`, `numero_projet`, `business_unit`, `reception_id`, `no_arrivage_camion` |
| `dw_arrivage_champs_libres` | Champs libres renseignés sur les arrivages. | `arrivage_id`, `libelle`, `valeur` |
| `dw_arrivage_nature_ul` | Nature et quantité des UL rattachées à un arrivage. | `arrivage_id`, `nature_ul`, `quantite_ul` |
| `dw_indicateur_arrivage` | Indicateurs globaux sur les arrivages ; pas de colonne par arrivage ni de date. | `nb_fournisseurs_differents`, `pourcentage_urgence`, `analyse_destinataire` |
| `dw_unite_logistique` | UL, nature, provenance et articles contenus. Un `id` peut se répéter si plusieurs articles ou acheminements sont associés à la même UL. | `id`, `code_unite_logistique`, `nature`, `quantite`, `projet`, `acheminement_id`, `arrivage_id`, `nb_articles_contenus`, `code_barre_article`, `date_creation` |
| `dw_tracabilite` | Mouvements de traçabilité, avec leurs rattachements lorsqu'ils existent. | `mouvement_traca_id`, `date_mouvement`, `unite_logistique_id`, `code_ul`, `article_id`, `code_barre_article`, `type_mouvement`, `groupe`, `quantite_mouvement`, `emplacement_mouvement`, `operateur_id`, `arrivage_id`, `acheminement_id`, `reception_id`, `tournee_ligne_id` |
| `dw_tracabilite_champs_libres` | Champs libres renseignés sur les mouvements de traçabilité. | `mouvement_traca_id`, `libelle`, `valeur` |
| `dw_association_br` | Associations entre un code UL et un numéro de bon de réception. | `date`, `code_ul`, `reception`, `cree_par_id` |

## Acheminements, services et tournées Trace

| Table | Contenu | Colonnes |
| --- | --- | --- |
| `dw_acheminement` | Demandes d'acheminement, prise/dépose, suivi et détail par UL et référence. Un `id` peut apparaître sur plusieurs lignes. | `id`, `numero`, `date_creation`, `date_validation`, `date_traitement`, `date_echeance_debut`, `date_echeance_fin`, `type`, `transporteur`, `numero_tracking_transporteur`, `numero_commande`, `demandeur_id`, `code_ul`, `quantite_ul`, `quantite_a_acheminer`, `nature_ul`, `longueur_ul`, `largeur_ul`, `hauteur_ul`, `emplacement_prise`, `emplacement_depose`, `destination`, `nb_ul`, `statut`, `operateur_id`, `traite_par_id`, `cree_par_id`, `dernier_emplacement`, `date_dernier_mouvement`, `urgence`, `numero_projet`, `business_unit`, `delais_traitement_attendu`, `delais_traitement_validation`, `reference`, `quantite_reference`, `numero_lot`, `numero_serie`, `numero_plombage_scelle`, `adr`, `commentaire`, `nom_client`, `adresse_client`, `telephone_client`, `destinataire_client`, `types_documents_associes`, `unite_logistique_id`, `reference_id`, `emplacement_prise_id`, `emplacement_depose_id` |
| `dw_acheminement_champs_libres` | Champs libres des acheminements. | `acheminement_id`, `libelle`, `valeur` |
| `dw_acheminement_statut` | Historique des statuts d'acheminement et signataires. `id` désigne la demande, pas l'événement. | `id`, `statut`, `date_statut`, `signataire_enlevement_id`, `signataire_livraison_id`, `initie_par_id` |
| `dw_service` | Demandes de service, dates, statut et nombre d'opérations réalisées. | `id`, `type`, `objet`, `demandeur_id`, `date_creation`, `date_attendue`, `date_realisation`, `operateur_id`, `emplacement_prise`, `emplacement_depose`, `numero`, `statut`, `urgence`, `delais_traitement_attendu`, `delais_traitement_validation`, `nombre_operations_realisees` |
| `dw_service_champs_libres` | Champs libres des demandes de service. | `service_id`, `libelle`, `valeur` |
| `dw_service_statut` | Historique des statuts de service. `service_id` correspond à `dw_service.id` mais est déclaré en texte dans cette table. | `date_statut`, `service_id`, `numero`, `statut`, `initie_par_id` |
| `dw_tournee` | En-têtes et état des tournées de traçabilité (module Trace). | `id`, `numero`, `date_creation`, `date_attendue`, `date_traitement`, `date_dernier_statut`, `statut`, `type`, `categorie`, `creee_par_id`, `demandee_par_id`, `emplacement_en_cours`, `urgence`, `commentaire` |
| `dw_tournee_ligne` | Emplacements et actions d'une tournée, dans l'ordre des étapes. Une étape peut porter plusieurs actions. | `id`, `tournee_id`, `emplacement_id`, `ordre`, `mouvement_traca_id`, `litige_id` |
| `dw_tournee_statut` | Historique des statuts de tournée ; le script exporte le code du statut. | `tournee_id`, `statut`, `date_statut`, `initie_par_id` |
| `dw_tournee_champs_libres` | Champs libres des tournées. | `tournee_id`, `libelle`, `valeur` |

## Qualité et urgences

| Table | Contenu | Colonnes |
| --- | --- | --- |
| `dw_litige` | Litiges et dernier statut, avec les UL, articles ou étapes de tournée concernés. | `litige_id`, `numero`, `type`, `date_creation`, `dernier_statut`, `dernier_commentaire`, `declarant_id`, `urgence`, `numero_arrivage`, `numero_reception`, `numero_commande_bl`, `numero_ligne`, `fournisseur`, `reference`, `transporteur`, `ul_article`, `libelle_article`, `reference_article`, `quantite_article`, `motif`, `tournee_id`, `tournee_ligne_id` |
| `dw_litige_statut` | Historique des événements de litige, avec statut et commentaire. | `litige_id`, `numero`, `type`, `statut`, `date_statut`, `initie_par_id`, `commentaire` |
| `dw_urgence` | Urgences de stock et de traçabilité, règles de déclenchement et de fin, délai et dernier déclenchement. | `id`, `type`, `declencheur_urgence`, `critere_fin_urgence`, `commentaire`, `emplacement_urgence`, `debut_delais_livraison`, `fin_delais_livraison`, `date_dernier_declenchement`, `no_commande`, `code_article_interne`, `code_article_fournisseur`, `fournisseur`, `transporteur`, `quantite`, `no_tracking`, `reference_article_id`, `dernier_numero_arrivage_reception` |
| `dw_urgence_champs_libres` | Champs libres des urgences. | `urgence_id`, `libelle`, `valeur` |
| `dw_urgence_arrivage` | Liaison entre urgences de traçabilité et arrivages. | `urgence_id`, `arrivage_id` |
| `dw_urgence_reception` | Liaison entre urgences de stock et réceptions. | `urgence_id`, `reception_id` |

## Stock, demandes et ordres

| Table | Contenu | Colonnes |
| --- | --- | --- |
| `dw_reference_article` | Références, quantités, seuils, paramètres de gestion et données de stockage. | `id`, `reference`, `libelle`, `quantite_stock`, `type`, `commentaire`, `emplacement`, `seuil_securite`, `seuil_alerte`, `date_securite_stock`, `date_alerte_stock`, `prix_unitaire`, `code_barre`, `categorie_inventaire`, `gestion_stock`, `statut`, `date_dernier_inventaire`, `synchronisation_nomade`, `groupe_visibilite`, `acheteur_id`, `creee_par_id`, `date_creation`, `editee_par_id`, `date_modification`, `date_derniere_entree`, `date_derniere_sortie`, `materiel_hors_format`, `code_fabricant`, `longueur`, `largeur`, `hauteur`, `volume`, `poids`, `marchandise_dangeureuse`, `code_onu`, `classe_produit`, `code_ndp`, `derniere_reponse_stockage`, `duree_stockage_maximale`, `duree_immobilisation_maximale` |
| `dw_reference_article_champs_libres` | Champs libres des références. | `reference_article_id`, `libelle`, `valeur` |
| `dw_article` | Articles, référence associée, code-barres, lot, projet, UL et données de stockage. | `id`, `reference`, `libelle`, `code_barre`, `statut`, `quantite`, `commentaire`, `emplacement`, `date_dernier_inventaire`, `lot`, `date_entree_stock`, `date_peremption`, `code_fournisseur`, `reference_fournisseur`, `label_fournisseur`, `label_reference_fournisseur`, `projet`, `date_assignation_projet`, `code_ul`, `prix_unitaire`, `anomalie`, `tag_rfid`, `type`, `numero_commande`, `numero_bon_livraison`, `pays_origine`, `date_fabrication`, `derniere_reponse_stockage`, `duree_stockage_maximale`, `duree_immobilisation_maximale` |
| `dw_article_champs_libres` | Champs libres des articles. | `article_id`, `libelle`, `valeur` |
| `dw_projet_article` | Historique des affectations d'articles à un projet. | `article_id`, `projet`, `date_assignation` |
| `dw_inventaire` | Saisies d'inventaire et quantités comptées, par article ou référence. | `id`, `code_barre_reference`, `code_barre_article`, `reference`, `libelle`, `type_flux`, `date`, `quantite_comptee` |
| `dw_mouvement_stock` | Mouvements de stock, quantités, emplacements et liens vers les ordres ou demandes. | `id`, `demande_collecte_id`, `ordre_collecte_id`, `demande_livraison_id`, `ordre_livraison_id`, `demande_transfert_id`, `ordre_transfert_id`, `ordre_reception_id`, `type_mouvement`, `type_flux`, `emplacement_prise`, `emplacement_depose`, `demandeur_id`, `reference`, `libelle`, `quantite_livree`, `cree_par_id`, `code_barre_reference`, `date`, `emplacement_stock`, `code_barre_article`, `prix_unitaire`, `commentaire` |
| `dw_reception` | Réceptions, commandes et détail par article ou référence. Le même `id` peut se répéter. | `id`, `no_commande`, `statut`, `commentaire`, `date`, `date_attendue`, `numero`, `fournisseur`, `emplacement`, `reference`, `libelle`, `quantite_reference`, `quantite_article_associe`, `code_barre_article`, `code_UL`, `type_flux`, `quantite_recue`, `quantite_a_recevoir`, `code_barre_reference`, `urgence_reception`, `numero_demande_achat`, `arrivage_id`, `prix_unitaire`, `frais_livraison`, `pieces_jointes`, `cree_par_id` |
| `dw_reception_champs_libres` | Champs libres des réceptions. | `reception_id`, `libelle`, `valeur` |
| `dw_demande_achat` | Demandes d'achat et détail des lignes, quantités et réceptions liées. | `id`, `numero`, `date_creation`, `date_validation`, `date_prise_en_compte`, `date_traitement`, `demandeur_id`, `acheteur_id`, `statut`, `reference`, `libelle`, `quantite_demandee`, `quantite_stock`, `quantite_commandee`, `numero_commande`, `numero_reception`, `fournisseur`, `date_commande`, `date_attendue`, `prix_unitaire`, `frais_livraison` |
| `dw_demande_collecte` | Demandes de collecte et détail des éléments à collecter. | `id`, `numero`, `date_creation`, `date_validation`, `point_collecte`, `cree_par_id`, `objet`, `destination`, `statut`, `type`, `commentaire`, `code_barre`, `quantite` |
| `dw_collecte_champs_libres` | Champs libres des demandes de collecte ; `collecte_id` correspond à `dw_demande_collecte.id`. | `collecte_id`, `libelle`, `valeur` |
| `dw_demande_livraison` | Demandes de livraison de stock, détail des articles, références ou UL, et codes des préparations et livraisons. | `id`, `numero`, `date_creation`, `date_traitement`, `date_validation`, `date_attendue`, `projet`, `demandeur_id`, `destinataire_id`, `type`, `statut`, `codes_preparations`, `codes_livraisons`, `destination`, `commentaire`, `reference_article`, `libelle`, `code_barre`, `quantite_disponible`, `quantite_a_prelever`, `delais_traitement`, `code_UL`, `projet_article`, `commentaire_article` |
| `dw_demande_livraison_champs_libres` | Champs libres des demandes de livraison. | `demande_livraison_id`, `libelle`, `valeur` |
| `dw_demande_transfert` | Demandes de transfert et détail des articles ou références. | `id`, `numero`, `date_creation`, `date_validation`, `statut`, `demandeur_id`, `origine`, `destination`, `commentaire`, `reference`, `code_barre` |
| `dw_ordre_collecte` | Ordres de collecte et détail des éléments à collecter. | `id`, `numero`, `statut`, `date_creation`, `date_traitement`, `operateur_id`, `type`, `reference`, `libelle`, `emplacement`, `quantite_a_collecter`, `code_barre`, `destination`, `delta_date` |
| `dw_ordre_livraison` | Ordres de livraison de stock et détail des articles ou références. | `id`, `numero`, `statut`, `date_creation`, `date_livraison`, `date_demande`, `demandeur_id`, `operateur_id`, `type`, `commentaire`, `reference`, `libelle`, `emplacement`, `quantite_a_livrer`, `quantite_en_stock`, `code_barre`, `delta_date` |
| `dw_ordre_transfert` | Ordres de transfert, numéro de demande et détail des éléments transférés. | `id`, `numero_ordre`, `numero_demande`, `statut`, `demandeur_id`, `operateur_id`, `origine`, `destination`, `date_creation`, `date_transfert`, `commentaire`, `reference`, `code_barre`, `delta_date` |

## Production

| Table | Contenu | Colonnes |
| --- | --- | --- |
| `dw_production` | Ordres de fabrication (OF), jalons, quantités et emplacements. | `production_id`, `numero_of`, `urgence`, `date_attendue`, `numero_projet`, `code_produit_article`, `emplacement_depose`, `commentaire`, `piece_jointe`, `quantite`, `nombre_lignes`, `emplacement_destination`, `type`, `date_creation`, `date_traitement`, `date_dernier_statut`, `cree_par_id`, `traitee_par_id` |
| `dw_production_statut` | Historique des statuts des OF. | `production_id`, `statut`, `date_statut`, `initie_par_id` |
| `dw_production_champs_libres` | Champs libres des OF. `production_id` est déclaré en texte dans cette table. | `production_id`, `libelle`, `valeur` |

## IoT

| Table | Contenu | Colonnes |
| --- | --- | --- |
| `dw_capteur` | Capteurs non supprimés, profil, dernière remontée, batterie et gestionnaire. | `code_capteur`, `nom_capteur`, `type_capteur`, `profil_capteur`, `derniere_remontee`, `niveau_batterie`, `gestionnaire_id` |
| `dw_actionneur` | Actions paramétrées pour un capteur, modèle et seuil. | `code_capteur`, `type_modele`, `nom_modele`, `seuil_capteur`, `type_seuil` |
| `dw_capteur_messages` | Messages remontés par les capteurs, type et donnée principale. | `code_capteur`, `date_message`, `type_donnee`, `donnee_principale` |
| `dw_capteur_elements_associes` | Associations marquées actives dans Follow GT, avec dates de début et de fin. | `code_capteur`, `element_associe`, `date_association`, `date_fin_association` |
| `dw_capteur_champs_libres` | Champs libres des capteurs. | `code_capteur`, `libelle`, `valeur` |

## Référentiels et contacts

| Table | Contenu | Colonnes |
| --- | --- | --- |
| `dw_emplacement` | Emplacements, paramètres de traitement et natures appliquées à la prise ou à la dépose. | `id`, `nom`, `point_de_livraison`, `delai_max_tracabilite`, `actif`, `prise_initiale`, `pause`, `depose_finale`, `activer_changement_prise`, `activer_changement_depose`, `nouvelle_nature_prise_id`, `nouvelle_nature_depose_id`, `description` |
| `dw_nature` | Natures d'UL, contact responsable et délai maximal de traitement. | `id`, `libelle`, `code`, `responsable_id`, `delai_max_traitement` |
| `dw_contact` | Référentiel des contacts et coordonnées. Limitez l'export des coordonnées aux rapports qui en ont besoin. | `id`, `nom_affichage`, `identifiant`, `adresse`, `nom_entreprise`, `service_entreprise`, `actif`, `email`, `emails_secondaires`, `telephone`, `emplacement_dropzone`, `groupe_emplacement_dropzone`, `utilisateur_lie`, `trigramme_signataire` |
| `dw_reference_article_gestionnaire` | Contacts gestionnaires des références. | `reference_article_id`, `contact_id` |
| `dw_arrivage_destinataire` | Contacts destinataires des arrivages. | `arrivage_id`, `contact_id` |
| `dw_arrivage_acheteur` | Contacts acheteurs des arrivages. | `arrivage_id`, `contact_id` |
| `dw_emplacement_signataire` | Contacts signataires des emplacements. | `emplacement_id`, `contact_id` |
| `dw_litige_acheteur` | Contacts acheteurs des litiges. | `litige_id`, `contact_id` |
| `dw_acheminement_destinataire` | Contacts destinataires des acheminements. | `acheminement_id`, `contact_id` |

## Délais, calendrier et version

| Table | Contenu | Colonnes |
| --- | --- | --- |
| `dw_calcul_delai_traitement` | Résultats horodatés des calculs de temps écoulé par UL. | `id`, `date_calcul`, `unite_logistique_id`, `temps_passe` |
| `dw_etapes_calcul_delai_traitement` | Étapes et actions prises en compte dans un calcul de délai de traçabilité. | `id`, `action`, `date_action`, `emplacement_id`, `nature_id`, `calcul_delai_traitement_id` |
| `dw_jours_horaires_travailles` | Jours de la semaine et deux plages horaires possibles (`horaire1`–`horaire2`, `horaire3`–`horaire4`). | `jour`, `travaille`, `horaire1`, `horaire2`, `horaire3`, `horaire4` |
| `dw_jours_non_travailles` | Dates déclarées non travaillées. | `jour` |
| `dw_informations` | Version du schéma de l'EDD. | `version` |

### Requêtes de calcul complémentaires

Les scripts `delais_traitement.sql`, `delais_traitement_attendu.sql` et `delais_traitement_validation.sql` du sous-dossier `queries` calculent séparément des délais en **heures travaillées** à partir des horaires et des jours non travaillés. Ce ne sont pas des tables `dw_*` supplémentaires.

| Colonne | Période utilisée par la requête |
| --- | --- |
| `dw_demande_livraison.delais_traitement` | De la validation de la demande à la fin de la dernière livraison associée. |
| `dw_service.delais_traitement_validation` | De la création à la validation du service. |
| `dw_service.delais_traitement_attendu` | Entre la date attendue du service et sa date de validation. |
