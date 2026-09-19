# Hyperliquid Scanner V3.2 — Netlify

Architecture: iPhone/Safari → Netlify Function → Hyperliquid.

## V3.2 changes
- Toutes les dates/horaires affichés dans l'interface utilisent l'ordre **heure → date** (`HH:mm · JJ/MM/AAAA`).
- Le panneau gagnant reste au-dessus du classement.
- Titre gagnant réduit à `🏆 COIN — LEVERAGE×`, en vert pour une hausse et rouge pour une baisse.
- Suppression du sous-titre directionnel, de la ligne début/fin supplémentaire et des légendes du graphique.
- Suppression des repères temporels de l'axe horizontal.
- Les heures de début et de fin sont affichées en grand sur le graphique, sans les mots « Début » et « Fin ».
- Le classement est présenté sous forme de vignettes responsive, une par ligne, adaptées au smartphone.
- Le rang `#`, la colonne Bougies et l'option Marchés max restent supprimés.
- Deux mouvements par perp sont conservés : meilleur haussier et meilleur baissier.
- Diagnostic toujours dernier panneau.

## Déploiement
Décompresser le ZIP et déployer le dossier sur Netlify. La fonction est dans `netlify/functions/hyperliquid.js`.
