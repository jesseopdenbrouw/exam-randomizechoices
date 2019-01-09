# The exam-randomizechoices package #
----------

#### LaTeX package for creating random placed choices in multiple choice environments using the [``exam``](https://ctan.org/pkg/exam) document class. ####

This package can be used with the [``exam``](https://ctan.org/pkg/exam) document class to typeset multiple choice questions with randomized typesetting of the possible choices. After loading this package, four new environments are available:

* ``randomizechoices`` -- the randomizing variant of ``choices``;
* ``randomizeoneparchoices`` -- the randomizing variant of ``oneparchoices``;
* ``randomizecheckboxes`` the randomizing variant of ``checkboxes``;
* ``randomizeoneparcheckboxes`` -- the randomizing variant of ``oneparcheckboxes``.

The package is loaded as given below

``\usepackage[``*options*``]{exam-randomizechoices}``
    
Options can be:

* ``randomize`` -- This option globally turns on the randomizing of the choices given for all available typesetting environments. Randomization is turned on by default.


* ``norandomize`` -- This option globally turns off the randomizing of the choices for all available typesetting environments. This option is useful for inspecting the resulting PDF output file with typesetting the choices in the order they were entered.

* ``keeplast`` This option globally turns on the preservation of the last entered item in the new environments.

* ``nokeeplast`` -- This option globally turns off the preservation of the last entered item in the new environments. This is the default behaviour.

* ``overload`` -- This option makes the standard multiple choice environments behave the same as the new environment counterparts, i.e. the the standard multiple choice environments are overloaded (or redefined). This is useful if you wish to use an old exam and randomize the choices of the questions.

* ``nooverload`` -- This option suppresses the overloading of the standard multiple choice environments so you have to use the new multiple choice environments if you want to randomize the choices to the questions. Overloading is turned off by default.

* ``debug`` -- This option causes the package to emit a lot of debug messages. Debug is turned off by default.

An example of a randomizing choices environment is given below:


    \question[5] What is the result of $1+1$?

    \begin{randomizechoices}
    \choice 1
    \CorrectChoice 2
    \choice 3
    \choice 4
    \end{randomizechoices}

which *possibly* (depends on de state of the pseudo random generator) typesets as:

1\. (5 points) What is the result of 1+1?

   A. 2
   
   B. 1
   
   C. 4
 
   D. 3
   
*** Note: verbatim environments such as [``verbatim``](https://ctan.org/pkg/verbatim) and [``listings``](https://ctan.org/pkg/listings) are not supported ***
   

See the documentation for full explanation of the package.

#### License

This work may be distributed and/or modified under the
conditions of the LaTeX Project Public License, either version 1.3
of this license or (at your option) any later version.
The latest version of this license is in
http://www.latex-project.org/lppl.txt
and version 1.3 or later is part of all distributions of LaTeX 
version 2003/12/01 or later.

This work consists of the files exam-randomizechoices.sty,
exam-randomizechoices.tex and exam-randomizechoices-doc.tex

This software is provided 'as is', without warranty of any kind,
either expressed or implied, including, but not limited to, the
implied warranties of merchantability and fitness for a
particular purpose.



