# TP examen : sujet de 2025

![En-tête TP exam](img/Header_TP_exam.png)

_Lors de cet examen, nous allons programmer un automate cellulaire 2D de type "Brian's brain" en paradigme orienté objet._

---

## Brian's brain

Cet examen portera à nouveau sur un type particulier d'automate cellulaire 2D : **Brian's brain**.

Imaginé en 1987 par l'informaticien Canadien Brian Silverman, cet automate cellulaire est connu pour son comportement émergent complexe et foisonnant.
De nombreuses structures appelées "vaisseaux" se déplacent rapidement sur la grille et s'entrechoquent, pour former d'autres "vaisseaux".

Chaque case de la grille d'un automate "Brian's brain" peut prendre **3 états** :

* Si la case est à 0, elle est considérée comme "**morte**".

* Si la case est à 1, elle est considérée comme "**mourrante**".

* Si la case est à 2, elle est considérée comme "**vivante**".

**Toutes les cases** de l'automate peuvent changer de valeur à chaque itération, en suivant le jeu de règles suivantes, basées sur la valeur de la case et son **voisinage de Moore** :

* Si une case a la valeur 2, elle prendra la valeur 1 à l'itération suivante.

* Si une case a la valeur 1, elle prendra la valeur 0 à l'itération suivante.

* Si une case a la valeur 0, et qu'elle a 2 voisins à la valeur 2, elle prendra la valeur 2 à l'itération suivante.
Sinon, elle restera à la valeur 0.



**N'oubliez pas d'importer Numpy et Matplotlib au début de votre programme !**

## Définition de la classe mère

## Définition de la classe fille

## Instanciation et simulation

![Simulation TP examen](img/TP_exam_example.gif)

## Pour aller plus loin