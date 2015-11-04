---
title: Notes de lecture
author: iGor
date: 2015-11-22
---

# Structure de l'article

```
├── I. Introduction
├── II. Method
│   ├── A. Data Sources
│   └── B. Scope
├── III. History of Privacy and Security Reviews
│   ├── A. IETF
│   └── B. W3C
```

# Définitions

À définir :

  * *privacy* et proposer une/des traductions.
  * Internet.
  * Web.
  * *Standard-setting organisations*, standards.
  * *reviewing for*.
  * IEEE : Institute of Electrical and Electronics Engineers
  * CS : Computer Society (association prof depuis 1971, conf, ateliers, peer reviews journals

Nick Doty :

  * [npdoty.name](https://npdoty.name/)
  * [CV](https://npdoty.name/npd-resume-2014.pdf)
  * bachelor en philo.
  * master en information management system
  * phD en IS
  * privacy analyst for W3C ([Privacy Interest Group (Ping)](http://www.w3.org/Privacy/)), [Do Not Track](http://www.w3.org/TR/tracking-dnt/)

# Abstract

Fonctionnalité Internet et Web déterminées par Standards → implémentations interopérables.
→ l'intimité des relations en ligne dépendent du travail fait dans les organistions qui établissent les standards.

Quelle importance des structures et modes de fonctionnement de ces orgs sur des valeurs comme la *privacy* ? [Question de recherche ?]

L'article évalue :

* l'histoire des considérations à propos de la *privacy* et de la sécurité dans ces orgs,
* l'impact de *Snowden* et les réactions,
* tendances sur la manière d'évaluer ces questions (*privacy* et sécurité).

# Introduction

Fonctionnalités ← standards (permettent des implémentations interopérables). *online privacy* dépend du travail des orgs développant ces standards.

L'évaluation des points liés à la *privacy* sont toujours faits sur les systèmes logiciels, dans le contexte des standards Internet, c'est pas si simple.

Les orgs travaillent par concensus, et la participation est sur une base volontaire, et sur un mode *bottom-up*, contairement au *top-down* des grandes boîtes.

Structure des standards Internet : par couche et *generative* (comme dans grammaire générative). But : permettre une grande variété d'implélmentation, d'application. → résistent à l'analyse systématique (**à préciser**).

Mentionne des travaux précédents présentant ces orgs (*multistakeholder groups*) comme des organisations frontières, avec des réponses innovatives. Leurs structure et approches ne sont pas suffisamment comprises.

Description du plan du travail :

   1. II : méthode, data, champ du travail
   2. III :
      1. procédures, outils, structure organisationnelle de IETF impactent les aspects de la sécurité, et le rapport avec la *privacy* des standards Internet
      2. contexte des standards spécifiques à la *privacy* pour le Web, l'auteur montre comment ce point est conçu (perçu, pensé ?) et comment la revue (évaluation) de ce point est réalisée
   3. IV : description des différentes réactions dans la communauté qui établit les standards face aux révélations Snowden, et l'impacte de celle-ci sur la manière d'évaluer les standards en lien avec la *privacy*.
   4. V : Sur base de III et IV, identification de 3 tendances : systématisation, intégration, *leadership*

# Méthode

## Sources de données

3 sources de données :

   1. Les standards Internet et Web eux-mêmes, corpus pour analyse textuelle automatique, indique et confirme les tendances quantitativement. Et l'activité y relative sur les mailings lists publiques.
   2. Les articles d'information *mainstream*, rapports de rencontres, principaux documents de standards → constituer la *timeline* et le type de réponse aux révélations Snowden.
   3. Entretiens semi-structurés avec des ingénieurs experts d'Internet et qui participent à IETF → perpective interne.

## Champ de recherche

Ne suppose pas une def. de *privacy*, mais : protection contre l'intrusion, immixion (cf. déclaration des droits de l'homme, [art. 12](http://www.un.org/fr/documents/udhr/#a12)) **ET** contrôle des informations concernant soi-même.

*essentially-contested concept* [wp](https://en.wikipedia.org/wiki/Essentially_contested_concept) et [wpfr](https://fr.wikipedia.org/wiki/Concept_essentiellement_contest%C3%A9) : n'a pas donné plus d'importance aux interviewés, ni supposé qu'ils aient une def partagée de la *privacy*. Pourtant, ça a une influence sur leur travail de conception de standards.

Centré sur deux orgs définissant des standards :

   * [Internet Engineering Task Force](http://www.ietf.org/) (IETF)
   * World Wide Web Consortium (W3C)

Les deux incontournables pour les protocols Internet et Web et sur model volontaire et concensus → pas de limite précise sur où se définissent les standards. Ex HTML5 et le WHATWG ([Web Hypertext Application Technology Working Group](https://whatwg.org/)), groupe de vendeurs de navigateurs. En collaboration ou non avec le W3C.

Autre exemple : [OASIS](https://www.oasis-open.org/), pour des applications du XML en sécurité, santé, web, commerce, etc. (Mais aussi le ODT). Se sont préoccupés de standards pour des méthodologie d'organisation devant gérer des éléments de *privacy* et se penchent sur des standards de processus qui prévoient dans leur conception la *privacy*.

Trop de lieux/orgs qui s'occupent de standards pour tous les mentionner, décrire. Sélectionne IETF et W3C, parce qu'il y accède... cf section *Future Work* qui devrait vérifier si dans les autres orgs définissant des standrards ça fonctionne de manière similaire ou pas.

# Histoire des évaluations de la *privacy* et de la sécurité

S'intéresse d'abord à la *privacy*, puis aux notions de sécurité en lien à IETF, puis W3C.

## Internet Engineering Task Force

Dispose de l'historique complet des documents publiés depuis 1969. Les publications de standards sont les RFC : [*Requests for Comment*](https://fr.wikipedia.org/wiki/Request_for_comments "wpfr"). La *privacy* != un sujet explicite, mais présent depuis le début sous le thème de la sécurité des communications.

La sécurité comme précurseur utile de la notion de *privacy* parce que :

   * La sécurité, comme *privacy*, a11y, i18n, performance, etc, sont des sujets transversaux ou *horizontaux*.
   * Plusieurs aspects de la *privacy*, la sécurité sont des pré-requis (confidentialité, intégrité);
   * Tech. en couches, la sécurité des couches de base déterminent si la *privacy* peut être possible à une couche applicative supérieure.
   * Non seulement il y a rel. entre sécurité et *privacy*, mais sécurité est un domaine qui peut s'appuyer sur expérience et méthodolgie, qu'on peut adapter pour défendre la *privacy*.

### Historique des considérations relatives à la sécurité

Vers 1987, intro d'une obligation d'aborder sécurité dans RFC → augmentation importante, puis 100% des RFCs mentionnent au moins le sujet (voir [fig1](figures/fig-1.gif). Pas le cas pour les mentions de *privacy*, au max 20% environ. L'obligation a un effet...

[RFC 1543](https://tools.ietf.org/html/rfc1543), 1993, *Instructions to RFC authors*. Toujours mise à jour (encore en 2014). Ne s'occupe que de la mise en forme (modèle), n'impose pas d'élément de contenu en matière de sécurité. Tout le monde d'accord pour dire que durant les 90, les considérations de sécurité étaient insuffisantes dans les RFCs.

Mentionne [RFC 3552](https://tools.ietf.org/html/rfc3552), 2003, *Guidelines for Writing RFC Text on Security Considerations* :

> All RFCs are required to hava a Security Considerations section. Historically, such sections have been relatively weak.

En 1996, une RFCs signale que les sections sur la sécurité ne sont pas si nombreuses et surtout très brèves...

**L'analyse textuelle automatique** [on aurait aimé une courte description] confirme, voir [fig 2](figures/fig-2.gif). La légende de la figure explique un peu le type d'analyse : *parse* le *plain-text*, repère les sections, et le nombre de ligne à largeur fixe, puis calcul d'un rapport entre la longueur de la RFC et la longueur de la partie "sécurité".

Considérations sécurité quasi absentes avant 90, très brèves au cours des 90. Depuis 2000, les sections se ralongent quelque peu, une plus grande proportion de chaque RFC, mais la plupart des sections restent minimalistes. La longueur des sections sécurité ne garantissent pas qualité sécurité, mais bonne mesure de l'attention portée au sujet.

Éléments technique renforçant la conformité avec exigences pour rédaction RFCs : modèle comprenant une section *Security Considerations* + outils de vérification de soumissions vérifiant la présence des sections. Ces sections sont ensuite évaluées par des reviewers volontaires qui participent au [*Security Directorate*](http://trac.tools.ietf.org/area/sec/trac/wiki/SecDirReview).

Selon affirmation d'un interivewé de IETF,

> Now everyone [thinks about security]. Not everyone does, but as soon as you don't, you get called out."

Info donnée aux *Area Directors*, part. les deux *Security Area Directors*. Chaque RFC évaluée par *IESG* (*Internet Engineering Steering Group*), RFCs peuvent être rejetées, ou sujettes à révisions si considérations sur la sécurité ou *privacy* pas suffisantes. Parfois évaluation pointilleuses et approbation difficile

### De la sécurité à la *privacy*

[RFC 6973](https://tools.ietf.org/html/6973), juillet 2013, introduit des recommandations pour la rédactions RFCs en rapport avec *privacy* :

   * liste des menaces particulières
   * des réduction de ces risques
   * une liste de question à vérifier pour identifier et résoudre les problèmes de *privacy*

Existe aussi des RFCs spécifiques à la *privacy* : le [``geopriv`` Working Group](http://www.ietf.org/wg/concluded/geopriv.html), développement de standards sur transmission des données de géolocalisation (qui prendrait en compte le choix de l'utilisateur, donc pas seulement sécurité des communications). Pendant plusieurs années, le groupe a développé :

   * des conditions nécessaires
   * analyses de menaces (modèles de menace ?)
   * formats de fichiers
   * plan

d'un modèle basique de communication d'information de géolocalisation sous forme de standard, avec l'exigence d'une politique claire de l'utilisation de ces données, communiquée à et contrôlée par l'utilisateur. Modèle jugé trop exigeant, existence d'une controverse.

Le fait que ces préoccupations s'appliquent à des domaines de types applicatifs est en cohérence avec les standards attentifs à la *privacy* au W3C : web est une couche applicative d'Internet.

## La *privacy* dans les standards du *World Wide Web Consortium*

IETF : RFCs. Pour le W3C, ce sont des TRs pour [*Technical Reports*](http://www.w3.org/TR/).

W3C publie aussi standards techniques, en accès libre → analysables. Pas d'exigences spécifiques comme au IETF, mais un nombre plus stable, et relativement important (envir. 20 %), voir [fig 4](figures/fig-4.gif). Le graph montre le pourcentage de TR qui mentionne au moins une fois le terme recherché.

### Standards spécifiques sur la *privacy*

Au W3C efforts significatifs spécifiques avec *privacy*. Non seulement mentionné ou abordé, mais même des standards qui s'occupent principalement de cette question sur le Web.

#### *Platform for privacy Preferences Project* (*P3P*)

http://www.w3.org/P3P/

*Était* effort sur plusieurs années d'améliorer la prise de conscience des pratiques des sites Web concernant *privacy* au moyen de description *machine readable* de leurs politiques. Existent d'autres tentatives de résoudre le problème : les divers projets d'icônes pour la *privacy* (http://opennotice.org - pas accessible le 2015-11-04); efforts avec plusieurs participants, soutenu par le US.gov pour établir des standards pour des avertissements courts, clairs et transparents.

P3P définit un langage XML extensible (?) pour communiquer les pratiques *privacy*, en développant un concept utilisé pour afficher quels contenus sont appropriés pour tel ou tel groupe d'âge. Conçu par couche pour offrir un langage neutre et descriptif pour les pratiques offrant une flexibilité pour les implémentations ou permettant aux usagers de se faire leur propre idée sur les différentes pratiques et sur les différentes possiblités de gérer les préférences en matière de *privacy*. Selon le principe : "*mechanism, not policy*". Pas eu un grand succès (sites Web et navigateurs) : pour cause, du moins exprimée, de trop grande complexité et manque d'incitation.

#### *Do Not Track* (*DNT*)

http://www.w3.org/TR/tracking-dnt/

Effort sur plusieurs années → mécanisme offrant à l'utilisateur le choix face au *tracking* du comportement en ligne. 2010 : pris en charge par *Federal Trade Commission*. 2011 implémentés dans les navigateurs, et efforts de standardisation. L'utilisateur doit pouvoir définir dans les préférences de son navigateur s'il accorde ou non aux sites Web le *tracking*, préférence qui doit être communiqué aux services en ligne. Comme P3P, n'impose pas des propriétés type *privacy*, ne limite pas automatiquement le *tracking*. Suppose coopération entre les *users agents* et les serveurs (qui décideraient de tenir compte des préférences des utilisateurs).

A été mis à jour, plus grande souplesse offerte aux serveurs d'indiquer comment ils tiennent compte des préférences des utilisateurs. Mention du *Privacy Badger* de l'EFF, qui bloque les cookies tiers s'ils n'affichent pas leur méthode DNT.
