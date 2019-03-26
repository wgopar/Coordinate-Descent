# CoordinateDescentExperimentation


This notebook showcases two different approaches to implementing coordinate descent on model defined with cross entropy loss. Coordinate descent does have problems if implemented on non-smooth multivariate functions as the algorithm may get stuck at a non-stationary points. This is because the level curves of the function are not smooth. Besides this, the algorithm does have increased interest in large-scale problems where it has been shown to be competitive to other algorithms when training support vector machines and performing non-negative matrix factorization. 

In this experiment I implement coordinate descent using the following approaches:


* Randomly optimize along a random coordinate.
* Optimize along coordinate with the largest gradient in magnitude

To benchmark the solutions I implemented a standard logistic regression model with out focusing on validation and was just used to obtain Scikit-Learns implementation of gradient descent and final loss. The model is trained with the `wine.data` dataset provided by UCI machine learning repository.
