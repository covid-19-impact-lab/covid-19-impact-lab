=====================
Tech Support and Help
=====================


We have a Zulip channel for tech-support related to CoViD-19 Impact Lab projects. We do not only want to help you to debug your code once it is too late, but can give you some recommendations on how to tackle a project even before you start. For example, which packages to use, how to structure your project and which blogposts to read. Maybe we even find a collaborator for your project or already have code that does what you wanted to implement.

Below we describe the different sub-channels and how you should ask your questions such that we can help you efficiently.

Designing a Large Project
==========================

Situation
---------

You have a rough idea what you want to do (maybe started to implement it) but are not satisfied with your approach for one of the following reasons:

- You think it is going to take very long to implement it in your way
- You suspect that there already is code to solve your problem, you just could not find it
- The code you drafted is unreadable and difficult to use and extend by others
- You have no experience to design code that is used by others and want an interface recommendation


What you should do
------------------

1. Write a short description of what you want to achieve. Make sure that it does not contain any implementation details. The style of your description should be like a readme to the ideal program you can imagine. If possible and applicable, include a `user story <https://www.freecodecamp.org/news/how-and-why-to-write-great-user-stories-f5a110668246/>`_.
2. (Very briefly describe what you already did)
3. Post it in the corresponding zulip channel and let us know when you have time for a call.


Implementing a Specific Feature
================================

Situation
---------

You have a concrete question about implementing something in Python. For example, you need to clean a Dataset and suspect that there is a pandas function that does what you want, but you cannot find it. Or you need to optimize a function but do not have previous experience.

What you should do
------------------

Formulate your task as precisely as possible: First describe what you have (e.g. the dataset you want to clean), then describe what you need. Ideally, you do this in form
of a function interface, e.g.:

.. code-block:: python

    def calculate_standardized_score_in_panel_data(data, variables):
        """Calculate score in a panel dataset, standardized for each period.

        Args:
            data (pd.DataFrame): Here you describe the exact structure of your dataset.
                If it has a MultiIndex, describe the index.
            variables (list): List of strings with variables to aggregate into a score.

        Returns:
            pd.Series: Here you describe the output

        """

The most likely thing is that writing the problem down so precisely already gives you an idea for the solution. If not, post it on Zulip and we will find someone who solves your problem.


Debugging Code
================

Situation
---------

You have written some code, but it does not run or it runs but produces the wrong output.

What you should do
------------------

Read `this great article <http://matthewrocklin.com/blog/work/2018/02/28/minimal-bug-reports>`_ on writing bug reports and write a bug report in the zulip channel.


Solving Installation Problems
==============================

Situation
---------

You want to use an OpenSourceEconomics package, the project templates or just some python package but run into problems installing it on your computer. You have googled the problem but could not find a solution.



What you should do
------------------

Describe the problem as precisely as possible:

- What operating system (including version) are you using
- Which package do you want to install
- How did you try to install the package (pip, conda, from source, environment file)
- What is the exact problem (error messages during installation, failing tests after installation, installation works but import fails, ...)

We will than try to find someone who managed to install this package on the same operating system and get back to you.
