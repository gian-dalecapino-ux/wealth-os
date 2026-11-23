# Wealth OS — gestionnaire financier personnel

Cockpit financier personnel : fiche de paie, budget, séquençage de la trésorerie, épargne et scénarios, centre d'actions chiffrées.
Un seul fichier (`index.html`), sans build ni serveur. Les données restent dans le navigateur (`localStorage`).

## Fonctionnalités
- **Accueil** : revenu net, cash-flow libre, taux d'épargne, runway (chaque carte explique sa formule), action prioritaire.
- **Paie** : import du PDF de la fiche de paie (lecture locale via pdf.js) ou saisie manuelle.
- **Budget** : postes prévu/réel par famille, jour de prélèvement, abonnements annualisés.
- **Séquence** : ordre de répartition à la paie, solde projeté sur 30 jours, poids des prélèvements par semaine.
- **Épargne** : rythme requis, leviers d'économie, revenu complémentaire, projection prudent/central/optimiste (hypothèses non garanties).
- **Actions** : constat, impact, action, alternative, confiance pour chaque recommandation.

## Déployer sur GitHub Pages
1. Crée un dépôt et pousse `index.html`, `README.md`, `.nojekyll`.
2. Settings → Pages → Source : branche `main`, dossier `/ (root)`.
3. L'app est servie sur `https://<utilisateur>.github.io/<depot>/`.

## Hypothèses à vérifier
- Le revenu net (1 900 €) est une **valeur de démonstration** tant qu'aucune paie n'est saisie.
- Les jours de prélèvement et la fin du crédit étudiant (déc. 2029) sont des estimations modifiables.
- La lecture PDF est une détection par mots-clés : vérifier les montants proposés.
