---
author: Nicolas Revéret
reviews: Franck Chambon, Sébastien Hoarau
title: Résidu d'un entier
---

# Résidu d'un entier

Soit $n$ un entier positif ou nul écrit en base 10.

Le *résidu* de $n$ est l'entier obtenu en additionnant tous les chiffres de $n$ et en recommençant jusqu'à ce que le résultat soit compris entre 0 et 9 (inclus l'un et l'autre).

Par exemple, le résidu de $39$ est $3$, car $3 + 9 = 12$ et ensuite $1 + 2 = 3$.

## Objectif

On demande d'écrire les fonctions `somme_chiffres` et `residu` :

* La fonction `somme_chiffres` prend en paramètre un entier positif ou nul `n` et renvoie la somme de ses chiffres. Cette fonction pourra être récursive.

    ```pycon
    >>> somme_chiffres(12)
    3
    >>> somme_chiffres(205)
    7
    >>> somme_chiffres(78)
    15
    ```

* La fonction `residu` calcule le résidu de l'entier `n` (positif ou nul) passé en paramètre.

    ```pycon
    >>> residu(12)
    3
    >>> residu(205)
    7
    >>> residu(78)
    6
    ```

On rappelle que `n // 10` renvoie le quotient entier de `n` par `10` et que `n % 10` son reste :

```pycon
>>> 58 // 10
5
>>> 58 % 10
8
```
