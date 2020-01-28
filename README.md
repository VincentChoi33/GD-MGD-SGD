# GD-MGD-SGD


##Practice : Source localization problem


-> Given : N-locations a_1, a_2,...,a_N \in R^m of seonsors and approximate distaces d_i between the sensors and an unknown "source" located at x \in R^m:

-> Goal : find and estimate x \in R^m given the locations a_1,a_2,...,a_N and d_1,d_2,...,d_N

-> optimization problem - a nonlinear least squares problem

\minx f(x) \equi \sum{i=1}^N(||x-a_i||_2^2 -d_i^2)^2

calculation of \nabla f(x) : \frac{\part f}{\part x_j}(x) = 4 \sum_i=1^N (||x-a_i||_2^2-d_i^2)(x-a_i)
