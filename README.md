# jupyter_impala

## Prerequisite

### ipython-sql
https://github.com/LucaCanali/ipython-sql

Admin > Engines > Environmental variables
- Name: `PYTHONPATH`
- PYTHONPATH=$PYTHONPATH:/home/cdsw/lib/python/

```
git clone https://github.com/LucaCanali/ipython-sql
mkdir lib
mkdir lib/python
cd ipython-sql/
python3 setup.py install --home=~
```

```
cdsw@vmwxu2ewl08k2a65:~/ipython-sql$ python3 setup.py install --home=~
running install
running bdist_egg
running egg_info
writing src/ipython_sql.egg-info/PKG-INFO
writing dependency_links to src/ipython_sql.egg-info/dependency_links.txt
writing requirements to src/ipython_sql.egg-info/requires.txt
writing top-level names to src/ipython_sql.egg-info/top_level.txt
reading manifest file 'src/ipython_sql.egg-info/SOURCES.txt'
reading manifest template 'MANIFEST.in'
writing manifest file 'src/ipython_sql.egg-info/SOURCES.txt'
installing library code to build/bdist.linux-x86_64/egg
running install_lib
running build_py
creating build/bdist.linux-x86_64/egg
creating build/bdist.linux-x86_64/egg/sql
copying build/lib/sql/magic.py -> build/bdist.linux-x86_64/egg/sql
copying build/lib/sql/column_guesser.py -> build/bdist.linux-x86_64/egg/sql
copying build/lib/sql/__init__.py -> build/bdist.linux-x86_64/egg/sql
copying build/lib/sql/connection.py -> build/bdist.linux-x86_64/egg/sql
copying build/lib/sql/parse.py -> build/bdist.linux-x86_64/egg/sql
copying build/lib/sql/run.py -> build/bdist.linux-x86_64/egg/sql
byte-compiling build/bdist.linux-x86_64/egg/sql/magic.py to magic.cpython-36.pyc
byte-compiling build/bdist.linux-x86_64/egg/sql/column_guesser.py to column_guesser
.cpython-36.pyc
byte-compiling build/bdist.linux-x86_64/egg/sql/__init__.py to __init__.cpython-36.
pyc
byte-compiling build/bdist.linux-x86_64/egg/sql/connection.py to connection.cpython
-36.pyc
byte-compiling build/bdist.linux-x86_64/egg/sql/parse.py to parse.cpython-36.pyc
byte-compiling build/bdist.linux-x86_64/egg/sql/run.py to run.cpython-36.pyc
creating build/bdist.linux-x86_64/egg/EGG-INFO
copying src/ipython_sql.egg-info/PKG-INFO -> build/bdist.linux-x86_64/egg/EGG-INFO
copying src/ipython_sql.egg-info/SOURCES.txt -> build/bdist.linux-x86_64/egg/EGG-IN
FO
copying src/ipython_sql.egg-info/dependency_links.txt -> build/bdist.linux-x86_64/e
gg/EGG-INFO
copying src/ipython_sql.egg-info/not-zip-safe -> build/bdist.linux-x86_64/egg/EGG-INFO
copying src/ipython_sql.egg-info/requires.txt -> build/bdist.linux-x86_64/egg/EGG-INFO
copying src/ipython_sql.egg-info/top_level.txt -> build/bdist.linux-x86_64/egg/EGG-INFO
creating 'dist/ipython_sql-0.3.7.1-py3.6.egg' and adding 'build/bdist.linux-x86_64/egg' to it
removing 'build/bdist.linux-x86_64/egg' (and everything under it)
Processing ipython_sql-0.3.7.1-py3.6.egg
creating /home/cdsw/lib/python/ipython_sql-0.3.7.1-py3.6.egg
Extracting ipython_sql-0.3.7.1-py3.6.egg to /home/cdsw/lib/python
Removing ipython-sql 0.3.7.1 from easy-install.pth file
Adding ipython-sql 0.3.7.1 to easy-install.pth file

Installed /home/cdsw/lib/python/ipython_sql-0.3.7.1-py3.6.egg
Processing dependencies for ipython-sql==0.3.7.1
Searching for six==1.13.0
Best match: six 1.13.0
Adding six 1.13.0 to easy-install.pth file

Using /usr/local/lib/python3.6/site-packages
Searching for sqlparse==0.3.0
Best match: sqlparse 0.3.0
Removing sqlparse 0.3.0 from easy-install.pth file
Adding sqlparse 0.3.0 to easy-install.pth file
Installing sqlformat script to /home/cdsw/bin

Using /home/cdsw/.local/lib/python3.6/site-packages
Searching for SQLAlchemy==1.3.13
Best match: SQLAlchemy 1.3.13
Removing SQLAlchemy 1.3.13 from easy-install.pth file
Adding SQLAlchemy 1.3.13 to easy-install.pth file

Using /home/cdsw/.local/lib/python3.6/site-packages
Searching for ipython==5.1.0
Best match: ipython 5.1.0
Adding ipython 5.1.0 to easy-install.pth file
Installing iptest script to /home/cdsw/bin
Installing iptest3 script to /home/cdsw/bin
Installing ipython script to /home/cdsw/bin
Installing ipython3 script to /home/cdsw/bin

Using /usr/local/lib/python3.6/site-packages
Searching for prettytable==0.7.2
Best match: prettytable 0.7.2
Removing prettytable 0.7.2 from easy-install.pth file
Adding prettytable 0.7.2 to easy-install.pth file

Using /home/cdsw/.local/lib/python3.6/site-packages
Searching for Pygments==2.5.2
Best match: Pygments 2.5.2
Adding Pygments 2.5.2 to easy-install.pth file
Installing pygmentize script to /home/cdsw/bin

Using /usr/local/lib/python3.6/site-packages
Searching for pickleshare==0.7.5
Best match: pickleshare 0.7.5
Adding pickleshare 0.7.5 to easy-install.pth file

Using /usr/local/lib/python3.6/site-packages
Searching for pexpect==4.7.0
Best match: pexpect 4.7.0
Adding pexpect 4.7.0 to easy-install.pth file

Using /usr/local/lib/python3.6/site-packages
Searching for prompt-toolkit==1.0.18
Best match: prompt-toolkit 1.0.18
Adding prompt-toolkit 1.0.18 to easy-install.pth file

Using /usr/local/lib/python2.7/site-packages
Searching for traitlets==4.3.3
Best match: traitlets 4.3.3
Adding traitlets 4.3.3 to easy-install.pth file

Using /usr/local/lib/python3.6/site-packages
Searching for setuptools==41.2.0
Best match: setuptools 41.2.0
setuptools 41.2.0 is already the active version in easy-install.pth
Installing easy_install script to /home/cdsw/bin
Installing easy_install-3.6 script to /home/cdsw/bin

Using /usr/local/lib/python2.7/site-packages
Searching for simplegeneric==0.8.1
Best match: simplegeneric 0.8.1
Adding simplegeneric 0.8.1 to easy-install.pth file

Using /usr/local/lib/python3.6/site-packages
Searching for decorator==4.4.1
Best match: decorator 4.4.1
Adding decorator 4.4.1 to easy-install.pth file

Using /usr/local/lib/python3.6/site-packages
Searching for ptyprocess==0.6.0
Best match: ptyprocess 0.6.0
Adding ptyprocess 0.6.0 to easy-install.pth file

Using /usr/local/lib/python3.6/site-packages
Searching for wcwidth==0.1.7
Best match: wcwidth 0.1.7
Adding wcwidth 0.1.7 to easy-install.pth file

Using /usr/local/lib/python3.6/site-packages
Searching for ipython-genutils==0.2.0
Best match: ipython-genutils 0.2.0
Adding ipython-genutils 0.2.0 to easy-install.pth file

Using /usr/local/lib/python3.6/site-packages
Finished processing dependencies for ipython-sql==0.3.7.1
```
