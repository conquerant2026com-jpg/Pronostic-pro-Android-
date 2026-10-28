PRONOSTIC PRO — prototype PWA

CONTENU
- index.html : interface, analyse indicative, ticket, historique
- manifest.webmanifest : métadonnées d'installation
- sw.js : cache hors ligne de base
- icon.svg : icône

IMPORTANT
Cette première version n'a pas de flux de données sportives en direct configuré.
L'indice d'analyse est une heuristique basée sur les valeurs saisies par l'utilisateur,
pas une probabilité statistique validée. Les tickets sont enregistrés localement dans
le navigateur et ne sont pas synchronisés entre appareils.

INSTALLATION ANDROID
La PWA doit être servie sur une adresse HTTPS pour permettre l'installation fiable.
1. Décompressez le dossier et hébergez son contenu sur un hébergement HTTPS statique.
2. Ouvrez l'URL du site dans Chrome sur Android.
3. Menu ⋮ > Installer l'application (ou Ajouter à l'écran d'accueil).
4. Lancez Pronostic Pro depuis l'icône créée.

Pour produire un APK natif, il faudra ensuite envelopper la PWA dans un projet Android
(par exemple Capacitor), construire avec Android Studio et signer le paquet. Ce zip n'est
pas un APK installable directement.
