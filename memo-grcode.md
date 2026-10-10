### **Mémo : Mise en route de l'environnement conteneurisé GRCoDe**

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