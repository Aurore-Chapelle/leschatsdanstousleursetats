# Directus local

## Mise à jour de npm

Installation de curl si besoin

`sudo apt install curl`

Téléchargement et installation de nvm

`curl https://raw.githubusercontent.com/creationix/nvm/master/install.sh | bash`

Mettre nvm en raccourci et faisant les 3 commandes suivantes OU relancer un terminal

`export NVM_DIR="$HOME/.nvm"`

`[ -s "$NVM_DIR/nvm.sh" ] && \. "$NVM_DIR/nvm.sh" `

`[ -s "$NVM_DIR/bash_completion" ] && \. "$NVM_DIR/bash_completion"`

Pour voir les versions node disponibles

`nvm ls-remote`

Installer la dernière

`nvm install 19.7.0`

Utilisation de la dernière. Potentiellement, il faudra gérer des conflits

`nvm use --delete-prefix v19.7.0`

## Installation

Installer un template grace à la commande : 

`npm init directus-project directus`

Il demande s'il continue, taper `y` puis "Entrée".

Attendre le téléchargement complet

Choisir la base de données `SQLite`.

Database File Path : "Entrée" sans rien taper d'autre

Compte admin : admin@example.com
Mot de passe : 1234

## Lancement 

Se placer dans le dossier `directus`

`cd directus`

Installer les dépendances :

`npm install`

Lancer le serveur : 

`npx directus start`

Aller sur chrome :

`http://0.0.0.0:8055/`

## Connexion

Utiliser l'email `admin@example.com` et le mot de passe `1234`