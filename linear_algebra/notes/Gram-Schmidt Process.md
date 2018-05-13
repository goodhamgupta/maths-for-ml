# Gram-Schmidt Process

- Orthonormal basis sets makes computation easier
  - This method helps construct orthonormal basis set vectors
- Lets say we have some vectors $\boldsymbol{V} = {v_1,v_2..v_n}$ that span the space we are interested in and that these vectors are linearly independent
  - check for linear independence, 
    - write the vectors down as a column matrix and check if the determinant is non-zero. 
    - If they are NOT linearly independant,  then the determinant will be zero
- These vectors are NOT ORTHONORMAL to each other

## Steps

- Take first vector in $\boldsymbol{V}\text{ i.e }v_1$ 
- Let's say this vector survives and we say our new orthonormal basis vector is equal to the normalized vector of $v_1$
$$e_1 = \frac{v_1}{|v_1|}$$
- Hence, $e_1$ is just the unit vector in the direction of $v_1$
- To compute the vector $v_2$, it will be composed of two things(refer the minute 2:00 [here](https://www.coursera.org/learn/linear-algebra-machine-learning/lecture/28C1t/the-gram-schmidt-process))
  - A component in the direction of $v_1$
    - Find this using vector projection of $v_2$ onto $e_1$ 
    - $\frac{v_2.e_1}{|e_1|}e_1= (v_2.e_1)e_1$ since $|e_1|=1$ as it is a unit vector
  - A component perpendicular to $e_1$
    - If we call this $u_2$ then using the above formula we get
    - $v_2=(v_2.e_1)e_1 + u_2$
    - $u_2 = v_2-(v_2.e_1)e_1$ after rearranging
- If we normalize $u_2$ we get $\frac{u_2}{|u_2|}=e_2$ which will be a normal vector to $e_1$
- Now, if we want to compute $e_3$ which will be a orthonomal unit vector of $v_3$, we will do the following
  - $v_3$ does not exist in the space spanned by $v_1$ and $v_2$ as it is not a linear combination of them 
  - Hence, it is not in the place defined by $e_1$ and $e_2$ either
  - We project $v_3$ down onto the plane defined by $e_2$ and $e_1$.This vector will be
  - $u_3 = v_3 - (v_3.e_1)e_1 - (v_3.e_2)e_2$
  - If we compute the normal vector of $u_3$ we get
  - $e_3=\frac{u_1}{|u_1|}$ which is a vector normal to $e_1$ and $e_2$
- We continue this process till we get a set of vectors $\boldsymbol{E}$ that are an orthonormal basis set of vectors
- This will make computation easier