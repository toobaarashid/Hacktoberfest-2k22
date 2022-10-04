<!This pseudocode is for Strassen's Multiplication Algorithm which uses Divide and Conquer Approach and limits the time complexity to O(n^3)>

## MM(A,B,N) <!A and B are matrices while N is the dimension of matrices>
{\
  if(n<=2)\
  {\
    c11 = a11b11 + a12b21\
    c12 = a11b12 + a12b22\
    c21 = a21b11 + a22b21\
    c22 = a21b12 + a22b22\
  }\
  else\
  {\
    N=N/2\
    MM(A11,B11,N/2) + MM(A12,B21,N/2)\
    MM(A11,B12,N/2) + MM(A12,B22,N/2)\
    MM(A21,B11,N/2) + MM(A22,B21,N/2)\
    MM(A21,B12,N/2) + MM(A22,B22,N/2)\
  }\
}

> For Reference, 

      [a11 a12]       [b11 b12]
      [a21 a22]       [b21 b22]
