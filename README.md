# Hébergement 3D V35 — PWA Android

Ce dossier contient la version PWA du jeu. Elle peut être ajoutée à l'écran d'accueil Android et mettre en cache ses fichiers pour une utilisation hors connexion.

## Fichiers
- `index.html` : jeu adapté pour charger Three.js localement.
- `three.min.js` : moteur 3D Three.js r160.
- `manifest.json` : paramètres d'installation.
- `service-worker.js` : mise en cache hors connexion.
- `README.md` : ce guide.

## Publier sur GitHub Pages depuis un téléphone
1. Ouvrir le dépôt GitHub `HEBERGEMENT-3D-O`.
2. Ajouter les cinq fichiers de ce ZIP à la racine du dépôt (pas dans un sous-dossier), en remplaçant l'ancien `index.html` si GitHub le demande.
3. Valider/committer les changements sur la branche utilisée par GitHub Pages.
4. Attendre la publication, puis ouvrir l'adresse GitHub Pages du dépôt. L'adresse doit se terminer par `/HEBERGEMENT-3D-O/` et charger `index.html`.
5. Laisser le jeu ouvert quelques instants avec Internet pour que les fichiers soient mis en cache.

## Installer sur Android
1. Ouvrir la page du jeu dans Chrome.
2. Ouvrir le menu ⋮ de Chrome.
3. Choisir **Installer l'application** ou **Ajouter à l'écran d'accueil** (le libellé dépend de Chrome).
4. Lancer ensuite Hébergement 3D depuis l'icône créée.

## Utilisation hors connexion
La première ouverture et la mise en cache nécessitent Internet. Après que le service worker a été installé et que les fichiers ont été mis en cache, la PWA peut se lancer hors connexion. Si la première ouverture hors ligne échoue, reconnecter Internet, ouvrir la page une fois, attendre quelques secondes et réessayer.

## À savoir
- Cette PWA n'est pas un fichier APK natif : elle s'installe depuis Chrome.
- Le code du jeu enregistre certaines données dans le stockage local du navigateur. Éviter d'effacer les données du site si l'on veut conserver ces sauvegardes.
- Si une page déjà publiée est encore en cache, fermer/réouvrir Chrome ou recharger la page après la publication.
