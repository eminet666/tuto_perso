# TERMINAL

* lien cours : https://openclassrooms.com/fr/courses/6173491-apprenez-a-utiliser-la-ligne-de-commande-dans-un-terminal/6349461-decouvrez-le-terminal
* lien cours (avancé) : https://openclassrooms.com/fr/courses/43538-reprenez-le-controle-a-laide-de-linux/37813-la-console-ca-se-mange


## synthèse
    * `pwd` : permet d’afficher le répertoire courant  
    * `ls -a` : l’option -a affiche également les fichiers et dossiers cachés   
    * `ls` : permet d’afficher le contenu d’un répertoire  
    * `cd dossier` : permet de se déplacer à l’intérieur d’un répertoire  
    * `ls -l` : l’option -l modifie l’affichage pour rajouter de nombreuses informations  
    * `mkdir dossier` : permet de créer un dossier  
    * `touch nomFichier` : permet de créer un fichier  
    * `mv source destination` : permet de déplacer des éléments  
    * `\*` : caractère substitut pour n’importe recherche  
    * `cp source destination` : permet de copier des éléments  
    * `cp -r` : l’option -r permet de copier un répertoire  
    * `rm fichiers` : permet de supprimer des fichiers  
    * `rm -r dossiers` : l’option -r permet de supprimer des répertoires  
    * `man commande` : permet d’afficher le manuel d’une commande  
    * `cat/less/more nomFichier` : permet d’afficher le contenu d’un fichier  
    * `>` : permet de rediriger le résultat d’une commande vers un fichier  
    * `grep motif chemin` : permet de faire des recherches dans des fichiers   

## installation (windows)
    * [Cygwin (uk)](https://www.cygwin.com/install.html) ok |
    * [Cygwin (fr)](http://migale.jouy.inra.fr/?q=fr/cygwin-install) ok |
    * [shell Bash Windows](https://docs.microsoft.com/fr-fr/windows/wsl/install-win10) pb |
    * [shell Bash Windows (alternative)](https://korben.info/installer-shell-bash-linux-windows-10.html) pb  
    Rem : l'invite de commande ou le powershell ne sont pas des terminaux (mais proches)

## accès
* sous Linux : "applications > Accessoires > Terminal" | "Ctrl + Alt + T"  
* sous Mac : "applications > Utilitaires > Terminal.app"  
* sous Windows : icone "Cygwin64 Terminal"

## commandes
    * répertoire courant : `pwd` (print workin directory) | `pwd --help`
    * contenu du répertoire courant : `ls` | `pwd -l` detaillé | `pwd -a` avec fichiers cachés
    * changement de répertoire : `cd rep` | `cd..` parent
    * création de répertoire : `mkdir rep` | `mkdir "rep rep"` | `mkdir rep\ rep` (si espace dans nom)
    * déplacer un fichier : `mv fichier.txt dossier/` | `mv dossier/fichier.txt .`
    * déplacer plusieurs fichiers : `mv fichier*.txt dossier/` (* est appelé joker)
    * copier fichier ou rep :  
        `cp fichier.txt dossier/` (dans un rep) |  
        `cp fichier.txt fichier2.txt` (avec un autre nom)
    * copier répertoire et sous répertoires : `cp -r dossier/ newdir` (-r récursive)
    * supprimer fichier : `rm fichier.txt`
    * supprimer répertoire et sous répertoires : `rm -r dossier/` (-r récursive)
    * afficher manuel d'une commande : `man commande` (q pour sortir)
    * afficher aide d'une commande : `commande --help`
    * afficher le contenu d'un fichier : `cat fichier.txt` | `less fichier.txt` (paginé)
    * redirection d'une commande : `ls -la > fichier.txt`
    * chercher une chaine dans un fichier : `grep txt *` (chaine cible)
