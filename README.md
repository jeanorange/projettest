
ELÉMENTS REPRIS D'UNE CONTRIBUTION FORMUM

Git à été crée par Linus Torvalds (Linux) Git est un modèle distribué
Un commit est une suite de modification accompagné d'un message
On peut faire un commit vide et on peut très bien ne pas mettre de messages.


Un repository est un dossier de projet sur GITHUB
un clonage permet cloner un dépôt ou une partie d'un dépôt. Cela va créer un nouveau projet git (comme avec un git init), créer une remote (comme avec git remote) récupérer les objets git (comme avec git fetch), et mettre à jour le dossier qui contient git à un commit précis (comme avec git checkout)
Un gist>est une façon de partager son code gist est un service de github comparable à pastbin mais avec de la gestion de version basé sur git.


Une remote c'est une URI (une addresse) permettant d'accéder à dépôt distant.
Origin c'est le remote par défaut

 fichier .gitignore et indiquez dedans le nom des fichiers
 .gitignore permet de dire à git d'ignorer certain fichier ou dossier.
 
Pull request  c'est un mécanisme propre à github ou d'autre outil de gestion de versions hébergé
Fork permet de récupérer un repository sur GITHUB et de le mettre sur mon compte GITHUB
 
# Création nouveau dossier de projet :
mkdir mon_projet
cd mon_projet/
git init
#Création nouveau fichier :
touch un_fichier.md
git add un_fichier.md ((indexe le fichier pour le suivre))
git commit ??? « Ajout de mon fichier »
-a = ajoute tous les fichiers présent dans l'index au commit
-am = applique les paramêtres a et m (ajout index et message)
-m = message

#Gestion du projet 
git status = voir le statut du projet
git log = voir l'historique des modifications
ls = permet de liste les fichiers

#Gestion du fichier dans VIM 
cat un_fichier.js = voir le contenu du fichier
vim un_fichier.md = rentrer dans l’éditeur de texte
sortir de vim sélectionné un emplacement après le dernier caractère et tapez :x

#Se déplacer dans les commit
git checkout SHA = se positionner sur un ancien commit
git checkout master = revenir sur le dernier commit
 
#Synchronisation GIT LOCAL WEB
git clone URL = récupérer un clone d'un GIT en ligne
git push origin master = envoi sur GITHUB
git pull origin master = récupère sur GITHUB
 

#Gestion des branches
git branch = permet de voir sur quelle branche on se trouve
git branch ma_branche = création d'une branche
git checkout ma_branche = se positionne sur la branche choisi
git checkout -b ma_branche = créé et se positionne sur la branche choisi
git merge mon_fichier = Fusionne dans la branche sur las-quelle on se trouve la branche demander
git branch -d ma_branche = supprime la  branche
 
git blame mon_fichier = Savoir qui à modifier qu'elle ligne
git show SHA = Voir le contenu exact d'un commot
git stash = mettre de côté ses modifications de façon temporaire sans faire de commit
git stash pop = reprend ou j'avais fait appel à git stash
