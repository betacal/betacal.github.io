# Beta calibration: a well-founded and easily implemented improvement on logistic calibration for binary classifiers

[Meelis Kull], [Telmo de Menezes e Silva Filho] and [Peter Flach]

For optimal decision making under variable class distributions and misclassification costs a classifier needs to produce well-calibrated estimates of the posterior probability. Isotonic calibration is a powerful non-parametric method that is however prone to overfitting on smaller datasets; hence a parametric method based on the logistic curve is commonly used. While logistic calibration is designed to correct for a specific kind of distortion where classifiers tend to score on too narrow a scale, we demonstrate experimentally that many classifiers including naive Bayes and Adaboost suffer from the opposite distortion where scores tend too much to the extremes. In such cases logistic calibration can easily yield probability estimates that are worse than the original scores. Moreover, the logistic curve family does not include the identity function, and hence logistic calibration can easily uncalibrate a perfectly calibrated classifier. 



In this paper we solve all these problems with a richer class of calibration maps based on the Beta distribution. We derive the method from first principles and show that fitting it is as easy as fitting a logistic curve. Extensive experiments show that beta calibration is superior to logistic calibration for naive Bayes and Adaboost.

# Packages

To make it easier for practitioners to experiment with our method, we have developed packages for [Python] and [R].

* [Python package] 
* [R package]

# Tutorials

We provide usage tutorials for beta calibration in Python and R.

* [Python tutorial] 
* [R tutorial]

# Documents

## AISTATS2017

Click on the following links to access the paper or download the poster and the presentation slides from AISTATS2017.

* [AISTATS2017 paper] 
* [AISTATS2017 poster] 
* [AISTATS2017 slides]

## Electronic Journal of Statistics

We have published an extended version of the AISTATS2017 paper in the Electronic Journal of Statistics. The most significant additions include additional experiments with logistic regression, random forest, multi-layer perceptron and support vector machine; an empirical investigation of the effect of dataset size on the performance of the various calibration methods; and a novel statistical test that builds on beta calibration to recognise if the model deviates from being well-calibrated.
Click [here] to access the paper.

# Citing Beta Calibration

If you want to cite the AISTATS work, please use the following citation format: 

_Meelis Kull, Telmo Silva Filho, Peter Flach; Beta calibration: a well-founded and easily implemented improvement on logistic calibration for binary classifiers, Proceedings of the 20th International Conference on Artificial Intelligence and Statistics, PMLR 54:623-631, 2017._

For the EJS paper, use the following citation format:

_Meelis Kull, Telmo Silva Filho, Peter Flach; Beyond sigmoids: How to obtain well-calibrated probabilities from binary classifiers with beta calibration. Electron. J. Statist. 11 (2017), no. 2, 5052--5080. doi:10.1214/17-EJS1338SI._

# Support or Contact

If you are having problems executing the experiments or the tutorials, do not hesitate to contact us.

[//]: # (References)
   [Meelis Kull]: <http://www.bris.ac.uk/engineering/people/meelis-kull/>
   [Telmo de Menezes e Silva Filho]: <https://www.researchgate.net/profile/Telmo_Silva_Filho>
   [Peter Flach]: <https://www.cs.bris.ac.uk/~flach/>
   [Python]: <https://www.python.org/>
   [R]: <https://www.r-project.org/>
   [Python tutorial]: <https://github.com/betacal/python/blob/master/tutorial/Python%20tutorial.ipynb>
   [R tutorial]: <https://github.com/betacal/R/blob/master/tutorial/Rtutorial.pdf>
   [Python package]: <https://pypi.python.org/pypi/betacal>
   [R package]: <https://cran.r-project.org/web/packages/betacal/index.html>
   [AISTATS2017 paper]: <http://proceedings.mlr.press/v54/kull17a.html>
   [AISTATS2017 poster]: <https://github.com/betacal/aistats2017/blob/master/aistats2017_beta_calibration_poster.pdf>
   [AISTATS2017 slides]: <https://github.com/betacal/aistats2017/blob/master/aistats2017_beta_calibration_slides.pdf>
   [here]: <https://projecteuclid.org/euclid.ejs/1513306867>
