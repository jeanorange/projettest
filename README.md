Git à été crée par Linus Torvalds (Linux) Git est un modèle distribué
Un commit est une suite de modification accompagné d'un message
Un repository est un dossier de projet sur GITHUB
Un clonage permet de récupérer un repository sur sa machine
Un gist est une façon de partager son code
Un remote c'est une autre machine ou service
Origin c'est le remote par défaut
Pour ignorer des fichiers de configurations par exemple crée un fichier .gitignore et indiquez dedans le nom des fichiers
Pull request est processus qui consiste à proposer une suite de commits pour qu'ils soient acceptés dans un projet open source
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
-am = on à déjà fait un commit
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