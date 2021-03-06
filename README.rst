===========
python_test
===========

| |license| |black|
|
| |azure_pipeline| |azure_coverage|
| |docs| |reqs|
|
| |py_versions| |implementations|
| |pypi| |status| |format| |downloads|
|
| |release| |commits_since|  |last_commit|
| |stars| |forks| |contributors|
|


Info
----

**Repo for testing different stuff with open source python repos. This project is under GPL-3.0 License even if the LICENSE file shows another license because of tests.**

#. create repo and cd into::

    $ git clone xxx
    $ cd xxx

#. add basic files::

    $ touch .gitignore
    $ touch .gitattributes
    $ touch LICENSE.rst
    $ touch README.rst
    $ touch CHANGELOG.rst

#. create venv and activate it::

    $ python3 -m venv venv
    $ . venv/bin/activate

#. update pip, setuptools::

    $ pip install -U pip setuptools

#. open in pycharm and setup venv as interpreter

#. setup docs
    Badges for docs:
      * License
      * Version
      * Travis (https://travis-ci.com/)
      * Coverage (https://coveralls.io/)
      * Docs (RtD)
      * Black

    ::

        $ pip install sphinx
        $ mkdir docs && pushd docs
        $ sphinx-quickstart
        $ make html
        $ popd
        $ touch .readthedocs.yaml

#. setup tests::

    $ pip install pytest
    $ mkdir tests && pushd tests
    $ touch conftest.py
    $ popd
    $ touch pytest.ini

#. setup tox
    tox:
      - flake8
      - pylint
      - black
      - isort
      - coverage
      - docs
      - pytest

::

    $ touch tox.ini

#. setup travis-ci::

    $ touch .travis.yml

#. setup setup::

    $ touch setup.py
    '''add stuff to setup.py'''
    $ pip install -e .




TODO:

* badges:

    - https://github.com/nedbat/coveragepy/blob/master/README.rst
    - https://github.com/pytest-dev/pytest-cov/blob/master/README.rst
    - requires.io

* pre-commit
* appveyor a

bla bla bla

.. .############################### LINKS ###############################

.. BADGES START

.. info block
.. |license| image:: https://img.shields.io/github/license/Cielquan/python_test.svg?style=for-the-badge
    :alt: License
    :target: https://github.com/Cielquan/python_test/blob/master/LICENSE.rst

.. |black| image:: https://img.shields.io/badge/code%20style-black-000000.svg?style=for-the-badge
    :alt: Code Style: Black
    :target: https://github.com/psf/black


.. tests block
.. .image:: https://travis-ci.com/Cielquan/python_test.svg?branch=master
.. .|travis| image:: https://img.shields.io/travis/com/Cielquan/python_test/master.svg?style=for-the-badge&logo=travis-ci&logoColor=FBE072
    :alt: Travis - Build Status
    :target: https://travis-ci.com/Cielquan/python_test

.. .image:: https://ci.appveyor.com/api/projects/status/github/Cielquan/python_test?branch=master&svg=true
.. .|appveyor| image:: https://img.shields.io/appveyor/ci/Cielquan/python_test/master.svg?style=for-the-badge&logo=appveyor
    :alt: AppVeyor - Build Status
    :target: https://ci.appveyor.com/project/Cielquan/pytest-cov

.. .image:: https://codecov.io/gh/Cielquan/python_test/branch/master/graph/badge.svg
.. .|codecov| image:: https://img.shields.io/codecov/c/github/Cielquan/python_test/master.svg?style=for-the-badge&logo=codecov
    :alt: Codecov - Test Coverage
    :target: https://codecov.io/gh/Cielquan/python_test

.. |azure_pipeline| image:: https://img.shields.io/azure-devops/build/cielquan/b6aee80c-ebd7-443c-9679-70e990729db6/1?style=for-the-badge&logo=azure-pipelines&label=Azure%20Pipelines
    :target: https://dev.azure.com/cielquan/python_test/_build/latest?definitionId=1&branchName=master
    :alt: Azure DevOps builds

.. |azure_coverage| image:: https://img.shields.io/azure-devops/coverage/cielquan/python_test/1?style=for-the-badge&logo=azure-pipelines&label=Coverage
    :target: https://dev.azure.com/cielquan/python_test/_build/latest?definitionId=1&branchName=master
    :alt: Azure DevOps Coverage

.. .image:: https://readthedocs.org/projects/python-test-cielquan/badge/?version=latest
.. |docs| image:: https://img.shields.io/readthedocs/python_test_cielquan/latest.svg?style=for-the-badge&logo=read-the-docs&logoColor=white
    :alt: Read the Docs (latest) - Status
    :target: https://python-test-cielquan.readthedocs.io/en/latest/?badge=latest

.. .image:: https://requires.io/github/Cielquan/python_test/requirements.svg?branch=master
.. |reqs| image:: https://img.shields.io/requires/github/Cielquan/python_test.svg?style=for-the-badge
    :alt: Requires.io - Requirements status
    :target: https://requires.io/github/Cielquan/python_test/requirements/?branch=master


.. PyPI block
.. |py_versions| image:: https://img.shields.io/pypi/pyversions/coverage.svg?style=for-the-badge&logo=python&logoColor=FBE072
    :alt: PyPI - Python versions supported
    :target: https://pypi.org/project/python_test_cielquan/

.. |implementations| image:: https://img.shields.io/pypi/implementation/coverage.svg?style=for-the-badge&logo=python&logoColor=FBE072
    :alt: PyPI - Implementations supported
    :target: https://pypi.org/project/python_test_cielquan/

.. |status| image:: https://img.shields.io/pypi/status/coverage.svg?style=for-the-badge&logo=pypi&logoColor=FBE072
    :alt: PyPI - Package stability
    :target: https://pypi.org/project/python_test_cielquan/

.. |pypi| image:: https://img.shields.io/pypi/v/coverage.svg?style=for-the-badge&logo=pypi&logoColor=FBE072
    :alt: PyPI - Package latest release
    :target: https://pypi.org/project/python_test_cielquan/

.. |format| image:: https://img.shields.io/pypi/format/coverage.svg?style=for-the-badge&logo=pypi&logoColor=FBE072
    :alt: PyPI - Format
    :target: https://pypi.org/project/python_test_cielquan/

.. |wheel| image:: https://img.shields.io/pypi/wheel/coverage.svg?style=for-the-badge
    :alt: PyPI - Wheel
    :target: https://pypi.org/project/python_test_cielquan/

.. |downloads| image:: https://img.shields.io/pypi/dm/coverage.svg?style=for-the-badge&logo=pypi&logoColor=FBE072
    :target: https://pypi.org/project/python_test_cielquan/
    :alt: PyPI - Monthly downloads


.. Github block
.. |release| image:: https://img.shields.io/github/v/release/Cielquan/python_test.svg?style=for-the-badge&logo=github
    :alt: Github Latest Release
    :target: https://github.com/Cielquan/python_test/releases/latest

.. |commits_since| image:: https://img.shields.io/github/commits-since/Cielquan/python_test/latest.svg?style=for-the-badge&logo=github
    :alt: GitHub commits since latest release
    :target: https://github.com/Cielquan/python_test/commits/master

.. |last_commit| image:: https://img.shields.io/github/last-commit/Cielquan/python_test.svg?style=for-the-badge&logo=github
    :alt: GitHub last commit
    :target: https://github.com/Cielquan/python_test/commits/master

.. |stars| image:: https://img.shields.io/github/stars/Cielquan/python_test.svg?style=for-the-badge&logo=github
    :alt: Github stars
    :target: https://github.com/Cielquan/python_test/stargazers

.. |forks| image:: https://img.shields.io/github/forks/Cielquan/python_test.svg?style=for-the-badge&logo=github
    :alt: Github forks
    :target: https://github.com/Cielquan/python_test/network/members

.. |contributors| image:: https://img.shields.io/github/contributors/Cielquan/python_test.svg?style=for-the-badge&logo=github
    :alt: Github Contributors
    :target: https://github.com/Cielquan/python_test/graphs/contributors

..  BADGES END

####################################

commit-msg hook for jira issue verification with pre-commit.

See also: https://github.com/pre-commit/pre-commit

Add this to your ``.pre-commit-config.yaml``:

.. code-block:: yaml

    - repo: https://github.com/Cielquan/commit-msg-jira-hook
      rev: v0.1.0 # Use the ref you want to point at
      hooks:
      - id: jira_commit_msg
        stages: [commit-msg]

Then add a ``jira.ini`` to you projects root directory with following data:

.. code-block:: ini

    [jira]
    JIRA_URL = e.g. https://jira.atlassian.com
    JIRA_TAG = tag
    JIRA_USERNAME = email
    JIRA_TOKEN = api-token

Lastly install the hook:

.. code-block:: console

    $ pre-commit install -t commit-msg
