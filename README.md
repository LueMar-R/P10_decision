# P10_decision
## Arbre de décision, Forêt aléatoire

### Principe du l'arbre de décision

Un arbre de décision modélise une hiérarchie de tests pour prédire un résultat. 
Il existe deux principaux types d’arbre de décision : l'arbre de régression ou l'arbre de classifiction. 
Ici, nous traitons un problème de régression, c'est donc le premier qui sera utilisé. Il permet de prédire une quantité réelle, une valeur numérique : par exemple, le prix d’une maison, comme c'est le cas ici.

Les décisions possibles sont situées aux extrémités des branches (les « feuilles » de l’arbre) et sont atteintes en fonction de décisions prises à chaque étape. 
Un arbre de décision fonctionne en appliquant de manière itérative des règles logiques très simples, chaque règle étant choisie en fonction du résultat de la règle précédente. 
Les arbres de décision ont pour avantage d’être simple à interpréter, très rapide à entrainer, d’être non paramétrique, et de nécessiter très peu de prétraitement des données.

### Random Forest

Un autre usage en machine learning consiste à construire non pas un arbre mais une forêt d’arbres de décision. 
Une décision est alors prise en faisant « voter » l’ensemble des arbres et en choisissant la réponse majoritaire (pour un choix discret) ou la moyenne des réponses (pour une variable continue). 
Les résultats ainsi obtenus sont remarquables notamment lorsque les arbres de décision sont utilisés en forêts aléatoires (Random Forest).







Leo Breiman. Random forests. Machine Learning, 45(1):5–32, 2001.
