# RAndom Circuit Block Encoded Matrix (RACBEM)  

This is a python module implementing RACBEM using IBM's Qiskit. It can used in various quantum linear algebra problems.



## Dependencies

+ Pyhton3.7
+ IBM Qiskit
+ QuTiP
+ numpy, scipy



## Introduction

This is an implementation of the a RAndom Circuit Block Encoded Matrix (RACBEM) and its Hermitian conjugate. It is then used to build a quantum singular value circuit using the method of quantum singular value transformation (QSVT).

Take a RAndom Circuit Block Encoded Matrix (RACBEM), this function uses a quantum signal processing circuit to evaluate the matrix inverse, using the method of quantum singular value transformation (QSVT). This implements a (non-Hermitian) block-encoding of a Hermitian matrix manually.



## References

+ Yulong Dong, Lin Lin. Random circuit block-encoded matrix and a proposal of quantum LINPACK benchmark
+ [Y. Dong, X. Meng, K. B. Whaley, and L. Lin. Efficient Phase Factor Evaluation in Quantum Signal Processing. arXiv: 2002.11649](https://arxiv.org/abs/2002.11649)
+ [A. Gilyén, Y. Su, G. H. Low, and N. Wiebe. Quantum singular value transformation and beyond: exponential improvements for quantum matrix arithmetics. In Proceedings of the 51st Annual ACM SIGACT Symposium on Theory of Computing, pages 193–204, 2019](https://dl.acm.org/doi/10.1145/3313276.3316366)



## Citing our work

If you find our work useful or you use our work in your own project, please consider to cite our work.



## The Authors

We hope that the package is useful for your application. If you have any bug reports or comments, please feel free to email one of the software authors:

* Yulong Dong, dongyl@berkeley.edu

* Lin Lin, linlin@math.berkeley.edu

  

## Running the demo

`>> python main_test.py`

The output should be like the follows.

```
kappa=5, sigma=1.00, polynomial approximation error=1.902e-02

Generic Block-Encoding
singular value (A) = 
 [0.99  0.979 0.952 0.79  0.694 0.306 0.248 0.204]
Job Status: job has successfully run
succ prob (exact)     =  0.22205160210017913
succ prob (noiseless) =  0.23183536309935282
succ prob (measure)   =  0.2242431640625

Hermitian Block-Encoding
singular value (A) = 
 [0.963 0.91  0.908 0.802 0.397 0.292 0.289 0.236]
condition number (A)  = 4.074
||A - A^\dagger||_2   = 2.675e-15
```

