
Variance
Variance (σ2) is a measurement of the spread between numbers in a data set. It measures how far each number in the set is from the mean and is calculated by taking the differences between each number in the set and the mean, squaring the differences (to make them positive) and dividing the sum of the squares by the number of values in the set.Variance measures the variation of a single random variable.

        Var(x) = (1/(n-1))sum(x(i) - mean(x)) * 2
        
        where n = samples
              i = some arbitary number
              the value of x varies from i to n.

A variance value of zero indicates that all values within a set of numbers are identical; all variances that are non-zero will be positive numbers. A large variance indicates that numbers in the set are far from the mean and each other, while a small variance indicates the opposite.




Covariance
The covariance of two variables (x and y) can be represented as cov(x,y). If E[x] is the expected value or mean of a sample ‘x’, then cov(x,y) can be represented in the following way:

        cov(x, y) = E[(x - mean(x))(y - mean(y))]
                    E[x.y]- E[x]E[y]
                    E[x.y] - mean(x)mean(y)
                    
If we look at a single variable, say ‘y’, cov(y,y), the expression can be written in the following way:
       
       cov(y,y) = Var(y) = E[(y - mean(y))*2]
                    Var(y) = s *2
                    s*2= sample variance
                    
Now as we see, in the image above, ‘s²’ or sampled variance is basically the covariance of a variable with itself. This term can also be defined in the following manner:
        s*2 = cov(x,x) = sum(x(i) - mean(x))*2 / n - 1
        
        where x ranges from i to n.
        
        n = number of samples in data set.
        n - 1 = degree of freedom
        
Degrees of freedom is the number of independent data points that went into calculating the estimate. As we see in the example above, it is not necessarily equal to the number of items in the sample (n).

Covariance is used to analyze the linear relationship between the two variable.The positive and negative value in covariance matrix denotes the increasing and decreasing relationship between the two variables.



What is the variance-covariance matrix?
The diagonal of covariance matrix provides the variance of each individual matrix whereas the off-diagonal element provides the covariance between two variables.
A variance-covariance matrix is a square matrix that contains the variances and covariances associated with several variables. The diagonal elements of the matrix contain the variances of the variables and the off-diagonal elements contain the covariances between all possible pairs of variables.
The variance-covariance matrix is symmetric because the covariance between X and Y is the same as the covariance between Y and X. Therefore, the covariance for each pair of variables is displayed twice in the matrix: the covariance between the ith and jth variables is displayed at positions (i, j) and (j, i).

Many statistical applications calculate the variance-covariance matrix for the estimators of parameters in a statistical model. It is often used to calculate standard errors of estimators or functions of estimators. For example, logistic regression creates this matrix for the estimated coefficients, letting you view the variances of coefficients and the covariances between all possible pairs of coefficients.
