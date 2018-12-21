# Deep Learning class - installation instructions

Download the Anaconda distribution for your Operating System
(Windows, macOS or Linux):

   - https://www.anaconda.com/download (~500 MB)
   - Choose **Python 3.7**
   - Choose "64-bit installer"

Follow the instructions of the Anaconda page to install anaconda
on your laptop.

Open a console / terminal and create a new virtual environment with conda,

    conda create -n dl-lectures-env -c conda-forge --file requirements.txt python=3.6
    activate dl-lectures-env
    jupyter notebook

This installs tensorflow and keras (without GPU support).

Check that you can import tensorflow with the python from anaconda:

    python3 -c "import tensorflow as tf; print(tf.__version__)"
    1.4.1

We tested the notebooks with keras 2.1.2 and tensoflow 1.4.1.

Ideally: create a new jupyter notebook and check that you can import
the numpy, matplotlib, keras and tensorflow  modules.


# Troubleshooting 

In a console check the installation location of the conda command in
your PATH:

    conda info

Read the output of that command to verify that your conda command is
associated with Python 3.6.


Check that the pip command in your PATH is the one installed by conda:

    pip show pip

and check that it matches:

    python3 -m pip show pip

In particular, look at the "Location:" line of pip is a subfolder
of the "environment root:" line from "conda info".

If you cannot solve your installations without the help of fellow students,
please feel free to send an email to the instructors with the outputs of the
previous command and include the full error messages along with the name and
version of your operating system.

