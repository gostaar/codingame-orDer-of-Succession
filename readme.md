 	Objectif
Vous devez produire l’ordre de succession au trône britannique d’une liste de personnes données.
L’ordre est simple:
d’un descendant A, le suivant dans l’ordre est le premier enfant de A B.Ensuite
, le suivant est le premier enfant C de B s’il y en a et ainsi de suite.
Si C n’a pas d’enfant, alors le suivant est le deuxième enfant de B D.Puis
les enfants de D s’il y en a. Puis le troisième enfant de B E... puis le deuxième enfant de A F...

Dessinons-le avec un arbre:

 A1
 ┌─┴─┐
 B2 F6
 ┌──┼──┐
 C3 D4 E5


Vous voyez l’ordre de succession: commencez à gauche de l’arbre, marchez jusqu’au niveau suivant chaque fois que possible sinon continuez vers la droite. Répétez l’opération jusqu’à ce que tout l’arbre soit couvert.
Ainsi, l’ordre est A-B-C-D-E-F.

En fait, dans les frères et sœurs de la même personne, les descendants mâles sont ordonnés avant les descendants femelles. Par exemple, si l’ordre de naissance des enfants (M pour mâle, F pour femelle) est Fa Ma Me Fe alors l’ordre de succession dans ces frères et sœurs est Ma Me Fa Fe.

Règles
d’ordre(a) par ordre de génération
(b) par ordre de sexe
(c) par ordre d’âge (année de naissance)

Règles
de sortie(a) exclure les personnes décédées (mais inclure les frères et sœurs des personnes décédées)
(b) exclure les personnes catholiques (mais inclure les frères et sœurs des personnes catholiques)

Notez que ce puzzle a été écrit en juin 2017 (certaines personnes pourrait être mort depuis cette date).

Entrées
Ligne 1 : Le nombre de personnes
Suivant n lignes: Nom Parent Année de naissance Année de décès Religion Sexe

Si le peuple n’est pas mort, l’année du décès est remplacée par le trait d’union -.n
Sortie
Un nom par ligne, dans l’ordre de succession au trône : d’abord la Reine, puis tous ses descendants.
Contraintes
Exactement une personne n’a pas de parent (le nom du parent est remplacé par le trait d’union -).
Il n’y a pas deux frères et sœurs du même sexe d’une personne qui ont la même année de naissance.
1 ≤ ≤ 100n
Exemple
Entrées
6
Elizabeth - 1926 - Anglican F
Charles Elizabeth 1948 - Anglican M
William Charles 1982 - Anglican M
George William 2013 - Anglican M
Charlotte William 2015 - Anglican F
Henry Charles 1984 - Anglican M
Sortie
Elizabeth
Charles
William
George
Charlotte
Henry
