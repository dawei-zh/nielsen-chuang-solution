# Exercise 6.6

<!-- eq. {eq}`eqn:6.3.2`    (eqn:6.3.1)-->

Gates in the dotted box in the second figure of Box 6.1 are given by

$$
U = (X\otimes X)(I\otimes H) {\rm CNOT} (I\otimes H)(X\otimes X)
$$

Here, the middle part is equivalent with a controlled-$Z$ gate, 

$$
(I\otimes H) (|0\rangle\langle 0| \otimes I + |1\rangle\langle 1| \otimes X) (I\otimes H) = |0\rangle\langle 0| \otimes I + |1\rangle\langle 1| \otimes Z 
$$

where $HXH = Z$. Then, operator $U$ can be written as

$$
\begin{split}
U=&(X\otimes X)(|0\rangle\langle 0| \otimes I + |1\rangle\langle 1| \otimes Z )(X\otimes X) \\
=& X|0\rangle\langle 0|X \otimes I + X|1\rangle\langle 1|X \otimes XZX \\
=& |1\rangle\langle 1| \otimes I - |0\rangle\langle 0| \otimes Z
\end{split}
$$

Adopting $I = |0\rangle\langle 0| + |1\rangle\langle 1|$ and $Z = |0\rangle\langle 0| - |1\rangle\langle 1|$, above equation becomes

$$
\begin{split}
U =& |1\rangle\langle 1| \otimes (|0\rangle\langle 0| + |1\rangle\langle 1|) - |0\rangle\langle 0| \otimes (|0\rangle\langle 0| - |1\rangle\langle 1|) \\
=& |10\rangle\langle 10| + |11\rangle\langle 11| - |00\rangle\langle 00| + |01\rangle\langle 01| \\
=& -2|00\rangle\langle 00| + |10\rangle\langle 10| + |11\rangle\langle 11| + |00\rangle\langle 00| + |01\rangle\langle 01| \\
=& -(2|00\rangle\langle 00| - \mathbb{I})
\end{split}
$$

where $\mathbb{I} = |10\rangle\langle 10| + |11\rangle\langle 11| + |00\rangle\langle 00| + |01\rangle\langle 01|$ is identity for two qubits. Therefore, operator in eq. {eq}`eqn:6.3.2` performs conditional phase shift operation $2|00\rangle\langle 00| − I$ up to a global phase of $-1$. 