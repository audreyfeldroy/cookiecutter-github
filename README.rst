===================
cookiecutter-github
===================

An experimental Cookiecutter that:

1. Generates a bare-bones GitHub project.
2. Sticks the project into a GitHub repo.

This functionality will be extracted into a Cookiecutter plugin soon.

Requires Cookiecutter 0.7.0, which isn't out yet.

Installation
------------

```
mkvirtualenv -p /usr/local/bin/python3.3 cc-github-repo
```

Install git://github.com/audreyr/cookiecutter.git into the virtualenv. 

(I had to download and do a `python setup.py install` because pip-3.3 doesn't believe that `sys.version > 3` inside the `setup.py` - either broken on my system or a pip bug.)

Then:

```
pip install requests
cookiecutter https://github.com/audreyr/cookiecutter-github-repo.git
```
