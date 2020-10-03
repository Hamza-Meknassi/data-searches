
#Data Link : 'https://www.data.gouv.fr/fr/datasets/consommation-annuelle-delectricite-et-gaz-par-departement-et-par-code-naf/'

#### Nom&Prenom:Meknassi 
#### Nom&Prenom:Hammad 
# Quel est le problème que vous allez traiter ?

Nous allons prédir la consomation de gaz et d'éléctricité pour chaque région de France en s'appuyant sur des données réelles depuis 2017 pour tous les départements Français.

# Quelles sont les données sur lesquelles vous allez travailler ?

Nous allons travailler sur des données:

-Année (2017-2020)

-Département

-Région

-Filières(électricité et gaz)

-Opérateurs

-Catégorie de consommation

-Consommation(MWh)

-Indice qualité

# Comment allez-vous procéder pour résoudre votre problème ?

Pour la resolution de notre probleme, on va pouvoir predire la consomation 
d'electricite et de gaz pour toutes les regions de france pour l'année 2021, cette prediction qui sera sous forme d'une fonction,qui recevera en entrée des données et essayera de trouver la meilleur valeurs des coefficients 
```(y = B0 + B1 * x)``` pour se faire on envisage procéder a la resolution de notre probléme comme suit: 
- Disposer d’un Dataset (x, y) où x sont nos features (une region geographique donées) ( et y notre  target (la consomation par (MWh)) 
- Développer un Modèle dont les paramètres sont à trouver pour aller d'un modele initiale avec des parametres aleatoires à un modele finale que la machine doit trouver en apprenant les valeurs du parametre  ```B0``` et ```B1``` de notre  model ```f(x) = ax + b. ``` en minimisant la fonction coût . 
- Déterminer une Fonction Coût optimale ? (pour le moment on pense a: ``L’Erreur Quadratique Moyenne``

# Quelles techniques et quels algorithmes allez-vous utiliser ?

- linear regression learning algorithm
    - algebre lineaire pour: 
        - least squares
        - gradient descent

# Comment allez-vous évaluer votre solution ?

Pour savoir l'éfficacite de notre solution,on va essayer de predire les resultats de l'année 2019 et comparer les resultats obtenus avec les données réelles. Ensuite voir la marge du  taux d'erreur entre les deux données,avec une representation graphique. Cela nous permettera de juger l'éfficacité de notre prediction. 
