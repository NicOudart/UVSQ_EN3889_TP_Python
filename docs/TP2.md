# TP 2 : Héritage et polymorphisme

![En-tête TP2](img/Header_TP2.png)

_Lors de ce TP, nous allons programmer un automate cellulaire 2D de type "turmite", en complétant petit à petit une classe mère commune à tous les automates cellulaires 2D, puis une classe fille spécifique aux "turmites"._
_En fin de TP, nous réfléchirons à comment nous pourrions améliorer notre programme en s'appuyant sur les méthodes spéciales Python._

---

## Les Turmites

## Définition de la classe mère

~~~
class 2D_cellular_automaton:
    
    def __init__(self,grid_size_x,grid_size_y):
        
		#Complétez ici
        
    def set_grid(self,grid):
        
		#Complétez ici
    
    def get_grid(self):
        
		#Complétez ici
        
    def set_rules(self,rules_code):
        
		#Complétez ici
        
    def get_rules(self):
        
		#Complétez ici
        
    def get_iteration(self):
        
		#Complétez ici
        
    def iterate_grid(self):
		
		#Complétez ici
        
    def display_grid(self):
        plt.figure()
        plt.imshow(self.grid,cmap='binary')
        plt.show()
        
    def save_grid(self):
        plt.figure()
        plt.imshow(self.grid,cmap='binary')
        plt.savefig('automaton_'+str(self.iteration)+'.png')
        plt.close()
~~~

### Constructeur

### Getters

### Setters

## Définition de la classe fille

~~~
class turmite(2D_cellular_automaton):
    
    def __init__(self,grid_size_x,grid_size_y,rules_code,state,pos_x,pos_y,orientation):
        
		#Complétez ici
        
    def set_rules(self,rules_code):
        
		#Complétez ici
        
    def get_rules(self):
        
		#Complétez ici
        
    def set_state(self,state):
        
		#Complétez ici
        
    def get_state(self):
        
		#Complétez ici
    
    def set_position(self,pos_x,pos_y):
        
		#Complétez ici
        
    def get_position(self):
        
		#Complétez ici
    
    def set_value(self,value):
        
		#Complétez ici
        
    def get_value(self):
        
		#Complétez ici
    
    def set_orientation(self,orientation):
        
		#Complétez ici
        
    def get_orientation(self):
        
		#Complétez ici
    
    def turn(self,direction):
        
		#Complétez ici
        
    def move(self):
        
        #Complétez ici
    
    def iterate_grid(self,nb_iterations):
        
        #Complétez ici
~~~

### Constructeur

### Getters

### Setters

## Instanciation et simulation

![Simulation TP2](img/TP2_example.gif)

## Vers les méthodes spéciales

---

