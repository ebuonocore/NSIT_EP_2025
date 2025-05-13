---
author: Nicolas Revéret
reviews: Franck Chambon, Sébastien Hoarau
title: Chameau en serpent
---

# Transformer un chameau en serpent

En informatique, la *camelCase*, littéralement *casse du chameau* en français, est une façon d'écrire les différents identifiants (variables, fonctions...) dans un programme.

Si un identifiant est composé de plusieurs _parties_ (lettres ou mots), on les écrit à la suite les unes des autres en prenant soin d'écrire la première lettre de chaque partie, sauf la toute première partie, en majuscule.

Le premier caractère de l'identifiant est donc toujours en minuscule.

Par exemple, `"casseDuChameau"`, `"serpent"`, et `"variableBis"` sont écrits en *casse du chameau*.

La *snake_case*, littéralement *casse du serpent*, est un autre formatage dans lequel tous les mots sont séparés par des tirets bas (un seul entre chaque partie). Tous les caractères sont écrits en minuscule.

Par exemple, `"casse_du_chameau"`, `"serpent"`, et `"variable_bis"` sont écrits en *casse du serpent*.

## Objectif

On demande d'écrire la fonction `en_serpent` qui prend en paramètre une chaine de caractères `identifiant` contenant un identifiant écrit en *casse du chameau* et renvoyant le même identifiant écrit en *casse du serpent*.

On rappelle que si `c` est un caractère alors :

* `c.islower()` indique, par un booléen renvoyé, si ce caractère est une minuscule,

* `c.isupper()` indique, par un booléen renvoyé, si ce caractère est une majuscule,

* `c.lower()` renvoie le même caractère dans sa version minuscule,

* `c.upper()` renvoie le même caractère dans sa version majuscule.

On garantit que les identifiants passés en arguments :

* ne sont pas vides,
* répondent exactement au format *casse du chameau*,
* **ne contiennent que des caractères alphabétiques.**

## Exemples

```pycon
>>> en_serpent("casseDuChameau")
'casse_du_chameau'
>>> en_serpent("serpent")
'serpent'
>>> en_serpent("xYZ")
'x_y_z'
>>> en_serpent("uneVariableHyperImportante")
'une_variable_hyper_importante'
```
