# GIT

* lien cours : https://openclassrooms.com/fr/courses/2342361-gerez-votre-code-avec-git-et-github
* nouveau cours : https://openclassrooms.com/fr/courses/5641721-utilisez-git-et-github-pour-vos-projets-de-developpement
* lien installation : http://msysgit.github.io

## memento Git
0. **configuration :**  
    `git config --global user.name "votre nom ou pseudo"`  
    `git config --global user.email "votre@email.com"`

1. **intialisation :**  
    `mkdir newdir` & `git init`

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
    * navigateur : utiliser l'option "clone URL" sur la page du repository  
    * terminal : `git clone https://github.com/facebook/react.git`(exemple avec react.js)

2.  **créer un repository github :**  
    * navigateur : le créer sur https://github.com/user/ (user est l'identifiant github)  
    * puis cloner le repository (voir ci-dessus)

3. **envoi/récupération de modifications :**   
    * envoi : `git push origin master` & `git log`  
    * récupération : `git pull origin master`

4. **création de branches :**   
    * création : `git branch new_branch`  
    * déplacement : `git checkout new_branch` | `git checkout master`
    * création + déplacement : `git checkout -b new_branch`
    * liste : `git branch` (* indique la branche active)

5. **fusion de branches :**  
    * de B sur A : `git checkout brancheA` & `git merge brancheB`  
    * conflit : le message suivant apparait et résoudre le conflit
        `Auto-merging new.md`
        `CONFLICT (content): Merge conflict in new.md`
        `Automatic merge failed; fix conflicts and then commit the result.`  
        remarque : outil de gestion de conflit `git mergetool vimdiff` (vimdiff par exemple)

6. **auteur d'une modification :**   
    1. liste de toutes les modifs : `git blame filename.ext`  (affiche le SHA)
    2. détail du commit : `git show SHA` (ou début du SHA)


7. **ignorer des fichiers :**   
    1. créer un fichier `.gitignore`
    2. éditer pour ajouter fichiers à ignorer (exp : motdepasse.txt)


8. **pile temporaure de modifications :**  `git stash` & `git stash pop` | `git stash apply`  
9. **PR (Pull Request) :** (participer à un projet collaboratif)
    * regarder dans la doc projet les recommandations sur pull request
    * En général, dans le fichier README, avec un intitulé "Contributing" ou "Pull requests".
    1. faire un fork du repo auquel vous souhaitez contribuer (navigateur : github : fork):  
        - exemple https://github.com/oc-courses/intro-git-github`
        - `git clone https://github.com/votre-username/intro-git-github.git`
    2. faire les modifications :  
        - créer une nouvelle branche : `git checkout -b my-new-feature`  
        - commit des mofis : `git commit -m "added modifs"`
        - envoi de la nouvelle branche : `git push origin my-new-feature`
    3. proposer nos modifications au projet :  Pull Request
        sur notre fork GitHub, sur notre nouvelle branche, cliquez sur "Compare & pull request".



## PDF / en ligne
+ https://www.konectik.com/wp-content/uploads/2017/01/M%c3%a9mento-Markdown.pdf
+ https://www.azur-web.com/astuces/markdown-memento-balise
+ https://github.com/nirae/Memento-Syntax-Markdown/blob/master/memo.md
