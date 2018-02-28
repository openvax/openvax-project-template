# Releasing Pyensembl

This document explains what do once your [Pull Request](https://www.atlassian.com/git/tutorials/making-a-pull-request/) has been reviewed and all final changes applied. Now you're ready merge your branch into master and release it to the world:

0. Make sure that you have `pandoc` and `pypandoc` installed: this is needed for readme markdown on PyPI. (See [here](http://pandoc.org/installing.html) and [here](https://pypi.python.org/pypi/pypandoc), respectively, for instructions.)
1. Bump the [version](http://semver.org/) in `__init__.py`, as part of the PR you want to release.
2. Merge your branch into master.
3. Travis has been configured to auto-deploy to PyPI, as long as the tests succeed and the library version is newer than any released. 
