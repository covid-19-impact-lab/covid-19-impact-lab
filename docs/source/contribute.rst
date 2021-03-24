.. _contribute:

=================
How To Contribute
=================

Joining CoViD-19 Impact Lab
=============================

We are happy about every person that would like to join our efforts. If you are interested, feel free to contact our community manager Renata Abikeyeva (covid-19-impact-lab@outlook.com). Please include the following information in your email:

- Let us know how you would like to contribute to our initiative!
- Your set of skills (i.e. prior experience working with data, coding, and conducting research).
- Your `GitHub <https://github.com/>`_ account (if your contribution is in the form of code).

We will then get back to you soon!



.. Help Wanted
.. ============

.. ..
.. 	German Speakers
.. 	-----------------
.. 	Have 10 minutes to spare? Then check out our `Tweet Labeling Game <http://web4.bonneconlab.uni-bonn.de/room/labeling_game/>`_ for a fun and easy way to support one of our projects, which aims to evaluate Twitter respones to CoViD-19 in Germany. Thank you for your help!

.. 	.. raw:: html

.. 	    <p align="center"><iframe src="https://giphy.com/embed/dBOMb0EkLCO9LrWbyU" width="240" height="233" frameBorder="0" class="giphy-embed" allowFullScreen></iframe></p><p align="center"><a href="http://web4.bonneconlab.uni-bonn.de/room/labeling_game/">Tweet Labeling Game</a></p>


.. .. _dutchtranslators:

.. Dutch Translators
.. -------------------
.. At the moment we are looking for **Dutch native speakers** who would like to help us with the translation of our `data exploration tool <https://covid-19-impact-lab.iza.org/app>`_ into Dutch.

.. There are three tables. Each has columns that end in ``_english``. These need translation.

.. The following comments apply:

.. - Only rows where ``nice_name_english`` is not missing need translation (if that column exists else everything needs a translation).
.. - You can save the table in any file you like but please send us a .csv, separated by semi-colons (;). That means, do not use semi-colons in any translation!
.. - You can copy and paste from the original Dutch questionnaire where applicable.
.. - The entries in the ``nice_name`` column must be very short. No more than 18 characters, preferably less than 15.

.. If you are interested, please contact us and we will send you the tables and answer any questions you may have. Your help is greatly appreciated!



Coding Guidelines
=================

One could think that due to the very ambitious deadlines we face, coding standards should be relaxed. However this is dangerous. We are working with larger teams than ever and cannot even meet face to face to coordinate our efforts. Even more importantly, we want to produce outputs that affect real policies. This makes it even more important to prevent bugs and ensure reproducibility.

Below we summarize a small set of guidelines that have proven useful in many
`OpenSourceEconomics <https://github.com/OpenSourceEconomics>`_ projects.


Collaboration and Version Control
---------------------------------

**Essential**

- Use git for version control and host your project on our `GitHub page <https://github.com/covid-19-impact-lab>`_. This is the most important of all guidelines on this page.
- Write a good README for your repository. The README should tell a new contributor:
    - What programs have to be installed to run your code
    - How to run your code
    - Where to find additional documentation
    - Whom to contact in case of questions

**Optional**

- Use a Pull Request Workflow: Do not work directly on the master branch but create a new branch for each feature you want to add to your code. Then push this branch, go to the GitHub webpage of your repository and create a pull request. Once you are done, do a squash-merge. This will summarize all commits you made to implement the feature into one.
- Do code reviews: Instead of merging your pull request directly, ask someone who is  familiar with the project for a review and only merge after he or she approves.


Reproducible Research
---------------------

**Essential**

- All outputs can be produced with one command. This can be a master do-file, a Python script or a build system command like waf or make.
- Strict separation of inputs and outputs. Inputs are the original datasets and your code. They are under version control. Everything else can be deleted and re-created with one command
- Use LaTeX instead of Word for your papers and presentations and create your regression tables automatically (i.e. without a manual copy paste step).


**Optional**

- Use the `econ-project-templates <https://econ-project-templates.readthedocs.io/en/stable/>`_ instead of a simple master do-file or script. This will run your tasks in parallel and always only run the steps that actually have to be run.


Python Coding Guidelines
------------------------

**Essential**

- Split your code into meaningful functions and write a docstring for each and every function
- Watch `this video <https://www.youtube.com/watch?v=ARKbfWk4Xyw>`_ by Raymond Hettinger (a Python core developer) about finding and preventing bugs on a time budget.


**Optional**

- Use `pytest <https://docs.pytest.org/en/latest/>`_ and `doctests <https://docs.python.org/3/library/doctest.html>`_ to test your functions. Check the above video by Raymond Hettinger to get started.
- Adhere to this `styleguide <https://estimagic.readthedocs.io/en/latest/contributing/styleguide.html>`_ (It was written for estimagic but is basically used in all OpenSourceEconomics Projects).
