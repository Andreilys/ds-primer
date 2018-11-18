# Data Science Primer

[View The Cheatsheet](https://ds-primer.readthedocs.io/en/latest/)

## How To Contribute

1. Clone Repo
```
git clone https://github.com/andreilys/ds-primer.git
```

2. Install Dependencies
```
# Assumes you have the usual suspects installed: numpy, scipy, etc..
pip install sphinx sphinx-autobuild
pip install sphinx_rtd_theme
pip install recommonmark
```
For python-3.x installed, use:
```
pip3 install sphinx sphinx-autobuild
pip3 install sphinx_rtd_theme
pip3 install recommonmark
```
3. Preview Changes
```
cd ml-cheatsheet
cd docs
make html
```

4. Verify your changes by opening the `index.html` file in `_build/`

5. [Submit Pull Request](https://help.github.com/articles/creating-a-pull-request/)


### Short for time?

Feel free to raise an [issue](https://github.com/bfortuner/ml-cheatsheet/issues) to correct errors or contribute content without a pull request.


## Style Guide

Each entry in the glossary MUST include the following at a minimum:

1. **Concise explanation** - as short as possible, but no shorter
2. **Citations** - Papers, Tutorials, etc.

Excellent entries will also include:

1. **Visuals** - diagrams, charts, animations, images
2. **Code** - python/numpy snippets, classes, or functions
3. **Equations** - Formatted with Latex

The goal of the cheatsheet is to present content in the most accessible way possible, with a heavy emphasis on visuals and interactive diagrams. That said, in the spirit of rapid prototyping, it's okay to to submit a "rough draft" without visuals or code. We expect other readers will enhance your submission over time.


## Why RST and not Markdown?

RST has more features. For large and complex documentation projects, it's the logical choice.

* https://eli.thegreenplace.net/2017/restructuredtext-vs-markdown-for-technical-documentation/


## Tips and Tricks

* [Adding equations](http://www.sphinx-doc.org/en/stable/ext/math.html)
* [Working with Jupyter Notebook](http://louistiao.me/posts/demos/ipython-notebook-demo/)
* Quickstart with Jupyter notebook template
* Graphs and charts
* Importing images
* Linking to code


## Resources

* [Desmos Graphing Tool](https://www.desmos.com/calculator)
* [3D Graphing Tool](https://www.geogebra.org/3d)
* [How To Submit Pull Requests](https://help.github.com/articles/creating-a-pull-request/)
* [RST Cheatsheet](http://docutils.sourceforge.net/docs/user/rst/quickref.html)
* [Markdown Cheatsheet](https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet)
* [Citation Generator](http://www.citationmachine.net)
* [MathJax Cheatsheet](https://math.meta.stackexchange.com/questions/5020/mathjax-basic-tutorial-and-quick-reference)
* [Embedding Math Equations](http://www.sphinx-doc.org/en/stable/ext/math.html)
* [Sphinx Tutorial](https://pythonhosted.org/an_example_pypi_project/sphinx.html)
* [Sphinx Docs](http://www.sphinx-doc.org/en/stable/markup/code.html)
* [Sphinx Cheatsheet](http://openalea.gforge.inria.fr/doc/openalea/doc/_build/html/source/sphinx/rest_syntax.html)

## Attribution

This primer is inspired by the [ml-cheatsheet](https://github.com/bfortuner/ml-cheatsheet) created by Brendan Fortuner. While his cheatsheet focuses more on the technical machine learning side of things, this primer emphasizes a holistic overview of Data Science. I found his approach to structuring the cheatsheet to be clean and intuitive, so I decided to replicate it here with the Data Science primer.