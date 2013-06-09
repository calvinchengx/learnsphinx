learnsphinx
===========

1.  mkvirtualenv --distribute --no-site-packages learnsphinx
2.  cd $PROJECT\_HOME
3.  git clone git@github.com:calvinchengx/learnsphinx.git
4.  cd learnsphinx
5.  pip install sphinx
6.  sphinx-quickstart  # Create docs as root of our documentation
7.  vim docs/source/conf.py and add in
	```
    sys.path.insert(0, os.path.abspath('../..'))
	sys.path.insert(0, os.path.abspath('../../example_project'))
	```
8.  sphinx-apidoc -o docs/source example\_project
9.  cd docs
10. make html
11. open build/html/index.html 
