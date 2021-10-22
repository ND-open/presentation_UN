# Présentation Alumni Master IS à l'Université de Nantes

Quelques ressources pour trouver un stage, un emploi en Data Sciences et se former en continu par la suite. La présentation récente est accessible [en mode web](https://nd-open.github.io/presentation_UN/), le code est situé en `index.ipynb`.

## Ressources pour construire une présentation (dynamique) avec Jupyter Notebook

Dans Jupyter afficher les options de présentation dans `View` > `Cell Toolbar` > `Slideshow`. Sélection le type de slide et les écrire en markdown (1 slide = 1 bloc).

Pour transformer le notebook en contenu web (html) et l'afficher dans le navigateur web, adapter la commande (à exécuter dans un terminal):

```
cd chemin/vers/le/projet # cd signifie 'change directory'
jupyter nbconvert slideshow.ipynb --to slides --post serve
```

Pour exposer les slides sur Github pages, renommer le notebook `index.ipynb` et ajouter le sous-module `reveal.js` :

```
git submodule add https://github.com/hakimel/reveal.js.git reveal.js
```

Créer une branche `gh-pages` pour exposer avec Github pages de manière automatique.

## Références

* [creating-presentations-with-jupyter-notebook](https://www.blog.pythonlibrary.org/2018/09/25/creating-presentations-with-jupyter-notebook/)
* [present-your-data-science-projects-with-jupyter-slides](https://medium.com/learning-machine-learning/present-your-data-science-projects-with-jupyter-slides-75f20735eb0f)
* [how-to-create-data-driven-presentations-with-jupyter-notebooks-reveal-js](https://towardsdatascience.com/how-to-create-data-driven-presentations-with-jupyter-notebooks-reveal-js-e7a42a1fb7d7)
