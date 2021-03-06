Code description
================

``reval`` module has one superclass :class:`FindBestClustCV` and a subclass :class:`RelativeValidation`.

Classes
-------

.. autoclass:: reval.relative_validation.RelativeValidation
   :members:
   :private-members:

.. autoclass:: reval.best_nclust_cv.FindBestClustCV
   :members:
   :private-members:

Functions
---------

Useful functions that can be used on their own are also available. In particular,
``reval.relative_validation._kuhn_munkres_algorithm`` performs consistent permutation of predicted labels
in order to minimize the misclassification error with respect to true labels. Kuhn-Munkres algorithm is used
(Kuhn, 1955; Munkres, 1957)

Kuhn, H. W. (1955). The Hungarian method for the assignment problem. *Naval research logistics quarterly*,
2(1‐2), 83-97.

Munkres, J. (1957). Algorithms for the assignment and transportation problems.
*Journal of the society for industrial and applied mathematics*, 5(1), 32-38.

.. automodule:: reval.relative_validation
   :members: _kuhn_munkres_algorithm
   :private-members:

The ``reval.best_nclust_cv._confint`` computes 95% confidence interval using ``scipy.stats.t.ppf()`` function.

.. automodule:: reval.best_nclust_cv
   :members: _confint
   :private-members:


Visualization
-------------

``reval.visualization`` enables plotting the cross-validation performance.

.. automodule:: reval.visualization
   :members:
   :private-members:
