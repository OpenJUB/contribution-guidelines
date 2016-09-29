Contributing Guidelines
=======================
A repository consisting of contrbution guidelines for OpenJUB projects.


Git Workflow
------------
- At beginning we'll start out with the pull request model. i.e. You fork the
  repository and maintain your fork while making pull requests to them main
  repository. This way you can get used to the typical workflow in the open
  source projects. Once we are reasonably confident in your skills, we can
  grant you push access to the main repository.
- To learn about the git workflow, check out the [github-usage.md](https://github.com/OpenJUB/contribution-guidelines/blob/master/github_usage.md) (Everything before `Accepting and Merging a Pull Request`)



Python
------
- Minimal Python version: Python 3.5 ([Type Annotated Python](https://www.python.org/dev/peps/pep-0484/))
- Follow Python Sytax guidelines a.k.a [PEP 8](https://www.python.org/dev/peps/pep-8)
- Use [virtual environments](https://virtualenv.pypa.io/en/stable/) to isolate work environment:
    * Install virtualenv: `pip install virtualenv`
    * Create a virtual environment in the root of your work directory `virtualenv env`
    * Activate the environment: `source env/bin/activate`
- Before committing check the code with `flake8`:
    * Install flake8: `pip install flake8`
    * Check PEP8 compliance before making a commit: `flake8 --exclude env .` or `python check_pep8.py`. (`check_pep8.py` is a       file included in all project roots that executes `flake8 --exclude env .` using a subprocess)
    * In case of PEP8 warnings, fix the warnings as per PEP8 and then commit code.



