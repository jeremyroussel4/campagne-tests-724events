# Anomalies représentatives

Fiches synthétiques sélectionnées pour illustrer la rédaction et l’analyse. Les références sont anonymisées et propres à cette version portfolio.

## QA-01 — La réservation ne confirme pas l’envoi

**Sévérité observée :** élevée  
**Reproductibilité :** systématique lors du scénario décrit

**Étapes**
1. Ouvrir la page d’un événement.
2. Renseigner les champs avec des valeurs valides.
3. Envoyer le formulaire.

**Attendu**  
La réservation est envoyée et un message de confirmation est affiché.

**Observé**  
Aucun message de confirmation n’apparaît et la requête échoue avec une réponse HTTP 400.

**Analyse**  
La requête envoyée et la documentation de l’API semblaient en désaccord sur le type attendu pour un champ. L’observation établit une incohérence entre contrat documenté et réponse de l’API ; la cause côté serveur reste à confirmer.

## QA-02 — L’accès à la dernière prestation déclenche une erreur

**Sévérité observée :** élevée  
**Reproductibilité :** systématique lors du scénario décrit

**Étapes**
1. Ouvrir la page d’accueil.
2. Descendre jusqu’au pied de page.
3. Sélectionner la dernière prestation.

**Attendu**  
La page de la prestation s’affiche avec ses informations.

**Observé**  
Une erreur applicative est affichée ; l’appel associé retourne une réponse HTTP 500.

**Analyse**  
Le même échec a été observé lors d’une vérification directe de l’endpoint documenté. Les éléments disponibles ne permettent pas d’identifier la cause serveur exacte.

## QA-03 — Les erreurs du formulaire de contact ne sont pas affichées

**Sévérité observée :** élevée  
**Reproductibilité :** systématique lors du scénario décrit

**Étapes**
1. Ouvrir la section Contact.
2. Ne renseigner qu’une partie des champs.
3. Envoyer le formulaire.

**Attendu**  
Les champs manquants sont signalés clairement et le formulaire reste compréhensible.

**Observé**  
Aucun message d’erreur n’est affiché alors que l’API répond avec une erreur de validation HTTP 400.

**Analyse**  
La validation côté serveur est observable ; le défaut porte sur le retour présenté dans l’interface. Une case d’autorisation prévue dans le scénario de recette était également absente du formulaire.

## QA-04 — Le formulaire déborde sur petit écran

**Sévérité observée :** élevée  
**Reproductibilité :** reproductible

**Étapes**
1. Réduire la largeur de la fenêtre ou activer l’affichage responsive.
2. Ouvrir la section Contact.
3. Observer les champs du formulaire.

**Attendu**  
Les champs restent entièrement visibles et s’adaptent à la largeur disponible.

**Observé**  
Les champs dépassent de leur conteneur et une partie de la mise en page est tronquée.

**Analyse**  
Le défaut a été observé en affichage responsive. La fiche décrit le comportement constaté sans présumer de la correction à apporter.
