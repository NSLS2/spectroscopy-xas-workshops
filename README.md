# spectroscopy-xas-workshops
Materials related to XAS Workshops at NSLS-II


## Dependencies

To compile this manual, you will need to install the following using
pip or some other method:

1. [sphinx-math-dollar](https://github.com/sympy/sphinx-math-dollar/)
2. [sphinx-subfigure](https://github.com/sphinx-extensions2/sphinx-subfigure)
3. [spinx-book-theme](https://github.com/executablebooks/sphinx-book-theme)

## Hints

To compile the manual on a machine with an externally managed python
environment, you may need to use a python virtual environment.  

First cd to the docs/ folder and do

    python3 -m venv ./my-venv
        
Then install the dependencies locally by doing:

    ./my-venv/bin/pip install sphinx_math_dollar
    ./my-venv/bin/pip install sphinx_subfigure
    ./my-venv/bin/pip install sphinx_book_theme

After installing the dependencies into the virtual environment, try
something like this:

     make SPHINXBUILD=./my-venv/bin/sphinx-build html

