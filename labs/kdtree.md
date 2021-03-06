# KdTree

L’objectif de ce TD est la familiarisation avec la structure de donnée KdTree.
Pour ce faire nous allons mettre en place un algorithme que quantization
d’image.
Une base de code vous est fourni dans le dépôt [GitHub](https://github.com/czanni/KdTree)
Il est conseillé d’effectuer un fork de ce dépôt git et de travailler sur votre
propre branche tout en effectuant des commits régulièrement.

Voici la liste des taches à réaliser :

# Question 1

Actuellement le fichier de test unitaire de la structure ne contient qu’un 
test de validation via une utilisation de la structure (comparaison de requête
de plus proche voisin via le KdTree et recherche linéaire). En cas
d’échecs un tel test ne donne que très peu d’information sur la source du problème.
Quel test pourrait-on mettre en place pour valider la création du KdTree? 
Implémenter le test proposé.

# Question 2

Mettre en place l’algorithme de Quantization dans la fonction main. 
Afin de faciliter sa mise en place, vous pouvez suivre les étapes suivantes:
- ajouter la possibilité de construire un kd-tree équilibré,
- utiliser une meilleure heuristique pour le choix de la dimension de coupe,
- paramétrer la construction du kd-tree par une profondeure maximale (un nombre de points
indéterminé devrait alors se retrouver dans une feuille de l’arbre, la bonne façon de faire serait de les stocker, cependant pour les besoins de l’exercice, vous pouvez vous contenter de stocker le barycentre des points).

# Question 3

Voici quelques améliorations pouvant être apporter à la structure de donnée:
- Implémenter une recherche des k plus proches voisins.
- Utiliser l’algorithme de la médiane des médianes pour obtenir une
	construction plus efficace.

ou à l’algorithme de quantification :
- Algorithme de dithering par propagation d’erreur ([wikipedia](https://en.wikipedia.org/wiki/Floyd–Steinberg_dithering))
