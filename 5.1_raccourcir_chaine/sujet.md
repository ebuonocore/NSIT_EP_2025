---
author: Nicolas Revéret
reviews: Franck Chambon, Sébastien Hoarau
title: Raccourcir une chaîne
---

# Raccourcir une chaine

En programmation web, il arrive que l'on doive abréger des chaines de caractères avant de les afficher.

Par exemple, le texte `"Hello World"` :

* abrégé sur 3 caractères devient `"..."`

* abrégé sur 5 caractères devient `"He..."`

* abrégé sur 8 caractères devient `"Hello..."`

* abrégé sur 9 caractères devient `"Hello ..."`

* abrégé sur 11 caractères devient `"Hello World"`

* abrégé sur 20 caractères devient `"Hello World"`


## Objectif

Écrire la fonction `abrege` qui prend en paramètres :

* la chaine de caractères `chaine`,

* l'entier positif `n` (`n` est supérieur ou égal à 3),

et qui renvoie la version abrégée de `chaine`.

## Exemples

```pycon
>>> abrege("Hello World", 3)
'...'
>>> abrege("Hello World", 5)
'He...'
>>> abrege("Hello World", 8)
'Hello...'
>>> abrege("Hello World", 9)
'Hello ...'
>>> abrege("Hello World", 11)
'Hello World'
>>> abrege("Hello World", 20)
'Hello World'
```
