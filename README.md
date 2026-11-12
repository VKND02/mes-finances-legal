# Mes Finances — pages légales

Site statique public (sans JavaScript, sans connexion bancaire, sans données privées) pour l'application personnelle **Mes Finances**.

## Déploiement sur GitHub Pages, gratuitement

1. Sur le compte GitHub propriétaire de ce projet, créer un dépôt **public** nommé `mes-finances-legal`. Ne pas utiliser de dépôt contenant du code bancaire, des tokens ou des fichiers privés.
2. Ouvrir le dépôt, puis **Add file → Upload files**. Ajouter tous les fichiers à la racine : `index.html`, `privacy.html`, `terms.html`, `style.css`, `.nojekyll` (le dernier est optionnel).
3. Valider le commit sur la branche `main`.
4. Ouvrir **Settings → Pages → Build and deployment**, choisir **Deploy from a branch**, **main**, **/(root)**, puis **Save**.
5. Attendre l'affichage de l'URL dans **Settings → Pages**, la visiter et vérifier que chaque page s'affiche correctement.

Avec le compte GitHub `VKND02`, l'adresse *attendue après publication et validation* serait :
- `https://vknd02.github.io/mes-finances-legal/privacy.html`
- `https://vknd02.github.io/mes-finances-legal/terms.html`

Ces adresses ne sont **pas encore publiées** par ce dossier et ne doivent pas être considérées comme actives sans vérification.

## Enable Banking

Dans le formulaire Production (usage personnel restreint) :
- **Application name** : `Mes Finances`
- **Application description** : `Private, non-commercial personal finance application for aggregating my own bank accounts, tracking expenses, and managing budgets in EUR and CAD.`
- **Email for data protection matters** : ton adresse personnelle (ne pas l'inclure dans ce dépôt public)
- **Privacy URL** : adresse HTTPS de `privacy.html` **vérifiée active**
- **Terms URL** : adresse HTTPS de `terms.html` **vérifiée active**
- **Allowed redirect URLs** : ne pas utiliser le site GitHub Pages comme callback bancaire. Définir plus tard le vrai callback HTTPS de l'application/serveur de confiance.

Les liens du formulaire ne sont pas vérifiés à l'activation restreinte, mais les pages doivent rester exactes et seront à adapter avant connexion bancaire réelle.

## Sécurité

Ne jamais mettre dans ce dépôt GitHub public : clés `.pem`, JWT, tokens d'accès, fichiers de transactions, exports CSV, identifiants, captures bancaires, historiques ou Google Sheets privés.

**Ce site est une vitrine légale, pas le système d'agrégation bancaire.** Il n'héberge aucun backend de connexion.
