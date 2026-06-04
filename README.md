# EFBMC - Elastic Functional Bayesian Model Calibration

[<img src="Logo.png" width="250"/>](Logo.png)

For Python, R, and MATLAB. There is two example notebooks. The one with `_toy` in the filename is a toy dataset. The other is an example calibration Equation of State model from the Z-machine.

## Getting started with Python
For the python code you need to have python 3.9 or later installed. We recommend anaconda and you can create an `conda` environment with the needed requirements using the following command

```bash
conda create -n EFBMC -c conda-forge fdasrsf seaborn scikit-learn pytest pandas pybind11 jupyterlab
conda activate EFBMC
pip install git+https://github.com/lanl/pyBASS.git
pip install git+https://github.com/gqcollins/pyBayesPPR.git
pip install "git+https://github.com/sandialabs/mvBayesPy"
pip install git+https://github.com/lanl/impala/impala.git
```

to install other surrogate models (e.g., BART (stochtree))
```
pip install git+https://github.com/StochasticTree/stochtree.git
```

You then can run the example notebook above

## Getting started with R
For the R code you will need to the following R packages installed

```R
install.packages(c("fdasrvf","BASS","stochtree","bayesplot","readr","interp","hexbin","remotes"))
library(remotes)
install_git("https://github.com/sandialabs/rImpala")
install_git("https://github.com/sandialabs/mvBayesR")
```

## Getting started with MATLAB
For the MATLAB code you will need to the following MATLAB packages in your path

1. [impala](https://github.com/sandialabs/impala_matlab)
2. [fdasrvf](https://github.com/jdtuck/fdasrvf_MATLAB)
3. [mvBayes](https://github.com/sandialabs/mvbayes_matlab)
4. [BASS](https://github.com/sandialabs/BASS_matlab)
5. [BayesPPR](https://github.com/sandialabs/BASS_matlab)

## References
D. Francom, J. D. Tucker, J. G. Huerta, K. Shuler, and D. Ries, "Elastic Bayesian Model Calibration", *SIAM/ASA Journal on Uncertainty Quantification*, vol. 13, no. 1, 2025. [PDF](http://research.tetonedge.net/Papers/Francom-2025-Calibration-JUQ.pdf)

J. Brown, J. P. Davis, J. D. Tucker, J. G. Huerta, and K. Shuler, "Quantifying uncertainty in analysis of shockless dynamic compression experiments on platinum, Part 2: Bayesian model calibration", *Journal of Applied Physics*, vol. 134, no. 23, 2023. [PDF](http://research.tetonedge.net/Papers/JAP23_calibration.pdf)

## Contact
For questions please contact J. Derek Tucker (5573) or Gavin Collins (5573)\
jdtuck@sandia.gov\
gqcolli@sandia.gov
