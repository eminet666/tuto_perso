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
    navigateur : utiliser l'option "clone URL" sur la page du repository
    terminal : `git clone https://github.com/facebook/react.git`(exemple avec react.js)

6. liens : `[texte du lien](url_du_lien "texte pour le titre, facultatif")`
    (pas d'espace entre le crochet fermant et la parenthèse ouvrante)

7. images : `![Texte alternatif](url_de_l'image "texte pour le titre, facultatif")`
    (pas d'espace entre le crochet fermant et la parenthèse ouvrante)

## PDF / en ligne
+ https://www.konectik.com/wp-content/uploads/2017/01/M%c3%a9mento-Markdown.pdf
+ https://www.azur-web.com/astuces/markdown-memento-balise
+ https://github.com/nirae/Memento-Syntax-Markdown/blob/master/memo.md
