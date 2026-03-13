# TP4 - Introduction à JavaScript

**Module :** Technologies Web et Web Sémantique
**Master :** SDIA
**Date :** Mars 2026

---

## Objectifs

Ce travail pratique constitue une introduction à la programmation en JavaScript côté client. Les exercices couvrent les notions fondamentales du langage : fonctions, structures conditionnelles, boucles imbriquées, manipulation de chaînes de caractères et arithmétique entière.

Chaque exercice est implémenté sous forme d'une page HTML autonome embarquant le code JavaScript directement dans une balise `<script>`. Les entrées utilisateur sont collectées via `prompt()` et les résultats affichés dans la console du navigateur.

---

## Structure du projet

```
TP4/
├── tempConversion.html          # Exercice 1   : Conversion Fahrenheit -> Celsius
├── durationConversion.html      # Exercice 2   : Conversion de durées en secondes
├── troisNombres.html            # Exercice 3   : Classement de 3 nombres
├── motifTriangleEscalier.html   # Exercice 4   : Motif en escalier
├── motifPyramid.html            # Exercice 4-bis : Motif en pyramide
└── testNombrePremier.html       # Exercice 5   : Test de primalité
```

---

## Description des exercices

### Exercice 1 - Conversion de température (`tempConversion.html`)

Conversion d'une température de Fahrenheit vers Celsius à l'aide de la formule :

```
C = (5 / 9) * (F - 32)
```

L'utilisateur saisit une valeur en Fahrenheit et le résultat est affiché avec deux décimales.

---

### Exercice 2 - Conversion de durées (`durationConversion.html`)

Conversion d'un nombre de secondes en une durée exprimée en jours, heures, minutes et secondes. La fonction `hjms(sec)` utilise la division entière et le modulo pour décomposer la durée. La gestion du singulier et du pluriel (« jour » / « jours », « heure » / « heures », etc.) est assurée pour produire un affichage grammaticalement correct en français.

**Exemple :** 90061 secondes -> 1 jour, 1 heure, 1 minute et 1 seconde

---

### Exercice 3 - Classement de 3 nombres (`troisNombres.html`)

L'utilisateur saisit trois nombres. La fonction `troisNombres()` les trie dans l'ordre croissant en implémentant un tri par sélection manuel : elle extrait itérativement le minimum du tableau non trié et le déplace dans le tableau résultat.

---

### Exercice 4 - Motif en escalier (`motifTriangleEscalier.html`)

Affichage d'un triangle rectangle composé d'astérisques. La taille `n` est saisie par l'utilisateur. La ligne `i` contient `i` astérisques. Deux implémentations sont fournies et comparées :

- `triangle1` : boucles `while` imbriquées
- `triangle2` : boucles `for` imbriquées

```
*
**
***
****
```

---

### Exercice 4-bis - Motif en pyramide (`motifPyramid.html`)

Affichage d'une pyramide symétrique centrée. La ligne `i` contient `(n - i)` espaces suivis de `(2i - 1)` astérisques. Deux implémentations sont également fournies (`while` et `for`).

```
   *
  ***
 *****
*******
```

---

### Exercice 5 - Test de primalité (`testNombrePremier.html`)

La fonction `estPremier(nbr)` détermine si un entier positif est un nombre premier. L'algorithme applique les optimisations suivantes :

- Les nombres inférieurs ou égaux à 1 sont immédiatement exclus.
- Le cas `2` est traité explicitement.
- Les nombres pairs sont rejetés sans itération.
- Pour les nombres impairs restants, seuls les diviseurs impairs de `3` jusqu'à `(n+1)/2` sont testés, avec un pas de 2.

Si le nombre n'est pas premier, le premier diviseur trouvé est affiché.

---

## Utilisation

1. Ouvrir le fichier HTML souhaité dans un navigateur web.
2. Renseigner la valeur demandée dans la boîte de dialogue `prompt`.
3. Ouvrir la console du navigateur (`F12` > onglet Console) pour consulter le résultat.
