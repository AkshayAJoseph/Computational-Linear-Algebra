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
!pip install array_to_latex
