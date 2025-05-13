---
author: Nicolas Revéret
reviews: Franck Chambon, Sébastien Hoarau
title: Qui aime cela ?
---

# Qui aime cela ?

Un créateur de site web récupère, sous la forme d'une liste Python, les noms des utilisateurs "aimant" un article.

Par exemple :

```python
utilisateurs = ["A", "B"]
```

Il souhaite conclure son article par une phrase du type : `"A et B aiment cet article."`.

Par exemple :

```pycon
>>> utilisateurs = ["A"]
>>> conclusion(utilisateurs)
'A aime cet article.'
```

```pycon
>>> utilisateurs = ["A", "B"]
>>> conclusion(utilisateurs)
'A et B aiment cet article.'
```

```pycon
>>> utilisateurs = ["A", "B", "C"]
>>> conclusion(utilisateurs)
'A, B et C aiment cet article.'
```

```pycon
>>> utilisateurs = ["A", "B", "C", "D"]
>>> conclusion(utilisateurs)
'A, B et 2 autres aiment cet article.'
```

La liste des utilisateurs peut être vide ou contenir un nombre quelconque de noms d'utilisateurs (tous au format `str`).

Si la liste ne contient aucun utilisateur, on renvoie la phrase `"Personne n'aime cet article."`,

Si la liste contient un seul utilisateur, on renvoie la phrase du type `"<utilisateur> aime cet article."`,

Si la liste contient deux utilisateurs, on renvoie la phrase du type `"<utilisateur_1> et <utilisateur_2> aiment cet article."` (dans cet ordre),

Si la liste contient trois utilisateurs, on renvoie la phrase du type `"<utilisateur_1>, <utilisateur_2> et <utilisateur_3> aiment cet article."` (dans cet ordre),

Si la liste contient quatre utilisateurs ou plus, on renvoie la phrase du type `"<utilisateur_1>, <utilisateur_2> et <N> autres aiment cet article."` (dans cet ordre) avec `N` égal au nombre d'utilisateurs non cités.

## Objectif

Écrire la fonction `conclusion` qui prend en paramètre la liste `utilisateurs` contenant les noms des utilisateurs et renvoie la phrase de conclusion.

## Exemples

```pycon
>>> conclusion([])
"Personne n'aime cet article."
>>> conclusion(["A"])
'A aime cet article.'
>>> conclusion(["A", "B"])
'A et B aiment cet article.'
>>> conclusion(["A", "B", "C"])
'A, B et C aiment cet article.'
>>> conclusion(["A", "B", "C", "D"])
'A, B et 2 autres aiment cet article.'
```
