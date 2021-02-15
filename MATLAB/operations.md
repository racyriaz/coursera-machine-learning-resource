# MATLAB COMPUTATIONS ON DATA

  1. TO ADD / SUBTRACT / MULTIPLY / DIVIDE
    + `>> 5 + 6`, returns `ans = 11`
      + if you dont give a variable to store the calculation then it would use the default **ans** variable.
  2. MATRIX AND VECTORS
    + Matrix variable are denoted in UpperCase letters, Vectors are denoted in LowerCase letters.
    + In a Vector
      + **Row** is represented as [1 2 3] which is a 1x3 matrix
      + **Columns** are represented as [1 ; 2 ; 3 ] which is a 3x1 matrix

    + In Matrices,
      + [ 1 2 3 ; 7 5 3 ; 4 2 4 ] represents a 3x3 matrix
      + the row can also be separated with **,** than space

  3. MATRIX/VECTOR ADDITION AND SUBTRACTION
    + They are performed element by element so no problem

  4. MATRIX x VECTOR
    + [refer this]()

  5. MATRIX X MATRIX
    + [refer this]()

  6. MATRIX/VECTOR x SCALAR
    + [refer this]()

  7. ELEMENT WISE OPERATION:
    + Use `.*` to perform **element wise product** in Matlab/Octave
    + Use `A .^ 2` to perform **element wise squaring** to the matrix
    + Use `1 ./ A` to perform **element wise reciprocal/inverse of matrix A**
    + log(v) &rarr; element wise log
    + exp(v) &rarr; element wise log
    + abs([1;2;3]) &rarr; converts negative values ↣ positive values

  8. `length(v)`
    + returns the length of the vector ||y to size of operator

  9. `ones(2,3)` or `zeros(2,3)`
    + returns a matrix of 1 or 0 with a dimension of 2x3

  10. `A'`
    + returns a Transpose of the matrix A
    + (A')' == A

  11. `max(a)`
    + returns the max value in the vector a
    + `[val, ind] = max(a)` returns the max value and its index position (list unpacking)

  12. CONDITIONAL STATEMENTS WITH MATLAB
    + `a < 3` returns a bool value with elements wise comparison say suppose if a value is [1,3,6] then `a<3` would result in [0 0 1 ], 0 &rarr; False (condition failed) and 1 &rarr; True (condition passed)

  13. `find(a < 3)`
    + returns the index of the position where the condition was satisfied
    + for Matrix use `[r, c] = find(A > 7)`, List unpacking where r &rarr; row index, c &rarr; column index

  14. `magic()`
    + returns a matrix of magic square where sum of row and columns and diagonals in any direction are equal
    eg. A = magic(3) <br /> A =  <br />8 1 6<br />3 5 6 <br />4 9 2<br />

  15. `help ___` or `doc ____`
    + returns the definition for the inbuilt functions

  16. PRODUCT OF ELEMENTS `prod(a)`
    + returns a rounded product of elements in a vector

  17. GENERATING RANDOM NUMBERS
    + `rand(3)` &rarr; returns a matrix of 3x3 random numbers from 0.00000 ... to 1.0000 ....
    + `max(rand(3), rand(3))` &rarr; takes two random matrix returns the element wise max of two matrix


  18. CONVERT A MATRIX INTO VECTOR
    + `A(:)`

  19. COLUMN/ROW WISE MAXIMUM ELEMENTS
    + `max(A,[],1)` &rarr; returns column wise max of a matrix
    + `max(A,[],2)` &rarr; returns row wise max of a matrix
    + TO GET MAX OF THE ENTIRE MATRIX USE
      + `max(max(A))`
      + `max(A(:))` converts a matrix into vector then find the max in the entire vector

  20. SUMMING ROW/COLUM WISE
    + sum(A,1) &rarr; column wise sum
    + sum(A,2) &rarr; row wise sum

  21. IDENTITY MATRIX
    + `eye(5)` &rarr; [ 1 0 0; 0 1 0; 0 0 1 ]

  22. SUM OF DIAGONALS
    + 1. `B = A .* eye(3)` &rarr; produces diagonal elements and others are 0
      2. `sum(sum(B))` &rarr; gives sum of diagonal elements
    + **opposite diagonal | Flip Up-Down**: `flipud(eye(3))` &rarr; [ 0 0 1; 0 1 0; 1 0 0 ]

  23. INVERSE OF A
    + `pinv(A)`
