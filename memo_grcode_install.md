# GRCoDe — Guide d'utilisation et de prise en main

Ce mémo décrit les étapes d'installation initiale ainsi que le workflow quotidien pour travailler dans l'environnement conteneurisé GRCoDe depuis un poste Windows d'entreprise.

---

## Phase 1 : Première installation (Initial Setup)

* **Initialisation depuis le terminal Windows :**
* Exécuter la commande d'installation fournie par l'entreprise :
`envinstall install grcode:1.32.0`


* **Authentification et enregistrement :**
* S'authentifier auprès du GitHub d'entreprise (SGitHub) en saisissant le code demandé.
* Confirmer son adresse e-mail publique d'entreprise pour valider l'enregistrement et la création de l'environnement distant.


* **Connexion depuis Visual Studio Code :**
* Ouvrir VS Code sur le poste Windows local.
* Ouvrir la palette de commandes avec le raccourci `Ctrl + Shift + P`.
* Rechercher et exécuter la commande : `Remote-SSH: Connect to Host...`
* Sélectionner l'hôte **`grcode`** dans la liste proposée.


* **Configuration de la plateforme distante :**
* Lorsque VS Code demande de choisir la plateforme système de l'hôte, sélectionner **Linux**.
* Patienter pendant le téléchargement et l'initialisation automatique du composant **VS Code Server** dans le conteneur distant.


* **Validation de la connexion :**
* Vérifier que l'indicateur situé en bas à gauche dans la barre d'état de VS Code affiche désormais **`SSH: grcode`**.


* **Accès au dossier de travail :**
* Aller dans le menu **Fichier > Ouvrir le dossier...** (ou `Ctrl + K` puis `Ctrl + O`).
* Sélectionner le répertoire souhaité dans l'arborescence Linux du conteneur.
* (Optionnel) Ouvrir un terminal intégré via **Terminal > Nouveau terminal** pour exécuter vos commandes directement dans l'environnement conteneurisé.

---

Une fois que l'environnement distant est créé et configuré, **vous n'avez généralement pas besoin de relancer la commande d'installation complète** à chaque fois. L'environnement reste provisionné sur le cloud de l'entreprise.

Voici comment se déroule une vraie reprise de session standard :

---

## Phase 2 : Quick Start (Utilisation au quotidien)

* **Lancement direct de VS Code :**
* Ouvrir directement **Visual Studio Code** sur votre poste Windows (sans repasser par le terminal ni retaper la commande `envinstall`).


* **Connexion à l'hôte distant :**
* Ouvrir la palette de commandes avec le raccourci `Ctrl + Shift + P`.
* Saisir et valider : `Remote-SSH: Connect to Host...`
* Sélectionner l'hôte **`grcode`** (qui est mémorisé par VS Code).


* **Vérification et test :**
* Attendre que l'indicateur en bas à gauche affiche **`SSH: grcode`**.
* Ouvrir le terminal intégré (`Ctrl + Shift + ` `) et tester directement : `docker --version`
