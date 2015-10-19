INSTALLER GIT
=============
GitHub est un outil de travail en ligne permettant de mettre en commun des modifications effectuées par plusieurs personnes sur un projet donné.

GitHub pour Windows: https://windows.github.com
GitHub pour Mac : https://mac.github.com
Git pour Linux - Solaris : http://git-scm.com

CONFIGURATION DES OUTILS
========================
Configurer les informations de l'utilisateur pour tous les dépôts locaux

**git config --global user.name "[nom]"**  
...

**git config --global user.email "[adresse email]"**  
...

**git config --global http.proxy http://192.168.1.17:8080**    (pour contourner proxy de l'école)
...

**git config --global –unset http.proxy**  
...

CRÉER/CLONER DES DÉPÔTS
=======================
Démarrer un nouveau dépôt ou en obtenir un depuis une URL existante
 
**git init [nom-du-projet]**  (nouveau dépôt)
...

**git clone [url]**  (cloner un dépôt existant)
...

EFFECTUER DES CHANGEMENTS
=========================
Consulter les modifications et effectuer une opération de commit

**git status**  (afficher les modifications)
...

**git add [fichier]**  (ajouter des modifications sur un fichier ; -a pour tous les fichiers du dépôt)
...

**git reset [fichier]**  (annuler les modifications sur un fichier)
...

**git diff**  (afficher les différences entre deux branches)
...

**git commit -m "[message descriptif]"**  (valider, finaliser la mofification de la branche et la nommer)
...

**git commit -a -m "[message descriptif]"**  
...

GROUPER DES CHANGEMENTS
=======================
Nommer une série de commits et combiner les résultats de travaux terminés

**git branch**  (afficher les branches existantes)
...

**git branch [nom-de-branche]**  (créer une nouvelle branche)
...

**git checkout [nom-de-branche]**  (changer de branche)
...

**git merge [nom-de-branche]**  (se placer dans le master pour pouvoir appliquer les modifications réalisées dans la branche)
...

**git branch -d [nom-de-branche]**  
...

VÉRIFIER L'HISTORIQUE DES VERSIONS
==================================
Suivre et inspecter l'évolution des fichiers du projet

**git log**  (donner les derniers messages descriptifs des commit)
...

**git log --follow [fichier]**  (donner les derniers messages descriptifs d'un fichier)
...

**git diff [premiere-branche]...[deuxieme-branche]**  (afficher les différences entre deux branches)
...

**git show [commit]**  
...

DÉFAIRE DES COMMITS
===================
Corriger des erreurs et gérer l'historique des corrections

**git reset [commit]**  (supprimer un commit)
...

**git reset --hard [commit]**  (supprimer un commit et ses modifications)
...

SYNCHRONISER LES CHANGEMENTS
============================
Référencer un dépôt distant et synchroniser l'historique de versions

**git fetch [nom-de-depot]**  (recuperer les informations à partir d'un dépôt distant sans l'avoir dans sa branche)
...

**git merge [nom-de-depot]/[branche]** 
...

**git push [vers --> alias d'un remote] [branche locale]**  (appliquer les modifications vers le dépôt distant)
...

**git pull [alias d'un remote] [sur --> branche locale]**  (= git fetch + git merge)
...

**git remote add mon_alias https://github.com/mon_login/spid-git.git**  
...
