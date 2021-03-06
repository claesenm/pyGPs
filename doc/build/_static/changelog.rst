
Changelog pyGPs v1.2
=====================

June 30th 2014
----------------

structural updates:

- input target now can either be in 2-d array with size (n,1) or in 1-d array with size (n,)
- setup.py updated
- "import pyGPs" instead of "from pyGPs.Core import gp"
- rename ".train()" to ".optimize()"
- rename "Graph-stuff" to "graphExtension"
- rename kernelOnGraph to "nodeKernels" and graphKernel to "graphKernels"
- redundancy removed for model.setData(x,y)
- rewrite "mean.proceed()" to "getMean()" and "getDerMatrix()"
- rewrite "cov.proceed()" to "getCovMatrix()" and "getDerMatrix()"
- rename cov.LIN to cov.Linear (to be consistent with mean.Linear)
- rename module "valid" to "validation"
- add graph dataset Mutag in python file. (.npz and .mat)
- add graphUtil.nomalizeKernel()
- fix number of iteration problem in graphKernels "PropagationKernel"
- add unit testing for covariance, mean functions



bug fixes:

- derivatives for cov.LINard
- derivative of the scalar for cov.covScale
- demo_GPR_FITC.py missing pyGPs.mean



July 8th 2014
----------------

structural updates:

- add hyperparameter(signal variance s2) for linear covariance
- add unit testing for inference,likelihood functions as well as models
- NOT show(print) "maximum number of sweep warning in inference EP" any more
- documentation updated

bug fixes:

- typos in lik.Laplace
- derivative in lik.Laplace


July 14th 2014
----------------

documentation updates:

- online docs updated
- API file updated

structural updates:

- made private for methods that users don't need to call
