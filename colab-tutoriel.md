# Tutoriel sur COLAB
Tiré de https://www.tutorialspoint.com/google_colab/your_first_colab_notebook.htm

# Accéder à Google
Avant de commencer à utiliser Colab, assurez vous d'avoir un compte Google afin de pouvoir utiliser Google Drive ainsi que Google Colab.

Allez sur https://colab.research.google.com et cliquez ensuite sur **Nouveau Notebook**.

## Changer le nom du Notebook
Par défaut, le Notebook s'intitule **UntitledXX.ipynb**. Vous pouvez renommer le titre en cliquant sur le titre:

![Nom](https://www.tutorialspoint.com/google_colab/images/setting_notebook_name.jpg)


## Sauvegarder sur Google Drive
Pour sauvegarder sur Google Drive, aller sur Fichier -> Enregistrer une copy sur Google Drive...

## Partager le Notebook
Il est possible de partager le Colab Notebook en cliquant sur le bouton Partager qui se situe en haut à droite.

![Share](https://www.tutorialspoint.com/google_colab/images/sharing_notebook.jpg)

## Commencer à coder
Similairement à Jupyter Notebook, vous pouvez commencer à écrire du code Python dans la fenêtre et l'exécuter en cliquant sur le bouton ci-dessous:

![Write](https://www.tutorialspoint.com/google_colab/images/executing_code.jpg)

Il est possible d'enlever le output du code en cliquant sur le `X`:

![Execute](https://www.tutorialspoint.com/google_colab/images/output_display.jpg)

## Ajouter des cellules de code
Pour ajouter plus de code dans votre Notebook, il suffit d'aller dans le `Insertion` puis `Cellule de code`. Sinon, vous pouvez déplacer votre souris en bas d'une cellule. Lorsque les choix `Code` et `Texte` apparaissent, cliquez tout simplement sur l'un des deux pour ajouter une nouvelle cellule.

![Cellule](https://www.tutorialspoint.com/google_colab/images/code_text_buttons.jpg)

## Tout exécuter
Pour exécuter toute les cellules de votre Notebook en un seul clique sans interruption, allez sur `Exécution` et ensuite `Redémarrer et tout exécuter`.

## Changer l'ordre des cellules
Il est possible de changer l'ordre des cellules à l'aide des flèches:
![Cell](cellorder.JPG "CellOrder")

## Supprimer une cellule
Pour supprimer une cellule, il suffit de cliquer sur la poubelle. Sinon faire clique-droit et `Supprimer la cellule`.

## Markdown
Les cellules de texte sont du format **markdown**, un language simple de balisage. Voici quelques exemples de syntaxe:

![Text](https://www.tutorialspoint.com/google_colab/images/markdown_examples.jpg)

## Équations mathématiques
Pour écrire des équations mathématiques, il suffit d'ajouter les signes d'argent ($) entre les équations:


```python
$\sqrt{3x-1}+(1+x)^2$
```

![Math](https://www.tutorialspoint.com/google_colab/images/mathematical_equations_text_cell.jpg)

## Traçage de courbe
Sur Colab, vous pouvez aussi créer des graphiques dans les cellules de code. Par exemple, si vous écrivez:


```python
# import numpy as np
from matplotlib import pyplot as plt

y = np.random.randn(100)
x = [x for x in range(len(y))]

plt.plot(x, y, '-')
plt.fill_between(x, y, 200, where = (y > 195), facecolor='g', alpha=0.6)

plt.title("Sample Plot")
plt.show()
```

Vous obtenez sur Colab:

![Chart](https://www.tutorialspoint.com/google_colab/images/graphical_outputs.jpg)

## Liste de fonctions
Pour connaître la liste des fonctions d'une bibliothèque, comme `numpy`, il suffit de mettre un point après le nom de la fonction comme ceci:

![Help](.\donnees\helpcolab.png "Help")

## Documentation de la fonction
Pour connaître la documentation de chaque fonction, il suffit d'écrire les parenthèses comme ceci et une fenêtre s'affichera avec la documentation:

![Docu](.\donnees\functiondoc.png "Docu")
