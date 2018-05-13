# Matrices tranform into the new basis vector set

## Transform from new basis to our basis
- Suppose we have 2 basis vectors in a new coordinate system(panda system) as $\hat{p_1} = \begin{bmatrix}3\\1\end{bmatrix}$ and $\hat{p_2} = \begin{bmatrix}1\\1\end{bmatrix}$
- Lets say there is a vector $\hat{r}$ in panda system with coordinates $\hat{r} = \begin{bmatrix}3/2\\1/2\end{bmatrix}$
- To transform this to our basis vector set which is $\hat{e_1} = \begin{bmatrix}1\\0\end{bmatrix}$ and $\hat{e_2} = \begin{bmatrix}0\\1\end{bmatrix}$, perform the following

$$\begin{bmatrix}3&1\\1&1\end{bmatrix} \begin{bmatrix}3/2\\1/2\end{bmatrix}$$
$$=\begin{bmatrix}5\\2\end{bmatrix}$$
- Hence, the $\hat{r}$ vector in our coordinate system is $\hat{v} = \begin{bmatrix}5\\2\end{bmatrix}$

## Transform our basis to new basis

- We will use the _inverse_ of basis vector matrix of the panda system to represent our basis vectors in the panda system and then multiply it with the $\hat{v}$ vector

$$\begin{bmatrix}3&1\\1&1\end{bmatrix}^{-1}\begin{bmatrix}5\\2\end{bmatrix}$$
$$= \frac{1}{2}\begin{bmatrix}1&-1\\-1&3\end{bmatrix}\begin{bmatrix}5\\2\end{bmatrix}$$
$$=\begin{bmatrix}3/2\\1/2\end{bmatrix}$$

- We get back the $\hat{r}$ vector, which confirms the formula.

## Orthonormal basis vectors

- Lets say the vectors in panda's world are ORTHONORMAL to each other
- Lets say the vectors are $\hat{p_1} = \frac{1}{\sqrt{2}}\begin{bmatrix}1\\1\end{bmatrix}$ and $\hat{p_2} = \frac{1}{\sqrt{2}}\begin{bmatrix}-1\\1\end{bmatrix}$
- Use the formula above to find the vector $\hat{r} = \begin{bmatrix}2\\1\end{bmatrix}$

## Projections

- We can transform vectors from one basis to another set of basis vectors if the first basis vectors are ORTHOGONAL to each other(explained in projections module)
- Take `our` version of the vector and dot it with panda's axis to get the vector in panda's world

$$\frac{1}{\sqrt{2}}\begin{bmatrix}1\\3\end{bmatrix}.\frac{1}{\sqrt{2}}\begin{bmatrix}1\\1\end{bmatrix} = \frac{4}{2} = 2$$
- We can do it again with the other panda's axis to get the other component

$$\frac{1}{\sqrt{2}}\begin{bmatrix}1\\3\end{bmatrix}.\frac{1}{\sqrt{2}}\begin{bmatrix}-1\\1\end{bmatrix}=\frac{2}{2}=1$$

- If panda's vectors are NOT ORTHOGONAL, this method WON'T WORK

## Transformations

- If we have a vector $\hat{r}$ in panda's coordinate system(which is represented by matrix $\boldsymbol{B}$) and we want to perform a rotation $\boldsymbol{R}$ on it($\boldsymbol{R}$ is the rotation matrix in OUR BASIS), then using the above steps we can apply the following formula

$$\boldsymbol{B}^{-1}\boldsymbol{R}\boldsymbol{B}\hat{r}$$

- This will get the rotated vector in PANDA's BASIS 
