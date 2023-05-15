# Installation et configuration de Visual Studio Code

## Installation

- Télécharger l'application depuis : https://code.visualstudio.com/
- Prendre la version Windows 64bits
- ATTENTION : cela peut prendre du temps ...
- Cela donne le fichier : VSCodeUserSetup-x64-1.78.2.exe
- Il s'agit de l'installeur au niveau User et non Admin

- Exécuter le fichier VSCodeUserSetup-x64-1.78.2.exe
- Cocher "Je comprends ...", cliquer sur Suivant
- Laisser le chemin proposé et cliquer sur Suivant
- Laisser le nom proposé du dossier Menu Démarrer et cliquer sur Suivant
- Cocher toutes les cases proposées et cliquer sur Suivant
- Décocher "Exécuter VSC" et cliquer sur Terminer.

L'installation de VSC est terminée.

Vérifier que l'on peut ouvrir un fichier texte du bureau avec VSC.

## Configuration

### Sauvegarder tous les fichiers ouverts sur Control+S

- Aller dans File / Préférences / Keyboard shortcuts
- Taper : Save all
- Editer le raccourci clavier et remplacer Control+K S par Control+S et valider par Entrée.

### Les Extensions

#### Live server

Cette extension permet de visualiser en temps réel, l'état d'un fichier HTML donné.

- Cliquer sur les carrés dans la partie gauche de l'écran
- Taper : Live Server
- Cliquer sur Installer
- Fermer la fenêtre de l'extension

- Créer un fichier index.html basique dans un répertoire de test
- Lancer Live Server en bas à droite : go live, le _navigateur par défaut_ s'ouvre ...
  - Au premier lancement de Live Server il faut cocher les deux cases du haut pour le firewall: Autoriser réseau local et entreprise.
  - Le fichier HTML devrait s'afficher dans le navigateur.
  - En modifiant légérement le fichier index.html, on constate après l'avoir sauvegardé que la modification s'affiche bien dans le navigateur.

#### Prettier - Code formatter

Cette extension permet de reformater le code.

- Cliquer sur les carrés dans la partie gauche de l'écran
- Taper : Prettier
- Cliquer sur Installer
- Fermer la fenêtre de l'extension

- Ouvrir le fichier des settings de VSC en appuyant Control + Maj + P
- Rechercher settings
- Sélectionner la ligne contenent : Preference open user settings JSON
- Ajouter les informations suivantes :

```
  "editor.defaultFormatter": "esbenp.prettier-vscode",
  "editor.formatOnSave": true,
  "editor.formatOnPaste": true
```

- Sauvegarder le fichier.

#### Rename Tag

Cette extension permet de renommer les balises d'ouverture et de fermeture en même temps.

- Cliquer sur les carrés dans la partie gauche de l'écran
- Taper : Auto Rename Tag
- Cliquer sur Installer
- Fermer la fenêtre de l'extension

## Références

- [Installation de VSC avec WeeForYou](https://youtu.be/1Z1JCuwXmiQ)
- [Configuration des extensions avec WeeForYou](https://youtu.be/CTz1vpJG68E)
- [Using Git with Visual Studio Code (Official Beginner Tutorial)](https://youtu.be/i_23KUAEtUM)
