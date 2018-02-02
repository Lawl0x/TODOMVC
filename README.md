# ToDo
Projet de cours basé sur le site todomvc.com

## User stories
Définitions des actions de l'utilisateur :
- [ ] En tant qu'utilisateur je peux ajouter une tâche
- [ ] En tant qu'utilisateur je peux valider une tâche
- [ ] En tant qu'utilisateur je peux supprimer une tâche
- [ ] En tant qu'utilisateur je peux afficher les tâches réalisées
- [ ] En tant qu'utilisateur je peux afficher les tâches à réaliser
- [ ] En tant qu'utilisateur je peux supprimer toues les tâches réalisées

## Mise en place du projet
Etapes à suivre pour préparer le projet PMDTodo
- [ ] Initier un server NodeJS
- [ ] Lancer le serveur de base de données
- [ ] Configurer la BDD MangoDB
- [ ] Créer une route `front` pour afficher un fichier `index` dans un dossier `www`
- [ ] Créer une route `api` qui renvoie en `json` l'objet `{ msg:'Hello API' }` 

## Configurer la base de données
Le but est de définir le-s model-s de données à utiliser pour l'application
- 1. Combien d'informations faut-il enregistrer pour une tâche ?
- 2. Comment une tâche est validée ?
- 3. Comment une tâche est supprimée ?
- 4. Comment les tâches sont filtrées ?

### 1. Combien d'informations faut-il enregistrer pour une tâche ?
Il faut trois informations :
- _id : string
- state : boolean
- content : string

### 2. Comment une tâche est validée ?
Quand la propriété `state` est égal à `true`.

### 3. Comment une tâche est supprimée ?
Si la propriété `state` est égal à `true`, supprimer l'objet de la base de données.
- [ ] Connaître `_id` de l'objet
- [ ] Créer une route `api` pour supprimer l'objet de la base de données

### 4. Comment les tâches sont filtrées ?
Je dois sélectionner tous les objets et n'afficher que ceux dont la propriété `state` est égale à `true` (ou `false`).
- [ ] Créer une route `api` pour sélectionner les tâches
