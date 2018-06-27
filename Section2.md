# discrete probability crash course
## final set
U: final set (e.g. ![equation](https://latex.codecogs.com/gif.latex?%5Cbigcup%20%3D%7B%20%5Cleft%20%5C%7B%200%2C1%20%5Cright%20%5C%7D%7D%5E%7Bn%7D) ) all n length fo bits

def: **Probablility distribution** P over U is a funciton ![equation](https://latex.codecogs.com/gif.latex?P%3A%5Ccup%20%5Cto%20%5B0%2C1%5D) such that 
![equation](https://latex.codecogs.com/gif.latex?%5Csum_%7Bx%20%5Cin%20%5Ccup%20%7D%5E%7B%20%7D%20f%28x%29%20%3D1)

* uniform distribution for all ![equation](https://latex.codecogs.com/gif.latex?X%5Cin%5Ccup%3A%20P%28X%29%20%3D%201/%5Cleft%20%7C%20%5Ccup%20%5Cright%20%7C)

* point districution ![equation](https://latex.codecogs.com/gif.latex?P%28X_%7B0%7D%29%20%3D%201%2C%20%5Cforall%20x%5Cneq%20X_%7B0%7D%3A%20P%28x%29%3D0)

Distribution vector (P(x0), P(x1)..., P(xn)

## event
for a set ![equation](https://latex.codecogs.com/gif.latex?A%5Csubseteq%20%5Ccup%3A%20Pr%5BA%5D%20%3D%20%5Csum_%7BX%5Cin%20A%7D%20P%28x%29%20%5Cin%20%5B0%2C1%5D)
this set is called an event

## union bound
![equation](https://latex.codecogs.com/gif.latex?Pr%28A_%7B1%7D%20%5Ccup%20A_%7B2%7D%29%20%5Cleq%20Pr%5BA_%7B1%7D%5D%20&plus;%20Pr%5BA_%7B2%7D%5D)

![](https://latex.codecogs.com/gif.latex?Pr%28A_%7B1%7D%20%5Ccup%20A_%7B2%7D%29%20%3D%20Pr%5BA_%7B1%7D%5D%20&plus;%20Pr%5BA_%7B2%7D%5D%20-%20Pr%28A_%7B1%7D%20%5Ccap%20A_%7B2%7D%29)
