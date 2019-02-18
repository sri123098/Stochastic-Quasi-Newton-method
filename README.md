# Stochastic-Quasi-Newton-method

![alt text](https://github.com/sri123098/Stochastic-Quasi-Newton-method/blob/master/algorithm.png)

Gradient Descent is a first order oracle optimisation algorithm where as Newton is a second order oracle which means that Newton is super linear in convergence and Gradient Descent is linear in convergence. Moreover, gradient descent takes O(d) computation time complexity per step and Newton takes O(d^3) computation time complexity as it requires the inverse computation. 

To get the best of these two algorithms, we can meet in the middle with the BFGS which is taylor series approximation of the hessian. 

When it comes to Limited BFGS optimisation algorithm, it's an algorithm in which the inverse step update takes account of limited steps instead of taking entire steps which has efficient Memory advantage than BFGS algorithm. 

Both of them are great for convex optimisation algorithms as these algorithms satisfy the curvature condition and therefore maintaining the postive definiteness of Hessian H_k. 
When it comes to non convex optimisation problems, this may not hold good. So, to ensure the positive definiteness of Hessian H_k, check have to be performed and limit the per step accordingly as per the algorithm presented in the paper. 



Stochastic Newton algorithm for non convex optimisation problem has been implemented and validated the algorithm for LSTM networks and observed its benefits. I observed that stochastic algorithms have a convergence rate of O(e^2). 


