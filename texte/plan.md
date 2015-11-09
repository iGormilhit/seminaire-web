---
title: plan de présentation
author: iGor
date: 2015-11-09
---

# Reprise points "modèle"

   1. Brève introduction étude
   2. Formulation des hypothèses
   3. Décrire approche utilisée
   4. Décrire résultats et conclusions principales
   5. Expliquer importance des résultats et conclusions
   6. Critique de l'étude (+/-)

# Plan

   1. Introduction étude
      1. Auteur
      2. Notion *Privacy* et sécurité
      3. *Reviewing for*
      4. Les orgs. : IETF et W3C → standards Internet et Web
         1. volontariat
         2. consensus
      5. Révélations Snowden
   2. Buts de l'étude
      1. Pas vraiment d'hypothèses (voir structure)
      2. Comprendre fonctnmt des orgas → fabrique standards
      3. Observer réaction révélations Snowden
      4. Identifier tendances pour éval. *privacy* et sécurité
   3. Approche
      1. Analyse textuelle automatique et manuelle
         1. RFCs et *mailing lists* de IETF (nbr lignes / nombre lignes total)
            1. Historique complet depuis 1969
            2. *privacy* notion transversale, comme a11y, i18n, *sécurité*
            3. Couches : déterminisme couches de bases
            4. Méthode : *parse* le *plain-text*, repère les sections, nbre de lignes sur hauteur fixe, puis calcul rapport entre longueur RFC et longueur partie sécurité.
         2. TRs et *mailing lists* de W3C (nbre de TRs mentionnant termes)
         3. Actus des medias de masse, rapports, documents principaux de standards en réponse à Snowden : timeline
         4. Entretien semi-structurés (IETF et W3C)
      2. Description champ de recherche :
         1. Def. *privacy* : protection contre immixion et contrôle
         2. *essentially contested concept*
         3. Les deux orgas : centrales (même si pas de limites, i.e. WHATWG, OASIS), + accès
      3. Produit :
         1. Historique
         2. Réaction à Snowden
         3. Tendances
   4. Résultats et conclusions
      1. Historique IETF
         1. Historique complet RFCs depuis 1969
         2. 1987, intro obligation aborder sécurité
         3. → 100% RFCs pour sécurité
         4. 20% pour *privacy*
         5. RFC 1543 : *Instructions to RFC authors*
         6. Mention sécurité insuffisantes durant 90s (quote, RFC 3552, 2003)
         7. 1996, RFC signale que section sécurité pas assez nombreuses, trop courtes
         8. Sécurité quasiment absentes avant 90s, très brèves ensuite
         9. 2000, sections plus grandes, mais tout de même minimaliste et long != qualité
         10. Introduction d'un modèle, avec section *Security Considerations* et outil de validation
         11. Sections évaluées par *Security Directorate*
         12. quote IETF
         13. *Area Directors* et les 2 *Security Area Directors* + IESG : *reviewing*, importance de sécurité et *privacy*
       2. IETF : de la sécurité à la *privacy*
          1. juillet 2013, RFC 6973, recommandation pr rédaction RFCs en rapport *privacy*
            * liste menaces particulières
            * réduction de ces risques
            * *checklist* pour identifier et résoudre problèmes de *privacy*
          2. RFC spécifiques *privacy* : ``geopriv`` WG (géolocalisation) : modèle de com. des données de géolocalisation (standard), avec exigence d'une politique claire d'utilisation des données, et contrôle par l'utilisateur.
      3. *privacy* dans standards du **W3C**
          1. Pas d'exigences spécifiques comme IETF, mais nombre plus stable, env. 20%
          2. fig3 : % de TR mentionnant au moins 1x le terme
          3. P3P, DNT
          4. *reviewing for privacy* au W3C, méthode
      4. Réactions à Snowden
      5. Tendances
   5. Importances résultats et conclusions
       1. ?
   6. Critique
      1. Utilisation plus visible des données quantitatives
      2. Utilisation plus visible des entretiens semi-structurés
      3. Intérêt de mieux comprendre fonctionnement                                                                
