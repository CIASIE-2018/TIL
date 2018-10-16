Si tu es dans ta branche et tu souhaites pull ce qu'a fait quelqu'un sur le master sans pour autant push ce que tu fais en ce moment 
il faut tout d'abord :


# I. Stocker ce que tu es en train de faire dans un espace à part

Grâce à la commande
''' git stash '''
vous pouvez envoyer toutes vos modifications en cours dans un espace à part (le temps de pull).
(Vous pouvez vérifier qu'il n'y a plus aucun changement grâce à ''' git status ''')


# II. Récupérer le master

tout d'abord faire un ''' git fetch '''
puis un ''' git rebase origin/master '''

Ainsi vous avez maintenant récupérer les infos du master mais il n'y a plus vos modifications.


# III. Récuperer les modifications

''' git stash apply ''' permet de retrouver toutes vos modifications
(faites un ''' git status ''' pour vérifier)
