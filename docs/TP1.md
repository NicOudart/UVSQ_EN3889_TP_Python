# TP 1 : De la programmation procédurale vers l'Orienté Objet

![En-tête TP1](img/Header_TP1.png)

---

## Les automates cellulaires élémentaires

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
    

init_sequence = '00000000000000000000000000000000000000000000000000000000111011010010001100000100111010110001011000001110111001100100100011001011001'

#Complétez ici
~~~

![Simulation TP1](img/TP1_example.png)