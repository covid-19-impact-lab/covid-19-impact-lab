=================
Coding Guidelines
=================

One could think that due to the very ambitious deadlines we face, coding standards should be relaxed. However this is dangerous. We are working with larger teams than ever and cannot even meet face to face to coordinate our efforts. Even more importantly, we want to produce outputs that affect real policies. This makes it even more important to prevent bugs and ensure reproducibility.

Below we summarize a small set of guidelines that have proven useful in many
`OpenSourceEconomics <https://github.com/OpenSourceEconomics>`_ projects.


Collaboration and Version Control
=================================

Essential
---------

- Use git for version control and host your project on GitHub. This is the most important of all guidelines on this page.
- Write a good README for your repository. The README should tell a new contributor:
    - What programs have to be installed to run your code
    - How to run your code
    - Where to find additional documentation
    - Whom to contact in case of questions

Optional
--------

- Use a Pull Request Workflow: Do not work directly on the master branch but create a new branch for each feature you want to add to your code. Then push this branch, go to the GitHub webpage of your repository and create a pull request. Once you are done, do a squash-merge. This will summarize all commits you made to implement the feature into one.
- Do code reviews: Instead of merging your pull request directly, ask someone who is  familiar with the project for a review and only merge after he or she approves.


Reproducible Research
=====================

Essential
---------

- All outputs can be produced with one command. This can be a master do-file, a Python script or a build system command like waf or make.
- Strict separation of inputs and outputs. Inputs are the original datasets and your code. They are under version control. Everything else can be deleted and re-created with one command
- Use LaTeX instead of Word for your papers and presentations and create your regression tables automatically (i.e. without a manual copy paste step).


Optional
--------

- Use the `econ-project-templates <https://econ-project-templates.readthedocs.io/en/stable/>`_ instead of a simple master do-file or script. This will run your tasks in parallel and always only run the steps that actually have to be run.


Python Coding Guidelines
========================

Essential
---------

- Split your code into meaningful functions and write a docstring for each and every function
- Watch `this video <https://www.youtube.com/watch?v=ARKbfWk4Xyw>`_ by Raymond Hettinger (a Python core developer) about finding and preventing bugs on a time budget.


Optional
--------

- Use `pytest <https://docs.pytest.org/en/latest/>`_ and `doctests <https://docs.python.org/3/library/doctest.html>`_ to test your functions. Check the above video by Raymond Hettinger to get started.
- Adhere to this `styleguide <https://estimagic.readthedocs.io/en/latest/contributing/styleguide.html>`_ (It was written for estimagic but is basically used in all OpenSourceEconomics Projects).
