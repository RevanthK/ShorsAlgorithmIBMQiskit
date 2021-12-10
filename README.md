# Shor's Quantum Integer Factorization Algorithm on IBM Qiskit

Many modern encryption algorithms (including RSA) rely on the assumption that factoring large integers is computationally intractable. This is true to classical computers, but the  Shor's algorithm shows that factoring integers is efficient on a quantum computer, so it may be feasible to defeat RSA by constructing a large quantum computer. I have implemented a Shor's algorithm using [IBM's Qiskit](https://qiskit.org/) and have ran experiments on small quantum computers.

## Introduction: Integer Factorization
Integer Factorization consists of decomposing of a composite number into a product of
smaller integers. Those integers may be further decomposed and so on. Decomposing an integer
into its prime integers is defined as its prime factorization. So, given a number N, a prime
factorization algorithm should find all its prime factors.
Testing whether the integer is prime can be done in polynomial time, such as through an AKS
primality test. However, classical techniques for finding the prime factorization of integers,
include the Rational Sieve method, are not efficient. Even state-of-the-art algorithms take
exponential time to find the factors of an integer. This means that with sufficiently large integers,
it would near impossible to solve despite immense computational power. The presumed
difficulty of this problem is the basis for widely used algorithms in cryptography such as RSA
encryption.
In 1994, Peter Shor theorized a polynomial-time quantum computing algorithm for integer
factorization. Shor's algorithm exploits both classical and quantum (period-finding)
computation. However, the predominant optimization of Shor's algorithm is due to the efficiency
of the quantum Fourier transform, and modular exponentiation by repeated squarings. This
result in sub-exponential runtime for the algorithm makes it exponentially faster than the most
efficient known classical factoring algorithm.

...

To see my full experiment please see here: https://github.com/RevanthK/ShorsAlgorithmIBMQiskit/blob/master/Final_Report.pdf 

I have also attached the [jupyter notebooks](https://github.com/RevanthK/ShorsAlgorithmIBMQiskit/blob/master/Shor's%20Algorithm.ipynb) used to run the experiments.
