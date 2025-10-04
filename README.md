
    LOCAL SITE TESTER v1.0

Cette application vous permet de tester vos sites web locaux 
sur votre téléphone en quelques clics.


📋 UTILISATION

1. DÉMARRER LE SERVEUR
   - Double-cliquez sur "Local Site Tester" dans le menu Démarrer
   - Ou lancez "start-server.bat"
   - Une fenêtre de commande s'ouvrira avec l'adresse IP

2. OUVRIR L'INTERFACE
   - Ouvrez votre navigateur
   - Allez sur http://localhost:4000

3. UPLOADER VOTRE SITE
   - Sélectionnez un dossier complet ou des fichiers individuels
   - Les fichiers CSS et JS seront automatiquement injectés
   - Cliquez sur "Héberger"

4. TESTER SUR MOBILE
   - Assurez-vous que votre téléphone est sur le même WiFi
   - Ouvrez l'URL affichée sur votre téléphone
   - Format : http://192.168.X.X:4000/preview

5. ARRÊTER LE SERVEUR
   - Fermez la fenêtre de commande
   - Ou lancez "stop-server.bat"


🛠️ DÉPANNAGE
========================================

PROBLÈME : Le serveur ne démarre pas
SOLUTION : Vérifiez que le port 4000 n'est pas déjà utilisé

PROBLÈME : Impossible de se connecter depuis le mobile
SOLUTION : 
  - Vérifiez que vous êtes sur le même WiFi
  - Désactivez temporairement votre pare-feu
  - Utilisez l'adresse IP affichée dans la console

PROBLÈME : Les CSS/JS ne s'affichent pas
SOLUTION : Le serveur injecte automatiquement les CSS/JS en inline.
  Si ça ne marche pas, vérifiez que les chemins dans votre HTML
  sont relatifs (pas de "/" au début)


📁 STRUCTURE DES FICHIERS
========================================

Votre dossier d'installation contient :
  - server.js          : Le serveur Node.js
  - package.json       : Les dépendances
  - start-server.bat   : Lance le serveur
  - stop-server.bat    : Arrête le serveur
  - uploaded_site/     : Vos fichiers uploadés (créé automatiquement)


💡 CONSEILS
========================================

- Utilisez des chemins relatifs dans votre HTML
  ✅ Bon : <link href="css/style.css">
  ❌ Mauvais : <link href="/css/style.css">

- Le fichier index.html doit être à la racine de votre projet

- Les images fonctionnent avec les chemins relatifs normaux

- Pour tester plusieurs sites, videz le site actuel avant d'en uploader un nouveau


🆘 SUPPORT
========================================

En cas de problème, consultez les logs dans la console du serveur.

Pour plus d'informations : https://example.com


Bon développement ! 🚀
