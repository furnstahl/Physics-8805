# Ohio State University Physics 8805
## "Learning from data: Bayesian methods and (some) machine learning"

### Objectives
In recent years there has been an explosion of interest in the use of Bayesian methods in nuclear physics. These methods are being used to quantify the uncertainties in theoretical work on topics ranging from the NN force to high-energy heavy-ion collisions, develop more reliable extrapolants of nuclear-energy-density functionals towards the dripline, predict the impact that future NICER observations may have on the equation of state of neutron matter, and determine whether or not nucleon resonances are present in experimental data. Meanwhile machine learning is gaining increased currency as a method for identifying interesting signals in both experiments and simulations. While most nuclear-physics Ph.D. students are taught some standard (frequentist) statistics as part of their graduate course work, very few encounter Bayesian methods until they are engaged in research. But Bayesian methods provide a coherent and compelling framework to think about inference, and so can be applied to many important questions in nuclear physics. The overall learning goal of this course is to take students who have had no previous exposure to Bayes’ theorem and show them how it can be applied to problems of parameter estimation, model selection, and machine learning.

This motivation for nuclear physics applies to other physics subfields; the Bayesian statistical methods are the same. 8805 will use nuclear physics applications as examples but no prior knowledge of nuclear physics research will be assumed. Jupyter notebooks will be used extensively throughout the course, so this is also a great opportunity to learn some Python and the use of these notebooks. There will be several guided "mini-projects" on topics including Bayesian parameter estimation, model selection, Bayesian optimization, and Bayesian neutral networks. You will be asked to put together a "project" based on your own physics interests and using methods from the course. Grading will be based on Juypter-based problems and these projects.

### Prerequisites
The course will only assume statistics knowledge at the level taught in undergraduate physics labs (e.g., least-squares fitting) and physics knowledge at the first-year graduate level.

### Learning outcomes
Upon completion of this course students should be able to:

* Apply the rules of probability to derive posterior probability distributions for simple problems involving prior information on parameters and various standard likelihood functions.
* Perform Bayesian parameter estimation, including in cases where marginalization over nuisance parameters is required.
* Use Monte Carlo sampling to generate posterior probability distributions and identify problems where standard sampling is likely to fail.
* Compute an evidence ratio and explain what it means.
* Explain machine learning from a Bayesian perspective and employ a testing and training data set to develop and validate a Gaussian-process model.
* Employ these methods in the context of specific physics problems (examples in class will be taken mostly from nuclear physics, but they have more general applicability).
* Be able to understand, appreciate, and criticize the growing literature on Bayesian statistics and machine learning for physics applications.

### Topics
The following topics will be covered (this is not an exclusive list):

* Basics of Bayesian statistics
* Bayesian parameter estimation
* Why Bayes is better
* MCMC sampling
* Assigning probabilities
* Model selection
* Model checking
* Gaussian processes
* Special topic: Bayesian methods and machine learning. [Note: we will not cover machine learning in great detail, but learn about connections to Bayesian methods, e.g., with Bayesian neural networks as a working example.]
* Special topic: Application of Bayesian methods in (nuclear) physics
