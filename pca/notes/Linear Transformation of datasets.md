# Linear Transformation of datasets

## Effect on mean
- Suppose we have a mean $\mu$ of a dataset $D$. 
  - If we increase each point in $D$ by 2, then the mean will shift to the right by 2
  $$E[D+a] = a + E[D]$$
  - If we stretch the dataset(multiply each component) by 2, then the mean will increase 2 times
  $$E[D*\alpha] = \alpha * E[D]$$
  - If we apply both operations together, we get
  $$E[\alpha D+a] = \alpha * E[D] + a$$
  
## Effect on (co)variance

- Suppose we have a dataset $D$
  - If we shift every point in the dataset by 2, then the variance of the dataset will not change(as variance is a measure of the spread of data)
  $$var[D+a]=var[D]$$ 
  - If we multiply each point by 2, the distance from the mean of each point will increase by a factor of two. Since variance is a measure of the SQUARE distance, the variance will increase by a factor of 4(2^2=4)
  $$var[\alpha D]=\alpha^2var[D]$$
  
- For a new dataset $D$ with n dimensional points

$$var[AD+b]=Avar[D]A^T$$