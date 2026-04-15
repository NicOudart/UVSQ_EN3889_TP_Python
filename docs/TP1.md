# TP 1 : De la programmation procédurale vers l'Orienté Objet

![En-tête TP1](img/Header_TP1.png)

_Lors de ce TP, nous allons réviser la programmation procédurale en Python._
_Vous devrez programmer un automate cellulaire élémentaire, en complétant petit à petit les fonctions d'un programme._
_En fin de TP, nous réfléchirons à la manière dont ce programme pourrait être transformé en Orienté Objet._

---

## Les automates cellulaires élémentaires

On appelle **automate cellulaire élémentaire** un algorithme itératif qui va initialiser une matrice 1D infinie, dont les éléments ne peuvent prendre que les valeurs 0 ou 1 :

![Automate cellulaire élémentaire](img/TP1_cellular_automaton.png)

A chaque itération, chaque élément de la matrice change ou non de valeur, suivant une série de règles sur :

* La valeur de l'élément à sa gauche.

* La valeur de l'élément à sa droite.

* La valeur de l'élément lui-même.

Pour chaque élément, il n'y a donc que **8 configurations possibles** :

![Les 8 configurations](img/TP1_configurations.png)

Il suffit donc de définir la valeur que prendra l'élément dans ces 8 situations pour obtenir les **règles** d'un automate cellulaire élémentaire.

On en déduit qu'il n'existe que **256 jeux de règles possibles**, soit autant d'automates cellulaires élémentaires différents.

En 1983, le mathématicien anglais Stephen Wolfram a proposé une manière d'identifier ces 256 automates, avec un numéro.

Si nous définissons la valeur que prend un élément d'un automate dans les 8 configurations possibles, dans cet ordre :

![Code de Wolfram](img/TP1_Wolfram_code.png)

On obtient la série de nombres binaires 01101110, qui correspond en décimal à 110.

Ce numéro, que l'on nomme **code de Wolfram**, sera l'identifiant de cet automate. 
On parlera aussi de "règle n°110".

Voici l'évolution de l'automate cellulaire n°110 pour une itération :

![Exemple pour la règle 110](img/.png)

Il est bien entendu impossible de simuler l'évoluation d'une matrice 1D infinie avec un ordinateur.
On définira donc une matrice 1D de dimensions finies, et on pourra choisir de gèrer les cas sur les bords de différentes façons :

* Ne jamais faire varier les cases sur les bords.

* Faire comme si une case imaginaire à gauche du bord gauche était à 0 et une case imaginaire à droite du bord droit était à 0.

* Faire comme si la case à gauche du bord gauche était la case du bord droit, et la case à droite du bord droit était la case du bord gauche.

_Vérifions si vous avez tout compris : quelles sont les règles de l'automate n°90 ?_
_Si nous initialisons l'automate avec une matrice 1D 010110100, quelle serait l'état de l'automate à l'itération suivante (en ne faisant pas varier les bords) ?_

## Déterminer les règles de l'automate

~~~
def nb_to_bin(rule_number):

	#Complétez ici
    
    return wolfram_code
~~~

~~~
def bin_to_rule(wolfram_code):

	#Complétez ici
    
    return rule_dict
~~~

## Initialiser l'automate

~~~
def init_automaton(init_sequence):
    
    #Complétez ici
    
    return auto_vect
~~~

## Mettre à jour l'automate

~~~
def update_automaton(auto_vect,rule_dict):
    
    #Complétez ici
    
    return auto_vect
~~~

## Itération de l'automate

~~~
def iterate_automaton(init_sequence,rule_number,nb_iterations):
    
    #Complétez ici
        
    return auto_mat
~~~

## Affichage de la simulation

~~~
def display_automaton(auto_mat):
    
    plt.imshow(auto_mat,cmap='binary')
    
rule = 110

init_sequence = '00000000000000000000000000000000000000000000000000000000111011010010001100000100111010110001011000001110111001100100100011001011001'

#Complétez ici
~~~

![Simulation TP1](img/TP1_example.png)

## Vers l'Orienté Objet

