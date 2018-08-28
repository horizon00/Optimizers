# Optimizers
Types of optimizers

Optimizers

The choice of optimization algorithm for your deep learning model can mean the difference between good results in minutes, hours, and days.

The Adam optimization algorithm is an extension to stochastic gradient descent that has recently seen broader adoption for deep learning applications in computer vision and natural language processing.

In this post, you will get a gentle introduction to the Adam optimization algorithm for use in deep learning.

After reading this post, you will know:

    What the Adam algorithm is and some benefits of using the method to optimize your models.
    How the Adam algorithm works and how it is different from the related methods of AdaGrad and RMSProp.
    How the Adam algorithm can be configured and commonly used configuration parameters.

Let’s get started.

What is the Adam optimization algorithm?

Adam is an optimization algorithm that can used instead of the classical stochastic gradient descent procedure to update network weights iterative based in training data.

Adam was presented by Diederik Kingma from OpenAI and Jimmy Ba from the University of Toronto in their 2015 ICLR paper (poster) titled “Adam: A Method for Stochastic Optimization“. I will quote liberally from their paper in this post, unless stated otherwise.

The algorithm is called Adam. It is not an acronym and is not written as “ADAM”.

    … the name Adam is derived from adaptive moment estimation.

When introducing the algorithm, the authors list the attractive benefits of using Adam on non-convex optimization problems, as follows:

    Straightforward to implement.
    Computationally efficient.
    Little memory requirements.
    Invariant to diagonal rescale of the gradients.
    Well suited for problems that are large in terms of data and/or parameters.
    Appropriate for non-stationary objectives.
    Appropriate for problems with very noisy/or sparse gradients.
    Hyper-parameters have intuitive interpretation and typically require little tuning.

