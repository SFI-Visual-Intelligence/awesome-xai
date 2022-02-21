# awesome-xai
Resources we like for Explainable Artificial Intelligence: sites, papers, implementations, and more!

This page is set up as part of the Interpretable Learning Spring 2022 curriculum arranged at UiT The Arctic University, but it is open to everyone who wants to contribute - send a pull request if you feel something is missing!

## Primer on explainable artificial intelligence

Briefly, explainable artificial intelligence (XAI) methods try to create machine learning models capable of explaining *how* they arrive at predictions. We can use these methods to verify that the models are using features relevant to prediction, to identify areas where the models need improvement, and to extend our own understanding of the problems the models solve.

We separate between

* **Intrinsic** and **post-hoc** explanations: *intrinsically interpretable* models rely on the model design being inherently understandable, while *post-hoc* methods try to infer conclusions about the model after training
* **Model-specific** and **model-agnostic** explanations: *model-specific* methods rely on certain properties of the model design to provide explanations, while *model-agnostic* methods can be adapted for all models
* **Local** and **global** explanations: *local* explanations attempt to explain specific predictions for a limited set of data points, while *global* explanations show patterns and rules applied for every input point

For a longer introduction, Nirmal Sobha Kartha's article for The Gradient, [Explain Yourself - A Primer on ML Interpretability & Explainability](https://thegradient.pub/explain-yourself/), is highly recommended.

## Libraries and repositories

* [EthicalML/xai](https://github.com/EthicalML/xai)
    * Python library with utilities for showing per-group statistical metrics, plotting feature importance, upsampling/downsampling to balance a dataset against specific attributes

### Interpretable models 
* [scikit-learn](https://scikit-learn.org/stable/index.html) 
    * Python library for data analysis and machine learning, with implementations of [nearest-neighbors](https://scikit-learn.org/stable/modules/neighbors.html#classification) classification, [Lasso regression](https://scikit-learn.org/stable/modules/linear_model.html#lasso), [decision trees](https://scikit-learn.org/stable/modules/generated/sklearn.tree.DecisionTreeClassifier.html), and more
* [glmnet](https://cran.r-project.org/web/packages/glmnet/) 
    * R library for generalized linear models with Lasso or ElasticNet regression

### Post-hoc explanations

* [marcotcr/lime](https://github.com/marcotcr/lime)
    * Python library implementing the [LIME (Local Interpretable Model Explanations) method](https://christophm.github.io/interpretable-ml-book/lime.html)
* [slundberg/shap](https://github.com/slundberg/shap)
    * Python library implementing the [SHAP (SHapley Additive exPlanations) method](https://christophm.github.io/interpretable-ml-book/shap.html)

## Books

* [Interpretable Machine Learning](https://christophm.github.io/interpretable-ml-book/) (2022) by Christoph Molnar
    * Available freely online, available for purchase in PDF/ebook format on Leanpub and in print on lulu.com
* [Interpretable AI](https://www.manning.com/books/interpretable-ai) by Ajay Thampi
    * Part of Manning's MEAP series, publishes in April 2022

## Courses / MOOCs

* [CS335: Fair, Accountable, and Transparent (FAccT) Deep Learning](https://cs335.stanford.edu/) at Stanford University
    * Lectures 3 through 7 discuss interpretable models and explainability methods. [Slides and recorded lectures](https://hci.stanford.edu/courses/cs335/2020/sp/lectures.html) available.

## Articles