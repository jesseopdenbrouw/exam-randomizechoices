# The exam-randomizechoices package #
- - - -

#### LaTeX package for creating random placed choices in multiple choice environments using the ``exam`` document class. ####

This package can be used with the ``exam`` document class to typeset multiple choice questions with
randomized typesetting of the possible choices. After loading this class, four new environments
are available:

* ``randomizechoices`` -- the randomizing variant of ``choices``;
* ``randomizeoneparchoices`` -- the randomizing variant of ``oneparchoices``;
* ``randomizecheckboxes`` the randomizing variant of ``checkboxes``;
* ``randomizeoneparcheckboxes`` -- the randomizing variant of ``oneparcheckboxes``.

The package is loaded as given below

``\\usepackage[`` *options* ``]{exam-randomizechoices}``
    
Options can be:

* ``randomize`` -- This option globally turns on the randomizing of the choices given for all available typesetting environments. Randomization is turned on by default.


* ``norandomize`` -- This option globally turns off the randomizing of the choices for all available typesetting environments. This option is useful for inspecting the resulting PDF output file with typesetting the choices in the order they were entered.

* ``keeplast`` This option globally turns on the preservation of the last entered item in the new environments.

* ``nokeeplast -- This option globally turns off the preservation of the last entered item in the new environments. This is the default behaviour.

* ``overload`` -- This option makes the standard multiple choice environments behave the same as the new environment counterparts, i.e. the the standard multiple choice environments are overloaded (or redefined). This is useful if you wish to use an old exam and randomize the choices of the questions.

* ``nooverload`` -- This option suppresses the overloading of the standard multiple choice environments so you have to use the new multiple choice environments if you want to randomize the choices to the questions. Overloading is turned off by default.

* ``debug`` -- This option causes the package to emit a lot of debug messages. Debug is turned off by default.
