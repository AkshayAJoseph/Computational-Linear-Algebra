##  Pseudocode for Linear Algebra
///python
FUNCTION matrix_sum(A,B);
  Get the number of rows and columns in matrix A
  Create an empty matrix C with same dimensions
  FOR each row i;
    FOR each column j;
      Set C[i][j] to the sum of A[i][j] and B[i][j]
  RETURN the matrix C
END FUNCTION
# Math
  $$
  A=\begin{pmatrix}
    1&2&3\\
    3&4&5\\
    5&6&7\\
    \end{pmatrix}
    $$
		
import numpy as np
import numpy.linalg as la
import array_to_latex as a2l
from IPython.display import display, Latex
# creating a 2X2 Numpy matrix
A = np.array([[50, 29], [30, 44]])
# Displaying the Matrix
print("Numpy Matrix is:")
print(A)

$$
A=\begin{bmatrix}
  50.00 &  29.00\\
  30.00 &  44.00\\
  \end{bmatrix}
  $$
