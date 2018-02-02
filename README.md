PMDtodo

Projet de cours basé sur le site todomvc.com.
User stories

Définition des actions de l'utilisateur :

    En tant qu'utilisateur je peux ajouter une tache
    En tant qu'utilisateur je peux valider une tâche
    En tant qu'utilisateur je peux supprimer une tâche
    En tant qu'utilisateur je peux flitrer les tâches réalisés
    En tant qu'utilisateur je peux flitrer les tâches à réaliser
    En tant qu'utilisateur je peux supprimer toutes les tâches réalisées

Mise en place du projet

Etapes à suivre pour préparer le projet PMDtodo

    Initier un server Nodejs
    Lancer le serveur de base de données
    Créer la BDD MongoDB
    Créer une route front pour afficher une fichier index dans un dossier www
    Créer une route api qui renvoie en json l'objet { msg: 'Hello API' }

Configurer la base de données

Le but est de définir le-s model-s de données à utiliser pour l'application

        Combien d'informations faut-il enregister pour une tâche ?
        Comment une tâche est validée ?
        Comment une tâche est supprimée ?
        Comment les tâches sont filtrées ?

1. Combien d'informations faut-il enregister pour une tâche ?

Il faut 3 informations :

    _id: string
    state: boolean
    content: string

2. Comment une tâche est validée ?

Quand la propriété state est égale à true.
3. Comment une tâche est supprimée ?

Si la propriété state est égale à true, spprimer l'objet de la base de données

    Connaître la propriété _id de l'objet
    Créer une route api pour supprimer l'objet de la BDD

4. Comment les tâches sont filtrées ?

Je dois sélectionner tous les objets et n'afficher que ceux dont la propriété state est égale à true (ou false)

    Créer une route api pour sélectionnher les tâches
