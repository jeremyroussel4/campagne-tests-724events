# Campagne de tests — 724 Events

Étude de cas de test logiciel menée dans le cadre d’un projet de formation OpenClassrooms. Le travail couvre la préparation d’un cahier de recette, l’exécution de tests fonctionnels et exploratoires, la consignation d’anomalies et la rédaction d’un bilan de campagne.

> Projet de formation réalisé individuellement. La campagne s’est conclue par une recommandation **NO GO** au regard des anomalies observées.

## Contexte

724 Events est un site de présentation d’événements. L’objectif de la campagne était de vérifier les principaux parcours du site et de repérer les défauts à corriger avant une mise en production.

- **Période de campagne :** 7 au 10 août 2026
- **Type de tests :** fonctionnels et exploratoires
- **Rôle :** préparation des tests, exécution, analyse et restitution
- **Résultat pédagogique :** projet validé le 14 août 2026

## Démarche

1. Préparer les cas de test à partir des exigences et des parcours du site.
2. Parcourir les fonctionnalités principales : navigation, slider, événements, formulaires, pied de page et affichage responsive.
3. Exécuter les scénarios et consigner les résultats observés.
4. Explorer les parcours au-delà des scénarios prévus pour repérer d’autres anomalies.
5. Documenter les défauts avec étapes de reproduction, résultat attendu, résultat obtenu et éléments d’analyse.
6. Synthétiser les résultats et formuler une recommandation de mise en production.

## Résultats clés

Plusieurs parcours présentaient des défauts, notamment :

- l’envoi du formulaire de réservation, qui ne se terminait pas correctement ;
- l’ouverture d’une prestation depuis le pied de page, qui conduisait à une erreur applicative ;
- la gestion des erreurs du formulaire de contact ;
- des problèmes d’affichage sur les petits écrans.

Le bilan a relevé des anomalies de sévérité élevée et des fonctionnalités en échec. La recommandation était donc **NO GO** jusqu’à correction et nouvelle vérification des parcours concernés.

## Livrables

- [Synthèse de campagne](docs/bilan-de-campagne.md)
- [Exemples de cas de test](docs/cas-de-test.md)
- [Anomalies représentatives](docs/anomalies.md)

Les documents publiés ici sont des versions éditées pour le portfolio. Les liens vers les espaces de travail et identifiants de tickets ont été retirés. Les anomalies sont renumérotées pour cette présentation.

## Compétences mises en pratique

- Investiguer des anomalies d’un site afin de faciliter leur résolution
- Mettre à jour un cahier de recette avec les résultats d’exécution
- Rédiger un bilan de campagne de tests
- Distinguer les faits observés des hypothèses sur la cause technique

## Limites de l’analyse

Les vérifications réseau et navigateur ont aidé à caractériser plusieurs défauts. Pour certaines anomalies, les éléments disponibles ne permettaient pas de confirmer la cause technique exacte ; ces limites sont conservées dans les fiches plutôt que de présenter une hypothèse comme un diagnostic établi.

## À propos

Étude de cas issue d’un projet pédagogique. Le site testé et les éléments de marque associés ne sont pas la propriété de l’auteur de ce portfolio.
