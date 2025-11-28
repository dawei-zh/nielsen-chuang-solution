# Extension of Section 2.1.8 - Trace

There are some missing part between eq. (2.60) and eq. (2.61) of the main text. For **pure state** $|\psi\rangle$, it can be written as a linear combination of an orthonormal basis $\{|j\rangle\}$, 

$$
|\psi\rangle = \sum_j c_j |\psi_j\rangle
$$

Then, the trace can be written under basis $\{|j\rangle\}$ as

$$
\begin{split}
{\rm tr}(A|\psi\rangle\langle \psi|) =& \sum_j \langle j|A|\psi\rangle\langle \psi|j\rangle \\
=& \sum_j \langle j|\psi\rangle^* \langle j|A|\psi\rangle \\
=& \sum_j c_j^*\langle j| A|\psi\rangle = \langle \psi|A|\psi\rangle.
\end{split}
$$

Mathematically, above relation is valid for **arbitrary square matrix $A$**. However, in quantum machanics, an **observable** $A$ should be a **Hermitian** matrix.