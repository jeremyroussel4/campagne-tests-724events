# Bilan de campagne — 724 Events

## Synthèse

| Élément | Résultat |
|---|---|
| Type de campagne | Tests fonctionnels et exploratoires |
| Période | 7–10 août 2026 |
| Décision | **NO GO** |
| Motif principal | Plusieurs parcours essentiels échouent ou donnent un retour incomplet à l’utilisateur |

## Objectifs

- Vérifier la conformité du site aux exigences disponibles.
- Valider le fonctionnement des principaux parcours.
- Repérer les anomalies avant la mise en production.
- Couvrir plusieurs exigences avec des scénarios pertinents.
- Vérifier qu’aucune anomalie critique ne bloque la campagne sans être signalée.

## Périmètre observé

Navigation, slider, pages de détail d’événements, formulaire de réservation, services, réalisations, équipe, formulaire de contact, pied de page et affichage responsive.

## Constats principaux

- **Réservation :** la soumission ne se concluait pas correctement et aucun message de confirmation n’était affiché.
- **Détail d’une prestation :** l’accès depuis le pied de page provoquait une erreur applicative.
- **Contact :** les erreurs de validation attendues n’étaient pas présentées à l’utilisateur ; un élément prévu dans le scénario n’était pas présent dans le formulaire.
- **Navigation et contenu :** des liens depuis une page de détail et le filtre des réalisations ne donnaient pas le résultat attendu.
- **Responsive :** certains éléments du formulaire et du pied de page débordaient ou perdaient leur alignement sur écran réduit.
- **Slider :** l’indicateur du slide actif ne correspondait pas toujours au contenu affiché.

## Décision

**NO GO.** Les défauts touchant la réservation, l’accès à une prestation, les retours de validation et l’affichage responsive dégradent des parcours visibles par les utilisateurs. La mise en production devrait attendre la correction des anomalies concernées et une nouvelle exécution des scénarios en échec.

## Retour sur le livrable

Le projet a été validé. L’évaluation a souligné la complétude des documents, la logique de la phase exploratoire et la qualité du bilan. L’axe d’amélioration identifié portait sur la présentation du rapport : limiter les sauts de page et structurer davantage le texte. Cette version portfolio condense les résultats en sections courtes pour faciliter la lecture.

## Limites

Les observations et vérifications réseau permettent de décrire plusieurs symptômes et réponses. Elles ne suffisent pas toujours à établir la cause technique côté application. Les fiches d’anomalie distinguent donc les éléments vérifiés des causes qui restent à confirmer.
