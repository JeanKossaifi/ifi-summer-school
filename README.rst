=============
summer-school
=============
Notebooks for the `IfI Summer School on Machine Learning <http://www.ifi.uzh.ch/en/studies/phd/summer-schools/summerschool2018.html>`_

Requirements
============
You will need a laptop to get the most of the session.
The requirements for the tutorial are to have Python installed, along with PyTorch, TensorLy and sckit-learn. You also need to have the jupyter notebook installed

Installation
============
If you are new to Python or simply want a pain-free experience, I recommend you install the `Anaconda <https://www.anaconda.com/download/>`_ distribution. It comes with all you need shipped-in and ready to use!

Once you have anaconda installed, you want to get either the `Jupyter Lab <http://jupyterlab.readthedocs.io/en/stable/>`_ , or the `Jupyter Notebook <http://jupyter.org/install.html>`_ . Typically, you can simply run:
conda install jupyterlab

For PyTorch, simply follow the `instructions <https://pytorch.org/>`_ . It should be something like:
conda install pytorch torchvision -c pytorch

Finally, to install TensorLy to get the latest version, you can clone the Github repository. In the command line, run:
git clone https://github.com/tensorly/tensorly
cd tensorly
pip install -e .

Or, if you have an issue during installation, you can also use conda:
conda install -c tensorly tensorly

Finally, you can install Scikit-Learn using pip. In the command line, just type:
pip install scikit-learn

Checking whether you have the correct versions
==============================================
First, open a jupyter lab (just type jupyter lab in the command line and open the link that appears) (you can also run the code directly in Python or IPython but it's not as nice). Generally, if you are not already familiar with jupyter lab or jupyter notebook, I recommend you spend a little time exploring as it's a very useful tool.

To check you have all you need, run the following:

.. code-block::
   :python:

  import torch
  import numpy as np
  import tensorly as tl
  import sklearn

  print(torch.__version__)
  print(tl.__version__)

For torch, you should have version of at least 0.4.0 and for TensorLy, if you followed the instructions, you should have 0.3.0.
