## Special Orthogonal Group SO(3)
1. **definition**:
    SO(3) is a group of 3*3 orthogonal matrices with determinant of 1. These matrices represent the rotation in a space.

2. **qualities**:
    Matrix R in SO(3) satisfied $R^TR = RR^T = I$, and $det(R) = 1$

3. **applications**:
    SO(3) describes a rotation in a 3D space, which is irrelevant to shifts.

## Special Euclidean Group SE(3)
1. **definition**:
    SE(3) is a group consists of all rotation and shift matricies. The matrix can be represented by a 4*4 matrix, which includes a SO(3) rotation matrix and a 3 dimension shifting vector.

2. **qualities**:
    The representation of SE(3) matrix often are denote as $\begin{pmatrix} R & v \\ 0 & 1 \\ \end{pmatrix}$. 

3. **applications**: SE(3) describes rotations and shifts of an object in a 3D space.

