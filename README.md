# P10_decision
## Arbre de décision, Forêt aléatoire

### Principe du l'arbre de décision

Un arbre de décision modélise une hiérarchie de tests pour prédire un résultat. 
Il existe deux principaux types d’arbre de décision : l'arbre de régression ou l'arbre de classifiction. 
Ici, nous traitons un problème de régression, c'est donc le premier qui sera utilisé. Il permet de prédire une quantité réelle, une valeur numérique : par exemple, le prix d’une maison, comme c'est le cas ici.

Les décisions possibles sont situées aux extrémités des branches (les « feuilles » de l’arbre) et sont atteintes en fonction de décisions prises à chaque étape. 
Un arbre de décision fonctionne en appliquant de manière itérative des règles logiques très simples, chaque règle étant choisie en fonction du résultat de la règle précédente. 
Les arbres de décision ont pour avantage d’être simple à interpréter, très rapide à entrainer, d’être non paramétrique, et de nécessiter très peu de prétraitement des données.
![img](images/decision-tree.png)

### Random Forest

Un autre usage en machine learning consiste à construire non pas un arbre mais une forêt d’arbres de décision. 
Une décision est alors prise en faisant « voter » l’ensemble des arbres et en choisissant la réponse majoritaire (pour un choix discret) ou la moyenne des réponses (pour une variable continue). 

L’algorithme des « forêts aléatoires » (ou Random Forest parfois aussi traduit par forêt d’arbres décisionnels) est un algorithme de classification qui réduit la variance des prévisions d’un arbre de décision seul, améliorant ainsi leurs performances.
Cet algorithme effectue un apprentissage en parallèle sur de multiples arbres de décision construits aléatoirement et entraînés sur des sous-ensembles de données différents. 
![img](images/forest.png)
Le nombre idéal d’arbres est un paramètre important : il est très variable et dépend du problème. 
Concrètement, chaque arbre de la forêt aléatoire est entrainé sur un sous ensemble aléatoire de features  selon le principe des « projections aléatoires ». Les prédictions sont ensuite moyennées (lorsque les données sont quantitatives) ou utilisés pour un "vote" (pour des données qualitatives, dans le cas des arbres de classification). 
L’algorithme des forêts aléatoires est connu pour être un des classifieurs les plus efficaces parmis ceux qui nécessitent peu de prétraitement des données. 


### Etude du dataset "California Housing"







sources :
_Leo Breiman. Random forests. Machine Learning, 45(1):5–32, 2001_

