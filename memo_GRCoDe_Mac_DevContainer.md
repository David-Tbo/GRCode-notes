**Memo_GRCoDe_Mac_DevContainer.md** 

*Suite du mémo initial "Guide d'équivalence GRCoDe sur macOS"*

---

## Synthèse de la configuration

* **Objectif :** Reproduire l'environnement de développement conteneurisé d'entreprise (GRCoDe) sur un Mac personnel.
* **Architecture retenue :** Environnement local via l'extension Dev Containers et Docker Desktop (alternative sans VPN ni accès serveur distant).

### Étapes réalisées

* **Configuration préalable de l'environnement macOS :**
* Installation de VS Code en anglais et de l'extension Remote-SSH.
* Ajustement des raccourcis clavier macOS pour la gestion du clavier Logitech.
* Installation et démarrage de Docker Desktop sur macOS.


* **Configuration de VS Code et Dev Containers :**
* Installation de l'extension **Dev Containers** (Microsoft) dans VS Code.
* Création d'un dossier de travail local ouvert dans VS Code.
* Ajout des fichiers de configuration via la palette de commandes (`Cmd + Shift + P` > *Dev Containers: Add Development Container Configuration Files...*).
* Choix de la portée : *Add configuration to workspace...*.


* **Sélection et construction de l'image :**
* Modèle choisi : **Docker-in-Docker** (version `latest`).
* Options activées : Support ZSH et version OSS Moby.
* Fichier optionnel inclus : `.github/dependabot.yml` pour le suivi des dépendances.
* Génération du fichier `devcontainer.json` à la racine du projet.
* Lancement de la construction du conteneur via la commande *Reopen in Container*.
