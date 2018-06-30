==========================================
IfI Summer School 2018 on Machine Learning
==========================================

Slides and material for tensor methods course at the `IfI Summer School on Machine Learning <http://www.ifi.uzh.ch/en/studies/phd/summer-schools/summerschool2018.html>`_

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

Some more readings
==================
Here are some more recommended readings:

For a great introduction on tensor decompositions:

* Tamara G. Kolda and Brett W. Bader. Tensor decompositions and applications. SIAM REVIEW, 51(3):455–500, 2009.

Another great review:

* Sidiropoulos, N.D., De Lathauwer, L., Fu, X., Huang, K., Papalexakis, E.E. and Faloutsos, C., 2017. Tensor decomposition for signal processing and machine learning. IEEE Transactions on Signal Processing, 65(13), pp.3551-3582.

The reference paper for learning latent variable models (e.g. topic modelling) using tensor decomposition:

* Animashree Anandkumar, Rong Ge, Daniel J Hsu, Sham M Kakade, and Matus Telgarsky. Tensor decompositions for learning latent variable models. Journal of Machine Learning Research, 15(1):2773–2832, 2014.

Tensor Faces:

* Vasilescu, M.A.O. and Terzopoulos, D., 2002, May. Multilinear analysis of image ensembles: Tensorfaces. In European Conference on Computer Vision (pp. 447-460). Springer, Berlin, Heidelberg.

Analysing neural nets with tensor methods:

* Nadav Cohen, Or Sharir, and Amnon Shashua. On the expressive power of deep learning: A tensor analysis. CoRR, abs/1509.05009, 2015
* Majid Janzamin, Hanie Sedghi, and Anima Anandkumar. Generalization bounds for neural networks through tensor factorization. CoRR, abs/1506.08473, 2015a.
* Majid Janzamin, Hanie Sedghi, and Anima Anandkumar. Beating the perils of non-convexity: Guaranteed training of neural networks using tensor methods. CoRR, 2015b
* Hanie Sedghi and Anima Anandkumar. Training input-output recurrent neural networks through spectral methods. CoRR, abs/1603.00954, 2016.

Compressing convolutional layers of deep nets:

* Yong-Deok Kim, Eunhyeok Park, Sungjoo Yoo, Taelim Choi, Lu Yang, and Dongjun Shin. Compression of deep convolutional neural networks for fast and low power mobile applications. CoRR, abs/1511.06530, 2015
* Vadim Lebedev, Yaroslav Ganin, Maksim Rakhuba, Ivan V. Oseledets, and Victor S. Lempitsky. Speeding-up convolutional neural networks using fine-tuned cp-decomposition. CoRR, abs/1412.6553, 2014.

Low-rank tensor regression:

* W Guo, I. Kotsia, and I. Patras. Tensor learning for regression. IEEE Transactions on Image Processing, 21(2):816–827, Feb 2012
* Qi Rose Yu and Yan Liu. Learning from multiway data: Simple and efficient tensor regression. CoRR, abs/1607.02535, 2016.
* Guillaume Rabusseau and Hachem Kadri. Low-rank regression with tensor responses. In D. D. Lee, M. Sugiyama, U. V. Luxburg, I. Guyon, and R. Garnett (eds.), NIPS, pp. 1867–1875. 2016.


Tensor Regression Networks and Tensor Contraction Layers:

* Kossaifi, J., Lipton, Z.C., Khanna, A., Furlanello, T. and Anandkumar, A., 2017. Tensor Regression Networks. arXiv preprint arXiv:1707.08308.
* Kossaifi, J., Khanna, A., Lipton, Z., Furlanello, T. and Anandkumar, A., 2017, July. Tensor contraction layers for parsimonious deep nets. In Computer Vision and Pattern Recognition Workshops (CVPRW), 2017 IEEE Conference on (pp. 1940-1946). IEEE.

Tensorizing neural networks (ttrain decomposition on the weights of a fully-connected layers):

* Novikov, A., Podoprikhin, D., Osokin, A. and Vetrov, D.P., 2015. Tensorizing neural networks. In Advances in Neural Information Processing Systems (pp. 442-450).

On TensorLy:

* Kossaifi, J., Panagakis, Y. and Pantic, M., 2016. Tensorly: Tensor learning in python. arXiv preprint arXiv:1610.09555.
