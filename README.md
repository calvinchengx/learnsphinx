Learn Sphinx
===========

1.  mkvirtualenv --distribute --no-site-packages learnsphinx

2.  cd $PROJECT\_HOME

3.  git clone git@github.com:calvinchengx/learnsphinx.git

4.  cd learnsphinx

5.  pip install sphinx

6.  sphinx-quickstart  # Create docs as root of our documentation

7.  vim docs/source/conf.py and add in

		sys.path.insert(0, os.path.abspath('../..'))
		sys.path.insert(0, os.path.abspath('../../example_project'))

8.  sphinx-apidoc -o docs/source example\_project

9.  cd docs

10. make html

11. open build/html/index.html 

Use sphinx_bootstrap_theme
===============

1.  pip install sphinx\_bootstrap\_theme
2.  vim docs/source/conf.py and add/edit

        import sphinx_bootstrap_theme
		html_theme = 'bootstrap'
		html_theme_path = sphinx_bootstrap_theme.get_html_theme_path()

    More customization details [here](https://github.com/ryan-roemer/sphinx-bootstrap-theme)

Generated Documentation
===============

The generated documentation can be found at [readthedocs.org](https://learn-sphinx.readthedocs.org/en/latest/)
