# Exercise 6.1

According to the main text, a phase shift operator adds phase $-1$ on computational basis state $|x\rangle$ only when $x = x_0$, that is

$$
|x\rangle \to (-1)^{\delta_{x_0}}|x\rangle = \begin{cases}
-|x\rangle  & x \neq x_0\\
|x\rangle & x = x_0
\end{cases}
$$(eqn:6.1.1)

Consider operator $U = 2|x_0\rangle\langle x_0| - I$. When performing $U$ on arbitrary computational basis state $|x\rangle$, 

$$
U|x\rangle = 2|x_0\rangle\langle x_0|x\rangle - |x\rangle = \begin{cases}
 -|x\rangle & x \neq x_0\\
 |x\rangle & x = x_0
\end{cases}
$$(eqn:6.1.2)

Also, operator $U$ is unitary since

$$
\begin{split}
U =& (2|x_0\rangle\langle x_0| - I )^{\dagger}(2|x_0\rangle\langle x_0| - I ) \\
=& 4|x_0\rangle\langle x_0| - 2|x_0\rangle\langle x_0| - 2|0\rangle\langle 0| + I = I
\end{split}
$$(eqn:6.1.3)

Therefore, unitary operator $U$ corresponds to the phase shift in the Grover iteration. 

It is worth pointing out that basis state $|x\rangle$ can be written in either decimal form $\{|0\rangle, |1\rangle, |2\rangle, |3\rangle, \dotsc, |N\rangle\}$ where $N = 2^n$, or binary form $\{|0\rangle, |1\rangle\}^{\otimes n}$. The main text tells that $|x_0\rangle = |0\rangle$ (decimal form), then 

$$
U = 2|0\rangle\langle 0| - I
$$(eqn:6.1.4)

One can also write $|x_0\rangle = |0\rangle^{\otimes n}$ so 

$$
U = 2|0\rangle^{\otimes n}\langle 0|^{\otimes n} - I
$$(eqn:6.1.5)

which is equivalent with eq. {eq}`eqn:6.1.4`.