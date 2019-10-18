Afin de consulter votre historique de commit vous pouvez utiliser la commande :

git log

Si vous les voulez les voir en plus court :

git log --oneline

Et sans pagination :

git --no-pager log --oneline

Et pour voir par exemple les 3 derniers commits vous pouvez utiliser la commande :

git --no-pager log -3 --one-line

Vous pouvez aussi voir les commits d'un auteur en particulier :

git log --author "Pseudonyme"

On peut aussi consulter les commits a partir d'une date :

git log--since=1.day
git log --before="2019-09-01"

Ou encore les commits d'un fichier en particulier :

git log Nomdufichier

Ainsi que ses changement :

git log -p Nomdufichier

Vous pouvez voir précisement les nombres de lignes modifiés dans un fichier :

git log --stat Nomdufichier

Vous pouvez aussi recherche un therme en particulier dans les commits:

git log -E -i --grep="Motrecherché"

Il peut aussi etre utile de savoir qui a fait les modifications sur un fichier :

git blame Nomdufichier

Lorsque vous faites une modification dans un fichier vous pouvez voir ces dernières avant de l'indexer avec :

git diff

Si vous voulez voir les modifs d'un commit en arrière :

git diff HEAD~1

Si vous voulez voir les modifs entre le HEAD et un état antérieur du dépot vous pouvez utiliser :

git diff HEAD~3 HEAD

Vous pouvez voir les stats sur les différences opérées dans les fichiers : 

git diff --stat

Si vous voulez remettre le dépot dans l'état dans lequel il se trouvait juste avant une modification :

git restore Nomdufichier

Mais si on ajoute le fichier dans l'index il faut taper :

git restore --staged

Si vous voulez modifier le message du dernier commit que vous avez effectué :

git commit "Votre message" --amend --no-edit

Si vous voulez annuler votre dernier commit il faut utiliser la commande :

git reset HEAD-1

Si vous voulez l'annuler mais pas le perdre pour le mettre dans la staging area :

git reset --soft HEAD-1

Et si vous voulez totalement le supprimer il suffit d'utiliser :

git reset --hard HEAD-1 