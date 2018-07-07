# RSA 

is created in 1976

![e](https://latex.codecogs.com/gif.latex?n%5Cleftarrow%20p.q) is easy. 

![e](https://latex.codecogs.com/gif.latex?p.q%20%5Cleftarrow%20n) is very difficult for large n


in RSA, derive public key e and private key d from p, q. User e,d,n for encryption and decryption. p and q is only used to generate e
and d

RSA is most widely implemented asymetric.

public key {e,n} ![e](https://latex.codecogs.com/gif.latex?c%20%3D%20m%5Ee%20%5Cmod%20n) for Encrytion

public key {d,n} ![e](https://latex.codecogs.com/gif.latex?m%20%3D%20c%5Ed%20%5Cmod%20n) for decrytion

m = m^ed mod n. this hold for carefully selected ed

## how to generated e, d from p, q

euler totient function is the number of postive integers that are btween 1 and n-1, inclusived and are relatively prime to n( thei biggest common divider is 1)
