Module Git et Github

GIT:
C'est un logiciel.
C'est l'outil, il permet de travailler en local et de figer des instantanés de notre progression.
Cela permet de changer fondamentalement le code et de pouvoir reven,ir à la version qui nous allait bien si on n'est pas satisfaits
On peut ensuite éventuellement merger sa version avec la précédente si ça nous va.
Ce n'est pas réservé aaux développeurs. Cela peut fonctionner avec n'importe quel type de fichier. C'est du versionning.

Les alternatives à GIT : Microsoft team fondation server / Helix score / Subversion / AWS Codecommit


GITHUB:
Plate-forme WEB.
Permet de faire du collaboratif et de travailler en groupe sur du code.
FORK : Permet de copier le code de quelqu'un et d'apporter des modifications.
PULL : Partager et suggérer avec le propriétaire.
MERGE: Fusion de la modification avec le code du propriétaire.
Lorsque l'on fait une veille technologique sur les logiciels, regarder sur Github, le readme, le nombre de stars.


Les alternatives : Bilbucket



Commandes GIT :l
commit
branch
checkout
cherry-pick
reset
revert
rebase
merge

Pour créer une copie "git commit"
Pour créer des branches "git branch [nom]"
Pour mettre le curseur et avancer sur l'une des versions "git checkout [nom]"
Pour fusionner deux branches "git merge nom"
Pour fusionner en passant sur une autre branche "git rebase nom" est une bonne pratique. Cela permet d'avoir une vue séquentielle plutôt que du parallèle.
Pour aller pointer sur les parents ou grands-parents "git checkout [name branch]^"
Pour remonter plusieurs branches on peut utiliser le ~ et on donne le nombre de générations à remonter "git checkout HEAD~4"
Pour assigner une branche à un autre commit on peut utiliser "git branch -f main HEAD~3" bouge de force la branche main pour aller 3 parents au dessus de HEAD
Pour annuler un commit on peut utiliser la fonction "git reset HEAD^". On revient alors sur la version d'avant.
Une autre façon est de faire "git revert [branch]" pour créer un commit qui revient à la version d'avant.


Informations sur les commandes GitBash :
echo "# jkdfjgf" >> README.md    --> Avec cette commande on crée le fichier qui va être dans notre dossier local
git init       --> Une fois qu'on est dans le bon dossier on lui dit qu'on veut travailler dans Git
git add README.md      --> On met le fichier README dans la staging area. Si on veut mettre le dossier en entier "git add ."
git commit -m "first commit"       --> On crée la nouvelle version du ou des fichiers qui sont dans la staging area
git branch -M main        --> On change le nom de la branche principale.
git remote add origin https://github.com/Rodolphe-74/jkdfjgf.git         --> On écrit le chemin de notre repository
git push -u origin main       --> On envoie sur Github
git commit -a -m "text" permet d'envoyer tout le dossier lié à la branche main
git pull origin main récupère les fichiers non présents en local. 
Quand on veut résoudre des conflits, il suffit de pull le fichier sur le github et de gérer les conflits sur notre notePad ou notre fichier.

