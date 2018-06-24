# IA, conception et fonctionement :

L’IA se décompose en plusieurs processus dirigés par un programme "noyau" (le main)
Les différents processus sont :

- L'objetisation
- La conceptualisation
- L'association
- Le processus d'objectif et d'action

I/ l'objet

Le premier processus est celui qui va transformer les sens/capteurs en série d'objets possédant tous un nom différents ainsi que des caractéristiques, des informations de même genre pour chaque type d'objet.

Les caracteristiques ont :
-	Un nom
-	Une forme ( entier, tableau etc)
-	Un mode (simple ou compexe)l
Elles peuvent Etre :
-	Simples ( dont le valeur n´a aucune signification, n´est la que pour differencier des autres valeurs)
-	Complexes (dont la valeur peut etre utilisee pour pouvoir etre comparee aux autres )

On suppose que chaque objet est garde en mémoire (on pourra simplifier certains aspect pour ne garder que ce qui est vraiment utile plus tard)

II/ Conceptualisation

A partir des objets qu’il a garde en mémoire le programme va créer de nouveaux objets appelés concept. Le concept est créé selon un certain mode, le plus simple étant de comparer une caractéristique avec la même caractéristique des autres objets pour regrouper ceux qui ont la même. Chaque concept possède donc la liste des objets auquel il renvoi. Il possède en plus de cela de la même façon que les objets des caractéristiques. Pour résumer on a :

 Un mode de conceptualisation :
-	Identité/égalité (les caracteristiques sont egales)
-	Approximation ( les caracteristiques se ressemblent)
-	Autres ( a rajouter)

Il existe aussi des niveaux de conceptualisation, en effet on ne se contente pas de regrouper les objets en concept, en regroupe aussi les concepts eux-mêmes. Ainsi si le concept de niveau 1 regroupe aux moins deux objets les concepts de niveau supérieur regroupe des concepts et des objets de niveau inférieur. Ainsi le concept de niveau deux regroupe au moins 1 concept de niveau 1 avec un objet ou avec un autre concept de niveau 1. Mais pour pouvoir regrouper des concepts et des objets entre eux il faut pouvoir comparer des caractéristiques commune. Ainsi il existe des caractéristique commune a tous les objets et concepts de tous niveaux. Par exemple quelques caractéristiques communes : la nature ; la présence ( si le concept est présent en ce moment)


III/ L’association

C’est un processus qui va associer les différents concepts entre eux en ajoutant de nouvelles caractéristiques ( qui sont autant d'information a traiter en plus)  Il ya  alors plusieurs types d’association. Par exemple il y a l’association logique d’implication qui va utiliser la caractéristique de présence des concepts pour déterminer si un concept en implique un autre et va stocker cette information dans une nouvelle caractéristique qui se nommerait l’implication regroupant tous les concepts implique par celui qui possède la caractéristique d’implication.


IV/ Objectif et action

Mais cette IA en plus de comprendre doit pouvoir agir et ce en suivant un objectif défini. Pour cela les processus d’objectif et d’action devront gérer les actions a effectuer afin d’atteindre un ou plusieurs concepts. C’est-à-dire qu’ils vont utiliser les processus d’association afin de parvenir au concept cible. Pour cela ils procéderont de la même manière que précédemment en ajoutant en premier lieu des caractéristiques donnant les i formations des concepts atteignable en utilisant les fonctions d’action de l’IA ainsi que des caractéristiques donnant les concepts cible. Cela signifie qu’il doit rendre « présent » un certain nombre de concepts.

 

Autres fonctions a rajouter, idées d’améliorations par la suite :

-	Simplification : regroupe les concepts simples (qui ne prennent en compte qu’un seul caractere) en concepts complexes. Par exemple les concepts qui possèdent exactement les mêmes objets peuvent être réunis entre eux
-	Evolution : création d’un concept complexe dont ses composant voient évoluer une de leurs caractéristique de la même façon tout en en gardant au moins une de fixe.
