##  Pseudocode for Linear Algebra
///python
FUNCTION matrix_sum(A,B);
  Get the number of rows and columns in matrix A /t
  Create an empty matrix C with same dimensions /t
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

    ///python
    # importing Numpy package
import numpy as np
import numpy.linalg as la
import array_to_latex as a2l
from IPython.display import display, Latex

