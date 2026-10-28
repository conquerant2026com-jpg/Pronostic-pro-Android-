PRONOSTIC PRO V2 — SOURCE ANDROID + API

Le dossier www contient l'application web et l'onglet « Matchs du jour ». Le dossier server contient un relais API pour API-Football. package.json et capacitor.config.json préparent la conversion Android avec Capacitor.

IMPORTANT : ce ZIP n'est pas un APK et ne contient aucune clé API. Les matchs Internet ne s'afficheront qu'après configuration de la clé fournisseur, déploiement du serveur sur HTTPS, puis saisie de l'URL dans l'application.

DONNÉES EN LIGNE
1. Crée un compte et récupère une clé sur https://www.api-football.com/
2. Dans server/, installe Node.js puis exécute npm install.
3. Copie .env.example en .env et renseigne APISPORTS_KEY=ta_clé.
4. Exécute npm start et déploie le serveur sur un hébergement Node.js HTTPS.
5. Dans l'onglet Matchs du jour de l'application, colle l'URL HTTPS du serveur et appuie sur Actualiser.
La clé doit rester côté serveur, jamais dans www. Le forfait gratuit a des limites d'appels et de couverture; vérifie les conditions du fournisseur.

CONSTRUIRE L'APK (ordinateur recommandé)
1. Installe Node.js et Android Studio + Android SDK.
2. À la racine du projet : npm install
3. npx cap add android
4. npx cap sync android
5. npx cap open android
6. Dans Android Studio : Build > Build Bundle(s) / APK(s) > Build APK(s). Pour distribuer largement, configure une signature release.
Documentation : https://capacitorjs.com/docs/getting-started

Le modèle de pronostic actuel reste heuristique et ne fournit pas de probabilités validées. Les tickets restent stockés localement. Aucun pari n'est placé automatiquement.
