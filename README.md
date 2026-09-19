# Hyperliquid Scanner V3.3 — GitHub Pages V7

Version GitHub Pages du scanner Hyperliquid, avec appel direct à l'API Hyperliquid depuis le navigateur.

## Nouveauté V7 — journal d'erreurs
Un panneau **🧾 Journal d’erreurs** est placé tout en bas de la page.

Il enregistre automatiquement :
- les erreurs JavaScript globales (`window.onerror`) ;
- les Promises rejetées sans gestionnaire (`unhandledrejection`) ;
- les erreurs de connexion/fetch à l'API Hyperliquid ;
- les réponses HTTP en erreur ;
- les erreurs de décodage JSON ;
- les erreurs rencontrées pendant le scan d'une paire, avec le symbole concerné ;
- les erreurs des diagnostics et du scan.

Chaque entrée contient l'heure, le contexte, le message, la pile d'appel et, lorsque le navigateur le fournit, le fichier, la ligne et la colonne concernés.

Le journal est conservé localement dans le navigateur (maximum 200 événements) et peut être :
- téléchargé en fichier `.txt` ;
- copié dans le presse-papiers ;
- vidé avec le bouton dédié.

Le scanner reste entièrement côté navigateur et utilise directement `https://api.hyperliquid.xyz/info`.
