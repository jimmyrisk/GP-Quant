# GP-Quant
Companion code for Gaussian Process Models for Quantitative Finance by Mike Ludkovski and Jimmy Risk

### Versions

All companion code was ran successfully with the following versions:

* ``R``: 4.2.1
* ``Python``: 3.11.4
  * Packages: ``numpy`` 1.25.2, ``matplotlib`` 3.9.2, ``seaborn`` 0.13.2; **ch2 and ch3**: ``torch`` 2.0.1, ``gpytorch`` 1.11; **ch7**: ``tensorflow`` 2.17, ``tensorflow-probability`` 0.24.0

### Chapter 2 Notebook
([Chapter 2 Notebook](./ch2_py.ipynb)) This notebook is in Python and reproduces plots from Chapter 2, demonstrating Gaussian Process surrogates using a synthetic univariate response function \( f(x) = -0.1 x^2 + \sin(3x) \).  It uses the GPyTorch library.  **IMPORTANT!**  Place `easygpr_helper.py` in the same directory as the notebook for the code to run.  

### Chapter 3 Notebook
([Chapter 3 Notebook](./ch3_py.ipynb)) This notebook is in Python and covers further details of Gaussian Process modeling, comparing different kernel configurations and hyperparameter tuning across varying training set sizes. It also uses GPyTorch and requires the `easygpr_helper.py` file for execution. 

### Chapter 5 Notebook
([Chapter 5 Notebook](./ch3_py.ipynb)) This notebook is in R and illustrates the use of Gaussian Process surrogates for estimating option prices and Greeks, focusing on both the Heston and Black-Scholes models. It demonstrates GP fitting, hyperparameter optimization, and inference of Delta, Theta, and Gamma using both Squared-Exponential and Matern-5/2 kernels.

### Chapter 6 Notebook
([Chapter 6 Notebook](./ch3_py.ipynb)) This notebook is in R and tackles Bermudan option pricing with Gaussian Processes using the Regression Monte Carlo (RMC) approach. It applies the [``mlOSP``](https://github.com/mludkov/mlOSP) package to build emulators for Bermudan Put options, showing both one- and two-dimensional examples. It includes dynamic emulation, sequential design, and adaptive batching techniques.

### Chapter 7 Notebook
([Chapter 7 Notebook](./ch7_py.ipynb)) This notebook constructs a Gaussian Process model for natural gas forward curves, modeling annual seasonality with additive kernels. It uses the TensorFlow library and reproduces Figure 7.2 from Section 7.2. 
