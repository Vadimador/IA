IA, conception et fonctionnement  

 

L’IA se décompose en plusieurs processus dirigés par un programme "noyau" (le main) Les différents processus sont : 

L'objetisation 

La conceptualisation 

L’analyse 

L'association 

Le processus d'objectif et d'action 

 

I/ l'objet 

 

Le premier processus est celui qui va transformer les sens/capteurs en série d'objets possédant des caractéristiques, des informations de même genre pour chaque type d'objet. Il n’est pas nécessaire de leur donner un nom pour les différencier, les caractéristiques sont là pour ça mais ces caractéristiques sont rassemblée sous la même enseigne  

Par exemple la caméra est l’objet sensoriel, mais chaque image va être converti en objet, ce seront par exemple des pixels avec comme caractéristique la couleur, la position sur l’écran ainsi que le moment où il a été capturé. Le type de l’objet permet de faire la différence entre l’objet issu de la caméra et celui issu du micro. Sa nature étant bien évidemment d’être un objet.  

On suppose que chaque objet est garde en mémoire (on pourra simplifier certains aspects pour ne garder que ce qui est vraiment utile plus tard) 

 

Mais revenons un peu sur ce que sont les caractéristiques, que sont-elles ? Ce sont des informations relatives à un objet ou à un concept (c’est relativement la même chose comme vous le verrez).  Chaque objet du même type possède les mêmes caractéristiques, seul leur contenu diffère. Ce contenu peut prendre autant de forme que possible (entier, tableau...). Mais ce contenu peut être interprété de deux façons différentes en fonction de comment la caractéristique a été créé. En effet on peut différentier deux types de caractéristique : 

Simple : une caractéristique simple est une caractéristique dont la valeur ne permet que de différentier l’égalité ou non de ce caractère. C’est à dire que la valeur en elle-même ne signifie rien de particulier. 

Exemple : Le caractère position de notre pixel, s’il est simple alors il peut se traduire par un simple entier dont la valeur ne correspond à rien de particulier. Le 1 et le 2 ne correspondent pas forcément à deux pixel cote à cote mais peut désigner un pixel situé à chaque extrémité de l’écran. 

Complexe : Est complexe une caractéristique dont la valeur peut être traité relativement aux autres valeurs possibles de la caractéristique. 

Suite de l’Exemple : En revanche s’il est complexe la valeur traduira des coordonnées précise du pixel et peut être comparé relativement aux autres positions des pixels. 

 

II/ Conceptualisation 

 

A partir des objets qu’il a gardé en mémoire le programme va créer de nouveaux objets appelés concept. Le concept est créé selon un certain mode, le plus simple étant de comparer une caractéristique avec la même caractéristique des autres objets pour regrouper ceux qui ont la même valeur. Il possède en plus de cela de la même façon que les objets des caractéristiques. 

Pour l’instant on peut se limiter à deux modes génériques de conceptualisation, un mode Identité/égalité (les caractéristiques sont égales) et un mode approximation (les caractéristiques se ressemblent) 

la particularité du système de conceptualisation réside dans les niveaux de conceptualisation, en effet on ne se contente pas de regrouper les objets en concept, en regroupe aussi les concepts eux-mêmes. Ainsi si le concept de niveau 1 regroupe aux moins deux objets les concepts de niveau supérieur regroupe des éléments de niveau inférieur (on appel concept de niveau n le concept qui possède comme concept de plus haut niveau n-1) Ainsi le concept de niveau 2 regroupe au moins deux éléments dont un concept de niveau 1 plus un autre éléments de niveau inférieur ou égal (un objet est donc de niveau 0).  

Mais pour pouvoir regrouper des concepts et des objets entre eux il faut pouvoir comparer des caractéristiques communes. D’où l’importance de nommer les caractéristiques. Malgré la différence de type de deux objets qui devrait changer la pluspart des caractéristiques on en retrouve tous de même des communes, commune même à tous les éléments de tous niveau. Parmi elles on peut retrouver la nature (objet, concept de niveau n etc...) 

 

 

III/ Analyse 

 

Pourtant juste regrouper les objets et les concepts à partir de leurs caractéristiques ne suffira probablement pas, il faut générer plus d’information à pouvoir traiter. C’est le rôle de ce processus, générer des caractéristiques à des éléments à partir de leurs caractéristiques et de celle d’autres objets qui leurs sont associé (que ce soit par association ou par le biais de concept qui les relie). Pour donner une idée de son fonctionnement voici la présentation succincte de deux fonctions qui pourraient lui appartenir : 

 

Simplification : regroupe les concepts simples (qui ne prennent en compte qu’un seul caractère) en concepts complexes. Par exemple les concepts qui possèdent exactement les mêmes objets peuvent être réunis entre eux 

 

Evolution : création d’un concept complexe dont ses composant voient évoluer une de leurs caractéristiques de la même façon tout en en gardant au moins une de fixe. 

 

 

IV/ L’association 

 

C’est un processus qui va associer les différents concepts entre eux en ajoutant de nouvelles caractéristiques (qui sont autant d'information a traiter en plus) Il ya alors plusieurs types d’association. Par exemple il y a l’association logique d’implication qui va utiliser la caractéristique de présence des concepts pour déterminer si un concept en implique un autre et va stocker cette information dans une nouvelle caractéristique qui se nommerait l’implication regroupant tous les concepts implique par celui qui possède la caractéristique d’implication. 

 

V/ Objectif et action 

 

Mais cette IA en plus de comprendre doit pouvoir agir et ce en suivant un objectif défini. Pour cela les processus d’objectif et d’action devront gérer les actions a effectuer afin d’atteindre un ou plusieurs concepts. C’est-à-dire qu’ils vont utiliser les processus d’association afin de parvenir au concept cible. Pour cela ils procéderont de la même manière que précédemment en ajoutant en premier lieu des caractéristiques donnant les i formations des concepts atteignable en utilisant les fonctions d’action de l’IA ainsi que des caractéristiques donnant les concepts cible. Cela signifie qu’il doit rendre « présent » un certain nombre de concepts. 

 
