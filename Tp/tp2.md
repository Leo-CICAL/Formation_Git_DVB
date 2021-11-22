# Mini TP Git 

(Oui je l'ai écrit en anglais, ça vous fait bosser en encore plus <3)

Travailler en Groupe ! Les branches, les merge, les reset 

## Mini-Project 1: Les Branches

## Step 1

### Summary

Dans cette étape, vous allez créer une branche, réaliser des modifs puis les push.

### Instructions

* Allez sur ce repo <a href="https://github.com/Leo-CICAL/Formation_Git_DVB">GitHub</a>.
* Clonez-le sur votre ordinateur.
* Vous allez créer votre première branche ! Allez dans le dossier cloné, et tapez `git branch`.
* Pour créer votre branche : `git branch nomdelabranche`
* Pour entrez dans la branche : `git checkout nomdelabranche`
* Pour supprimez la branche : `git branch -d nomdelabranche` (si aucune modif)
* Pour supprimez la branche : `git branch -D nomdelabranche` (si modifs dedans)

J’ai modifié la branche principale, mais j'ai pas encore commit  !

-> git status
-> git stash
-> git status
-> git stash apply (la dernière)

git stash list
git stash apply stash@{0}

J’ai modifié la branche principale, mais j'ai commit !

-> git log (se seouvenir de l'id (les 8 premiers char))
-> git reset --hard HEAD^
-> Créer une nouvelle branche
-> git reset --hard ca83a6df

Fichier oublié dans le commit :

-> git add FichierOublie.txt
-> git commit --amend --no-edit

Commit pushé alors que pas bon !

-> git revert HEAD^

Nous avons maintenant reverté notre dernier commit public et cela a créé un nouveau commit d'annulation. Cette commande n'a donc aucun impact sur l'historique ! Par conséquent, il vaut mieux utiliser  git revert  pour annuler des changements apportés à une branche publique, et git reset  pour faire de même, mais sur une branche privée. 

Gardez à l'esprit que Git revert sert à annuler des changements commités, tandis que Git reset HEAD permet d'annuler des changements non commités.

Toutefois, attention, Git revert peut écraser vos fichiers dans votre répertoire de travail, il vous sera donc demandé de commiter vos modifications ou de les remiser.




## Step 2

### Summary

