# COURS GIT

Pour configurer GIT : 

* aller sur https://git-scm.com/ , télécharger et installer git

* Créer un compte github ou gitlab

**git config --global user.name "Nom Prenom"**

**git config --global user.email "votre mail**

Pour vérifier la config on fait :

**git config --global --list** ==> user.email=votremail@mail.com user.name=Votre nom et prénom


# DEPOT LOCAL
Comme son nom l'indique , c'est un dépôt qui se trouve sur notre ordinateur

Initialisation du dépôt git

**git init**

Afin de dire à git quel fichier doit être suivi

**git add SUIVI_DU_NOM_DU_FICHIER**

git add accueil.html


Afin de vérifer le statut de l'ajout on fait :

**git status**

**git add -A** OU **git add .** pour ajouter tous les fichiers

Pour faire un commit
**git commit -m"Premier commit"**

Pour voir l'historique des modifications
**git log**

Pour modifier un commit 
**git commit --amend**

Dans VIM 

Taper i pour faire une modification

utiliser les touches de direction pour se positionner sur le message. A la fin de la modification, taper ESC ou ECHAP ==>: ==>w ==>q ==>!

w ==> permet d'enregister les modification
q ==> permet de quitter 
! ==> permet de forcer l'action

Donc on enregiste, on quitte et on force l'action

# DEPOT DISTANT

**echo "# coursgit" >> README.md**
**git init** ==> Pour initialiser le dépot
**git add README.md** == n> Pour créer le fichier README.md
**git commit -m "first commit"** ==> Ajout du commit + le message
**git branch -M main** ==> Pour envoyer sur la branche principale(main)
**git remote add origin https://github.com/Kalo-Green/coursgit.git** ==> ajout du dépot distant
**git push -u origin main** ==> Transférer le dossier distant

Si plus tard on fait des modifications et qu'on veut envoyer nos modification sur notre dépôt distant, on fera :

**git add .** ou **git add -A**

**git commit -m "Message du commit"**

**git push**