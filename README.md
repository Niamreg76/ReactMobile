# ReactMobile Roman Germain

# Guide de Déploiement et d'Exécution de l'Application

Ce guide fournit des instructions étape par étape pour déployer et exécuter votre application sur un serveur en utilisant SSH.

## Étapes

1. **Se Connecter au Serveur :**
   - Ouvrez un terminal sur votre machine locale.
   - Utilisez la commande suivante pour vous connecter à votre serveur via SSH :
     ```bash
     ssh nom_utilisateur@adresse_ip_de_votre_serveur
     ```
   - Remplacez `nom_utilisateur` par le nom d'utilisateur de votre serveur et `adresse_ip_de_votre_serveur` par l'adresse IP de votre serveur.

2. **Accéder au Répertoire du Projet :**
   - Une fois connecté, accédez au répertoire où vous souhaitez déployer votre application. Par exemple :
     ```bash
     cd /chemin/vers/votre/projet
     ```

3. **Transférer le code de l'Application :**
   - Si ce n'est pas déjà fait, transférez le code de votre application sur le serveur. Vous pouvez utiliser `scp` ou toute autre méthode de votre choix.
     ```bash
     scp -r /chemin/vers/votre/projet/local nom_utilisateur@adresse_ip_de_votre_serveur:/chemin/vers/destination
     ```
     Remplacez les chemins et les détails du serveur en conséquence.

4. **Installer les Dépendances :**
   - Installer Node.js
     ```bash
     # Exemple pour une application Node.js avec npm
     cd /chemin/vers/votre/projet
     npm install
     ```

5. **Compiler l'application :**
     ```bash
     # Exemple pour une application Node.js
     npm run build
     ```

6. **Lancer l'application :**
   - Démarrez l'application.
     ```bash
     # Exemple pour une application Node.js
     npm start
     ```

7. **Accéder à l'application :**
   - Ouvrez un navigateur web et accédez à l'adresse IP du serveur sur le port ou le chemin spécifié.
  
8. Exécution de l'application

Téléchargez l'APK généré depuis le serveur SSH.
Installez l'APK sur un appareil Android.
Exécutez l'application sur l'appareil.

~~L'APK devrait se trouver dans le dossier wrapper dans le chemin /mobile/deploy_2023-12-07_0916/app-mobile/android/gradle/wrapper$~~
