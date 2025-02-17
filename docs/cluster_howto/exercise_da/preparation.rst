Preparation
===========

Using the commands below to download :download:`the exercise package <torque_exercise.tgz>` and check its content.

.. code-block:: bash

    $ cd
    $ wget https://github.com/Donders-Institute/hpc-wiki-v2/raw/master/docs/cluster_howto/exercise_da/torque_exercise.tgz
    $ tar xvzf torque_exercise.tgz
    $ cd torque_exercise
    $ ls
    subject_0  subject_1  subject_2  subject_3  subject_4  subject_5 ...

In the package, there are folders for subject data (i.e. ``subject_{0..5}``).  In each subject folder, there is a data file containing an encrypted string (URL) pointing to the subject's photo on the Internet.

In this fake analysis, we are going to find out who our subjects are, using an trivial "analysis algorithm" that does the following two steps in each subject folder:

#. decrypting the URL string, and
#. downloading the subject's photo.