# GIT

* lien cours : https://openclassrooms.com/fr/courses/2342361-gerez-votre-code-avec-git-et-github
* lien installation : http://msysgit.github.io

## memento Git
0. **configuration :**  
    `git config --global user.name "Votre nom ou pseudo"`  
    `git config --global user.email "votre@email.com"`

1. **intialisation :**  
    `mkdir newdir` | `git init`

2. **ajout de fichier :**  
    `git add memento.md` | `git add .` (. ajout de tous les fichiers du répertoire)  
    `git commit -m "ajout memento.md"` (-m commentaire)  
    `git commit -a -m "modif memento.md"` (-a met à jour fichier existant)

3. **lecture de l'historique :**  
    `git log `

4. **positionnements :**  
    * se positionner sur un SHA : `git checkout SHADuCommit`  
    * revenir au master : `git checkout master`  
    * annulation du dernier commit : `git revert SHADuCommit`  
    * modifier message du dernier commit : `git commit --amend -m "nw msg"` (avant le push uniquement)  
    * annulation de tous les changements : `git reset --hard‌` (avant le nouveau commit)

## memento GitHub

1. **récupérer un repository github :**    
    - navigateur : utiliser l'option "clone URL" sur la page du repository  
    - terminal : `git clone https://github.com/facebook/react.git`(exemple avec react.js)

2.  **créer un repository github :**  
    navigateur : le créer sur https://github.com/user/ (user est l'identifiant github)  
    puis cloner le repository (voir ci-dessus)

3. **envoi/récupération de modifications sur github :**   
    - envoi : `git push origin master` | `git log`  
    - récupération : `git pull origin master`

4. **création de branches :**   
        envoi : `git push origin master` | `git log`  
        récupération : `git pull origin master`

## PDF / en ligne
+ https://www.konectik.com/wp-content/uploads/2017/01/M%c3%a9mento-Markdown.pdf
+ https://www.azur-web.com/astuces/markdown-memento-balise
+ https://github.com/nirae/Memento-Syntax-Markdown/blob/master/memo.md
