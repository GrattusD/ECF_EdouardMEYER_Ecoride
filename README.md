Bienvenue dans le projet : ECF_EdouardMEYER_Ecoride


liste des stack utilisées et a installer pour le projet:

    - Installation de xampp version 8.2.12 pour utilisation de php 8.2.2, du serveur Apache (2.4.58) et MariaDB (10.4.32)
    - installation de node.js (version 22.14 (LTS)) et fnm (fnm install 22.14)
    - installation de git (version 2.48.1)
    - installation de composer (version 5.11.2)
    - installation de MongoDB (version 8.0.4)

Une fois le git clone effectué avec la commande:
    git clone https://github.com/GrattusD/ECF_EdouardMEYER_Ecoride.git
cd ECF_EdouardMEYER_Ecoride

il faut configurer le Front-End:
    aller dans le repertoire du front et installer les dépendances (npm install)
il faut aussi configurer le Back
    aller dans le repertoire Back-End (composer install)
Il faut ensuite démarrer MongoDB et configurer les paramètres dans le fichier backend/.env
    DB_MONGO_HOST=127.0.0.1
    DB_MONGO_PORT=27017
    DB_MONGO_DATABASE=ECF_EMEYER_Ecoride_Mongo
    DB_MONGO_USERNAME=
    DB_MONGO_PASSWORD=

L'étape suivante est la migration de la base de données avec Laravel
    php artisan migrate
s'il y a des seed (données initiales) dans le dossier backend/database/seeders, executer la commande 
    php artisan db:seed