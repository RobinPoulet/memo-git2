# memo-git2
Mémo GIT

Vérifier sa version de GIT
$ git - - version

Définir son nom : 
$ git config - - global user.name « mon nom »

Définir mon adresse mail :
$ git config - - global user.email « mon email »

Repo = dépôt = collection de fichiers liées à un projet

Activer Git pour un répertoire
$ git init 

Créer un nouveau dossier
$ mkdir nomdudossier

Naviguer dans un dossier
$ cd nomdudossier

Lister les éléments dans un dossier
$ ls

Vérifiez l'état des modifications dans un dépôt
 $ git status

Afficher les modifications apportés aux fichiers
$ git diff

Ajouter les modifications d'un fichier à soumettre
$ git add <FILENAME>

Pour ajouter toutes les modifications d'un seul coup
$ git add .

Pour soumettre les modifications que vous avez ajoutées avec un court message décrivant les modifications
$ git commit -m "your commit message"

Afficher le numéro et le nom des commits
$ git log --pretty=oneline

La commande checkout permet de faire plusieurs choses

Passer de branche en branche (on en parlera dans un prochain chapitre)
Revenir sur un fichier par rapport à un commit
Revenir sur un commit

git checkout <commit>
 
 revert
Revert permet d'inverser un commit.

git revert <commit>
 
 reset
Tout comme la commande checkout, la commande reset permet de faire plusieurs choses à la fois. En revanche il faudra faire très attention lors de l'utilisation de cette commande car elle altère l'historique et peut dans certains cas supprimer vos modifications (si vous voyez --hard, vérifiez 6 fois ce que vous voulez faire).

git reset <fichier>
 
Supprime un fichier de la zone de staging, mais ne supprime pas les modifications qui sont faites

git reset

Supprime tous les fichiers de la zone de staging, sans supprimer les modifications.

git reset --hard

revenir d'une branche head sur la branche master

$ git checkout master

créer une étiquette
$ git tag -a v1.4 -m 'ma version 1.4'

Lister vos étiquettes
$ git tag
