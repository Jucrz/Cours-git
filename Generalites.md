Avant tout il faut définir un utilisateur Git pour pouvoir utiliser ce dernier. 

git config --global user.name Prénom

Vous pouvez mettre le pseudonyme que vous voulez a la place du prénom.
Il faut aussi définir son email avec la commande :

git config --global user.email Votre@email.fr

Si vous n'avez pas d'étieur définit ou si vous voulez le changer vous pouvez utiliser la commande :

git config --global core.editor Lenomdevotreéditeur

Si vous etes dans un dépot en particulier vous devez redéfinir votre pseudonyme et votre email dans
le fichier config du dossier .git/ puis ensuite utiliser les commandes suivantes:

git config --local user.name Prénom
git config --local user.email Votre@email.fr

Pour initialiser un projet git il faut utiliser la commande suivante :

git init 

Pour voir si tout est en ordre placez vous dans votre dossier versionné et tapez la commande:

git status

Vous pouvez l'utiliser exessivement pour voir si vous n'avez rien oublié dans vos modification 
Après avoir modifié un fichier il faut l'ajouter dans la zone index avec la commande:

git add Nomdufichier

Maintenant fait un "git status" vous pouvez voir que git connait votre fichier mais il demande de 
faire un commit un commentaire a votre modification vous utiliserez donc la commande :

git commit -m "Un commentaire qui décrit votre modification"

ou si vous voulez faire un commentaire plus en détail:

git commit

L'éditeur que vous avez définit plus haut s'ouvre et vous pouvez faire un commentaire mieux organisé et plus complet.
Ensuite vous pouvez vérifier si vous avez bien fait votre commit et voir la liste de tout vos commit avec la commande :

git log --oneline