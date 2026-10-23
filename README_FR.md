# KËR FATÛ JOP — créer un APK Android gratuitement

Ce projet emballe la version HTML actuelle de KËR FATÛ JOP dans une application Android avec Capacitor. Le fichier APK est compilé gratuitement par GitHub Actions (aucun Android Studio requis sur le téléphone).

## Étapes

1. Téléchargez et décompressez ce ZIP sur un ordinateur si possible.
2. Créez un compte GitHub gratuit sur https://github.com/ si vous n'en avez pas.
3. Créez un nouveau dépôt GitHub, par exemple `ker-fatu-jop-android`. Pour une utilisation privée, gardez-le privé; les minutes Actions gratuites dépendent des quotas du compte. Pour une compilation gratuite sans quota de dépôt privé, un dépôt public est généralement le plus simple, mais le code sera visible publiquement.
4. Téléversez tous les fichiers de ce dossier dans le dépôt, en conservant `.github/workflows/build-apk.yml`.
5. Ouvrez l'onglet **Actions** du dépôt, choisissez **Construire APK Android**, puis **Run workflow**. Si un workflow s'est déjà lancé après l'envoi des fichiers, ouvrez cette exécution.
6. Lorsque l'exécution est terminée avec succès, ouvrez-la, descendez à **Artifacts**, puis téléchargez `ker-fatu-jop-apk`.
7. Décompressez l'archive téléchargée. Sur votre Android, ouvrez `app-debug.apk` et autorisez l'installation depuis cette source si Android le demande.

## Important

- Il s'agit d'un APK de test/debug, non signé pour publication Play Store. Il est installable manuellement sur Android.
- Les données de cette version sont locales à l'appareil. Elles ne sont pas synchronisées automatiquement entre plusieurs téléphones. Exportez régulièrement une sauvegarde si l'application propose cette fonction.
- Une mise à jour installée par-dessus l'ancienne version doit garder le même identifiant d'application et la même signature; conservez le même dépôt et la même méthode de compilation.
- Ne partagez pas de données familiales sensibles dans un dépôt public. Le dépôt public expose le code source, pas les données locales contenues dans l'application installée.
- L'APK n'a pas encore été compilé ou testé dans cet environnement; la compilation doit réussir dans GitHub Actions avant installation.
