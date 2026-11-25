# Application — Touch Unique Gestion

Dossier à publier à la racine du dépôt `touchunique-app`.

Fichiers clés :

- `index.html` — coquille, navigation, panneau assistant, modales, toasts.
- `css/styles.css` — thème sombre / clair, responsive, `prefers-reduced-motion`.
- `js/data.js` — miroir généré du catalogue et du contenu.
- `js/automation.js` — copie de `../ai/engine.js` (moteur local).
- `js/store.js` — base `tus_app_db_v1`, import des leads `tus_site_leads_v1`.
- `js/sync.js` — liaison temps réel avec le site (`BroadcastChannel` + `tus_sync_v1`).
- `js/app.js` — vues, actions, assistant, cycle autopilot, export/import.
- `assets/` — données miroir, images catalogue, portraits et icônes.

Fonctions testées : import d’un lead depuis le site, score « chaud », création automatique de projet et de tâches, cycle autopilot, génération de pack de contenu (5 cartes), file sociale, suggestions boutique, export CSV/JSON. Lighthouse : Accessibilité 100, Bonnes pratiques 100, SEO 100.

Les connecteurs non configurés restent explicitement « Non connecté » dans les réglages : aucune publication ni paiement simulé.
