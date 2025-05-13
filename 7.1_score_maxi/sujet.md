---
author: Nicolas Revéret
reviews: Franck Chambon, Sébastien Hoarau
title: Score maximal
---

# Score maximal

On place dans une urne $N$ boules portant chacune un numéro distinct de $1$ à $N$.

On tire une boule dans l'urne et l'on note son numéro avant de la remettre dans l'urne. Cette opération est répétée plusieurs fois.

À l'issue des tirages on obtient donc la liste des résultats : chaque valeur dans la liste indique combien de fois on a obtenu une valeur. Par exemple, si on effectue 7 tirages parmi 6 boules numérotées de 1 à 6, on peut obtenir les résultats suivants :

```python
# valeur    1  2  3  4  5  6
resutats = [2, 0, 0, 3, 2, 0]
```

On définit le **score maximal** associé à un résultat comme étant égal à la valeur maximale du produit (nombre de boules tirées fois numéro de la boule).

Pour les résultats précédents, on a obtenu :

* 2 boules de valeur 1 : le score est de $2 × 1 = 2$ ;

* 0 boules de valeur 2 : le score est de $0 × 2 = 0$ ;

* 0 boules de valeur 3 : le score est de $0 × 3 = 0$ ;

* 3 boules de valeur 4 : le score est de $3 × 4 = 12$ ;

* 2 boules de valeur 5 : le score est de $2 × 5 = 10$ ;

* 0 boules de valeur 6 : le score est de $0 × 6 = 0$ ;

Le score maximal est donc de $12$.

## Objectif

Écrire la fonction `score_max` qui prend en paramètre la liste des résultats et renvoie son score maximal.

On garantit que le nombre de résultats obtenus pour chaque valeur est toujours un entier positif ou nul.

## Exemples

```pycon
>>> score_max([5, 0])  # 5 boules valant 1 et 0 valant 2
5
>>> score_max([2, 0, 0, 0, 2, 0])
10
>>> score_max([2000, 3000, 2000, 5000, 2000, 3000, 1000, 6000, 2000])
48000
```
