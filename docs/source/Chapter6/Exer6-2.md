# Exercise 6.2

Consider the operator $U = 2|\psi\rangle\langle\psi| - I$ where $|\psi\rangle$ is the equal superposition state

$$
|\psi\rangle = \frac{1}{N^{1/2}}\sum_{x=0}^{N-1}|x\rangle 
$$(eqn:6.2.1)

where $\{|x\rangle\}$ is computational basis set. The operator $U$ can be obtained by

$$
\begin{align}
2|\psi\rangle\langle\psi| - I &= \frac{2}{N}\left(\sum_{x=0}^{N-1}|x\rangle \right)\left(\sum_{x'=0}^{N-1}\langle x'|\right) - I \\
&= \frac{2}{N}\sum_{x, x'=0}^{N-1}|x\rangle \langle x'| - \sum_{x=0}^{N-1}|x\rangle \langle x|
\end{align}
$$(eqn:6.2.2)

Applying operator $U$ to an arbitrary state $\sum_k\alpha_k |k\rangle$ gives

$$
\begin{split}
(2|\psi\rangle\langle\psi| - I)\sum_k\alpha_k |k\rangle =& \frac{2}{N}\left(\sum_{x, x'=0}^{N-1}|x\rangle \langle x'|\right)\left(\sum_{k=0}^{N-1}\alpha_k |k\rangle \right) \\
&- \left(\sum_{x=0}^{N-1}|x\rangle \langle x|\right)\left(\sum_{k=0}^{N-1}\alpha_k |k\rangle \right) \\
=& \frac{2}{N}\sum_{x, x',k=0}^{N-1}\alpha_k|x\rangle \langle x'|k\rangle
-\sum_{x,k=0}^{N-1} \alpha_k |x\rangle \langle x|k\rangle \\
=&\frac{2}{N}\sum_{x, k=0}^{N-1}\alpha_k|x\rangle \langle k|k\rangle - \sum_{k=0}^{N-1}\alpha_k|k\rangle \langle k|k\rangle \\
=&\sum_{x=0}^{N-1}\left(\sum_{k=0}^{N-1}\frac{2}{N}\alpha_k\right)|x\rangle - \sum_{k=0}^{N-1}\alpha_k|k\rangle  \\
=&\sum_{x=0}^{N-1}2\langle \alpha\rangle|x\rangle - \sum_{k=0}^{N-1}\alpha_k|k\rangle
\end{split}
$$(eqn:6.2.3)

Note that change the index would not change the state, so we could re-write eq. {eq}`eqn:6.2.3` as 

$$
(2|\psi\rangle\langle\psi| - I)\sum_k\alpha_k |k\rangle  = \sum_{k=0}^{N-1}2\langle \alpha\rangle|k\rangle - \sum_{k=0}^{N-1}\alpha_k|k\rangle = \sum_{k=0}^{N-1}\left[2\langle \alpha\rangle-\alpha_k\right]|k\rangle
$$(eqn:6.2.4)