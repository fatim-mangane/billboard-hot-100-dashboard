# Billboard Hot 100 — Music Insights

Tableau de bord web statique construit à partir du fichier CSV Billboard Hot 100 fourni.

## Fichiers
- `index.html` : interface interactive (Chart.js via CDN)
- `data.json` : agrégats calculés à partir du CSV original

## Tester en local
Ouvrir `index.html` dans un navigateur avec une connexion Internet. Si le navigateur bloque le chargement local de `data.json`, lancer un serveur local depuis ce dossier :
`python -m http.server 8000`
Puis ouvrir `http://localhost:8000`.

## Déployer gratuitement sur Vercel
1. Créer un dépôt GitHub et y téléverser `index.html`, `data.json` et ce README.
2. Dans Vercel, choisir **Add New → Project**, importer le dépôt GitHub.
3. Framework Preset : **Other** ; Build Command : laisser vide ; Output Directory : `.`.
4. Cliquer sur Deploy. Vercel fournit une URL publique.

Les données sont agrégées localement à partir du CSV. Les années 1958 et 2021 sont partielles.
