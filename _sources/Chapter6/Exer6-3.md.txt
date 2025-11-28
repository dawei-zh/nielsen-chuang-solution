# Exercise 6.3

Consider two orthonormal states $|\alpha\rangle$ and $|\beta\rangle$ defined as

$$
\begin{split}
|\alpha\rangle &= \frac{1}{\sqrt{N-M}}\sum_{x}'' |x\rangle \\
|\beta\rangle &= \frac{1}{\sqrt{M}}\sum_{x}' |x\rangle \\
\end{split}
$$(eqn:6.3.1)

The equal superposition state can be rewritten under the basis $\{|\alpha\rangle, |\beta\rangle\}$, 

$$
|\psi\rangle = \frac{1}{\sqrt{N}}\sum_{x=0}^{N-1}|x\rangle  = \sqrt{\frac{N-M}{N}}|\alpha\rangle + \sqrt{\frac{M}{N}}|\beta\rangle 
$$(eqn:6.3.2)

Let

$$
\cos\frac{\theta}{2} =\sqrt{\frac{N-M}{N}}, \sin\frac{\theta}{2} =\sqrt{\frac{M}{N}}
$$(eqn:6.3.3)

such that 

$$
\sin\theta =2\cos\frac{\theta}{2} \sin\frac{\theta}{2} =\frac{2\sqrt{M(N-M)}}{N}
$$(eqn:6.3.4)

Using eq. {eq}`eqn:6.3.3`, eq. {eq}`eqn:6.3.2` becomes

$$
|\psi\rangle = \cos\frac{\theta}{2} |\alpha\rangle + \sin\frac{\theta}{2} |\beta\rangle
$$(eqn:6.3.5)

The main text tells a Grover iteration takes $|\psi\rangle$ to 

$$
G|\psi\rangle = \cos\frac{3\theta}{2}|\alpha \rangle + \sin\frac{3\theta}{2}|\beta\rangle
$$(eqn:6.3.6)

Using trigonometry identities to rewrite $\cos({3\theta}/{2})$ and $\sin({3\theta}/{2})$, $G|\psi\rangle$ becomes 

$$
\begin{split}
G|\psi\rangle =& \left(\cos\theta \cos\frac{\theta}{2} - \sin\theta\sin\frac{\theta}{2}\right)|\alpha \rangle \\
&+ \left(\sin\theta \cos\frac{\theta}{2} + \cos\theta\sin\frac{\theta}{2}\right)|\beta\rangle 
\end{split}
$$(eqn:6.3.7)

Above equation can also be re-written into below matrix form under basis $\{|\alpha\rangle, |\beta\rangle\}$,

$$
G|\psi\rangle = \begin{pmatrix}
\cos\theta \cos\frac{\theta}{2} - \sin\theta\sin\frac{\theta}{2} \\
\sin\theta \cos\frac{\theta}{2} + \cos\theta\sin\frac{\theta}{2}
\end{pmatrix} = \begin{pmatrix}
\cos\theta & -\sin\theta \\
\sin\theta & \cos\theta
\end{pmatrix}\begin{pmatrix}
\cos\frac{\theta}{2} \\ \sin\frac{\theta}{2} 
\end{pmatrix}
$$(eqn:6.3.8)

Therefore, we may write the Grover iteration under basis $\{|\alpha\rangle, |\beta\rangle\}$ as

$$
G|\psi\rangle = \begin{pmatrix}
\cos\theta & -\sin\theta \\
\sin\theta & \cos\theta
\end{pmatrix}
$$(eqn:6.3.9)