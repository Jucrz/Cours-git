Pour créer une branch vous pouvez utiliser la commande :

git branch Nomdevotrebranch

Et pour voir la liste de toute vos branchs :

git branch

Pour vous deplacer d'une branch a une autre :

git checkout Nomdelabranch

Vous pouvez aussi créer une branch et vous deplacer dessus en une seule commande :

git checkout -b Nomdelabranch

Pour supprimer une branch il suffit de taper :

git branch -d Nomdelabranch

Pour merge une branch dans une autre branch placez vous sur la branch a laquelle vous voulez ajouter les modifications de l'autre branch :

git merge Nomdelabranch

Et pour faire un commit sur le merge de la branch vous pouvez utiliser :

git merge Nomdelabranch --no-ff

Vous pouvez aussi lister toute les branch pas merger :

git branch --no-merged

Si vous voulez changer de branch et que vous ne voulez pas faire de commit vous pouvez juste enregistrer ce que vous avez fait puis changer de branch :

git stash

Vous pouvez lister les stash d'une branch avec la commande :

git stash list

On peut recuperer ce qui était dans un stash et l'appliquer avec :

git stash apply

Et on peut supprimer ce qui était dans la remise :

git stash drop 

Vous pouvez créer des tags annotés :

git -a v1.0 -m "Descriptif du tag" 