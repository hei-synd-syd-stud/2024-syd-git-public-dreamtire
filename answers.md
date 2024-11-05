# Answers of Xavier Bondaz github-dreamtire

## Basics

### Task 1

Après avoir cloné un dépôt Git, le répertoire contient :

- **Les fichiers du projet** : ce sont les fichiers sources ou de configuration du projet, copiés depuis le dépôt distant.
- **Un dossier `.git`** : il s'agit d'un répertoire caché contenant tous les éléments nécessaires pour suivre l'historique du projet, comme les commits, les branches, et les objets Git. Il est essentiel pour le suivi de version.
- **Un dossier `img`** : il s'agit d'un répertoire pour les images.
- **Un fichier `.md`** : C'est le fichier sur lequel, je vais écrire les réponses du laboratoire.

### Task 2

- **git status** : indique que `README.md` est un "fichier non suivi" (untracked file), car il est dans le répertoire de travail mais n'a pas encore été ajouté au stage.
- **git log --oneline** : n'affiche aucun changement puisque `README.md` n'a pas été commité. Le fichier doit d'abord être ajouté au stage avec `git add`, puis commité pour apparaître dans l'historique des logs.

### Task 3

Après avoir exécuté `git add README.md`, la commande `git status` montre que `README.md` est désormais en "staged", prêt à être commité. Ce fichier n'est plus affiché comme un "fichier non suivi" mais comme un fichier "suivi" en attente de validation (commit).

### Task 4

`git status` montre maintenant que `README.md` a été modifié et est en attente d'ajout (dans la section des modifications non indexées). La version actuelle dans le stage est différente de celle du répertoire de travail. Pour inclure ces nouvelles modifications, il faut ajouter le fichier à nouveau avec `git add`.

### Task 5

- **Chaîne de caractères au début** : c'est un identifiant abrégé du commit (hash) qui permet d'identifier de manière unique chaque commit.
- **HEAD** : référence à la dernière révision ou commit actif dans le dépôt local, le point où se trouve l’utilisateur.
- **main** : la branche sur laquelle se trouve actuellement HEAD.
- **Après les parenthèses** : c'est le message de commit qui décrit les changements effectués dans ce commit.

### Task 6

- **En revenant sur le commit initial** : Git restaure le projet à l'état exact de ce commit. Certains fichiers et modifications récentes peuvent donc disparaître, car ils n'existaient pas encore à ce stade.
- **En revenant sur la branche `main`** : Git restaure l'état le plus récent du projet, incluant toutes les modifications récentes et les fichiers créés après le commit initial.

## Gitgraph

### Task 7

![Gitgraph](img/gitgraph.svg)

<style>
</style>

1)     Le nom de la branche

2)     Le short hash du commit

3)     Les informations de la branche, ici on voit qu’on a merge une branche qui s’appelle « feature-auth » dans la branche « develop »

4)     Le nom et l’adresse électronique de la personne qui a fait l’action

5)      C’est la version de la branche main

6)     C'est le commit final du projet : baa6795

7)     Le point de la branche « feature-auth » ou on a add un nouvel utilisateur qui est Carol

8)     C’est le merge de la branch « develop » avec la branche « main »

9)     C’est la branche « develop »

10)  C’est la branche « main »