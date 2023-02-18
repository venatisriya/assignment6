# Assignment6
## Sriya Reddy

In this assignment, the task was to create two matrices and perform addition and subtraction operations, followed by learning to use the `diag()` function in various ways.

As instructed, I created two matrices of shape `2 x 2` using the following lines of code.
```
> A = matrix(c(2,0,1,3), ncol=2)
> B = matrix(c(5,2,4,-1), ncol=2)
```
To find A + B, I used the following code and obtained the result as shown.
```
> A+B
     [,1] [,2]
[1,]    7    5
[2,]    2    2
```

To find A - B, I used the following code and obtained the result as shown.
```
> A-B
     [,1] [,2]
[1,]   -3   -3
[2,]   -2    4
```

For the second task, I need to create a diagonal matrix with the elements [4,1,2,3] on the diagonal.
To achieve this, I first created a `4 x 4` zero matrix as shown.
```
> X = matrix(0,4,4)
> X 
     [,1] [,2] [,3] [,4]
[1,]    0    0    0    0
[2,]    0    0    0    0
[3,]    0    0    0    0
[4,]    0    0    0    0
```

I now used the `diag()` function to change the diagonal elements of the `X` matrix.

```
> diag(X) = c(4,1,2,3)
> X 
     [,1] [,2] [,3] [,4]
[1,]    4    0    0    0
[2,]    0    1    0    0
[3,]    0    0    2    0
[4,]    0    0    0    3
```

For the third task, I need to create a `5 x 5` matrix as shown with 3s in the diagonal, 1s in the first row and 2s in the first column. 
To achieve this, I first created a diagonal matrix of size `5 x 5` with 3s in the diagonal with the following code. 
```
> matrix_3 = diag(3,5,5)
> matrix_3
     [,1] [,2] [,3] [,4] [,5]
[1,]    3    0    0    0    0
[2,]    0    3    0    0    0
[3,]    0    0    3    0    0
[4,]    0    0    0    3    0
[5,]    0    0    0    0    3
```

I then replaced the last 4 elements of the first row with 1s using the following command.
```
> matrix_3[1, 2:5] = 1
> matrix_3
     [,1] [,2] [,3] [,4] [,5]
[1,]    3    1    1    1    1
[2,]    0    3    0    0    0
[3,]    0    0    3    0    0
[4,]    0    0    0    3    0
[5,]    0    0    0    0    3
```

The resulting matrix has 1s in the first row.

I then replaced the last 4 elements of the first column with 2s using the following command.
```
> matrix_3[2:5, 1] = 2
> matrix_3
     [,1] [,2] [,3] [,4] [,5]
[1,]    3    1    1    1    1
[2,]    2    3    0    0    0
[3,]    2    0    3    0    0
[4,]    2    0    0    3    0
[5,]    2    0    0    0    3
```

The resulting matrix now has the required elements in the required locations. 
