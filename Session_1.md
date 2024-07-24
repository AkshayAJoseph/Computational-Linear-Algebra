##  Pseudocode for Linear Algebra
///python
# Matrix Sum
FUNCTION matrix_sum(A,B);\
  Get the number of rows and columns in matrix A\
  Create an empty matrix C with same dimensions\
  FOR each row i;\
    FOR each column j;\
      Set C[i][j] to the sum of A[i][j] and B[i][j]\
  RETURN the matrix C\
END FUNCTION
# Math
  $$
  A=\begin{pmatrix}
    1&2&3\\
    3&4&5\\
    5&6&7\\
    \end{pmatrix}
    $$

# Matrix Product
FUNCTION matrix_product(A, B):\
    Get the number of rows and columns in matrix A\
    Get the number of columns in matrix B\
    Create an empty matrix C with dimensions rows_A x cols_B\
    FOR each row i in A:\
        FOR each column j in B:\
            Initialize C[i][j] to 0\
            FOR each element k in the common dimension:\
                Add the product of A[i][k] and B[k][j] to C[i][j]
    RETURN the matrix C
END FUNCTION


import numpy as np\
import numpy.linalg as la\
import array_to_latex as a2l\
from IPython.display import display, Latex\
# Creating a 2X2 Numpy matrix
A = np.array([[50, 29], [30, 44]])
# Displaying the Matrix
print("Numpy Matrix is:")\
print(A)

$$
A=\begin{bmatrix}
  50.00 &  29.00\\
  30.00 &  44.00\\
  \end{bmatrix}
  $$
