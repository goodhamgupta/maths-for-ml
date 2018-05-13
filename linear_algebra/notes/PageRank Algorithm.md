# PageRank Algorithm

- Used to decide which order to display the websites in response to a query
- Importance of a website is related to it's link TO AND FROM other websites


## Steps

- Each link for a page can be described as a vector
  - `1` represents a link exists
  - `0` represents a link does not exist
- Normalize the vector by the total number of links to describe a probability for the page
- Build matrix $\boldsymbol{L}$ in which each of the above vectors will be a column. This matrix will represent the probability of ending up on each of the pages.

@startuml
A ..|> B
A ..|> C
A ..|> D
B ..|> A
B ..|> D
C ..|> D
D ..|> B
D ..|> C
@enduml
- For the above sample pages, we get

$L-A = [0, \frac{1}{3}, \frac{1}{3}, \frac{1}{3}]$
$L-B = [\frac{1}{2}, 0, 0, \frac{1}{2}]$
$L-C = [0, 0, 0, 1]$
$L-D = [0, \frac{1}{2}, \frac{1}{2}, 0]$

We can not build our link matrix $\boldsymbol{L}$
$$\boldsymbol{L} = \begin{bmatrix}0&0&0&0\\\frac{1}{3}&0&0&\frac{1}{2}\\\frac{1}{3}&0&0&\frac{1}{2}\\\frac{1}{3}&\frac{1}{2}&1&0\end{bmatrix}$$

- This problem is self-referential i.e the ranks of all pages depend on the all the other pages
- Matrix $\boldsymbol{L}$ was built using columns of outward links BUT the rows describe the NORMALIZED inward links between pages
- We will use the vector $\vec{r}$ to store the rank of all web pages
- To calculate the rank of a page, we need to know three things about all other pages on the internet
  - What's your rank? 
  - Do you link to the current page(the page we are trying to calculate the rank for)
  - How many outgoing links do you have in total?
- The expresion to represent this mathematically is:
$$\vec{r_A} = \sum_{j=1}^{n}\boldsymbol{L_{A,j}}r_j$$
$$n=\text{total number of web pages}$$
$$\boldsymbol{L_{A,j}} = \text{Link matrix relevant to webpage A and location j}$$
$$r_j = \text{rank of location j}$$
- This will scroll through each of our webpages
- Hence, rank of A => Sum of ranks of all pages which link to it weighted by the specific link probability taken by L
- For all pages, we can rewrite the exp as a matrix multiplication
- Since we do not know the initial value of $\vec{r}$, we simply assume all the ranks are EQUAL and normalize them by the total number of web pages in our analysis

$$r = \begin{bmatrix}\frac{1}{4}\\\frac{1}{4}\\\frac{1}{4}\\\frac{1}{4}\end{bmatrix}$$
- Everytime we multiply $r$ with $\boldsymbol{L}$, we get na updated value of $r$
$$r^{i+1} = Lr^i$$ 
- Do this till the values of $r$ stop changing. 
- This implies $\vec{r}$ is a eigenvector of $\boldsymbol{L}$ and has eigenvalue 1
- Multiplying $\vec{r}$ will $\boldsymbol{L}$ many times will be easier with the diagonalisation technique.


## Real world scenario
- There were be millions on pages on the real internet
- However, most of these pages will not be connected to each other i.e the link matrix $\boldsymbol{L}$ will mostly be filled be zeros. This matrix is called a _sparse matrix_


## Damping factor

- Additional term to the iterative formula
- Between 0 and 1
  - It is (1 - probabilty(someone will type in a URL instead of clicking a link))
- Tradeoff between speed and stability of convergence process in the iteration
$$r^{i+1} = d(Lr^i) + \frac{1-d}{n}\boldsymbol{J}$$
$$\boldsymbol{J} => \text{n x n  identity matrix}$$