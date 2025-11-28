# Exercise 8.2

Consider a quantum measurement $\{M_m\}$ with outcome labeled by $m$, where $M_m$ is not a unitary operator. For a pure state $|\phi\rangle$, the probability of measuring outcome $m$ is $p(m) = \langle \phi|M^{\dagger}_mM_m|\phi\rangle$. Here, the expectation value of operator $M^{\dagger}_m M_m$ can be written as

$$
\langle \phi|M^{\dagger}_mM_m|\phi\rangle = {\rm tr}\left( M^{\dagger}_mM_m \rho_{\phi}\right) = p(m)
$$(eqn:6.2.1)

where $\rho_{\phi} = |\phi\rangle\langle \phi|$. The post-measurement state $|\phi'\rangle$ is given by

$$
|\phi'\rangle = \frac{M_m|\phi\rangle}{\sqrt{p(m)}} = \frac{M_m|\phi\rangle}{\sqrt{\langle \phi|M^{\dagger}_mM_m|\phi\rangle}}
$$(eqn:6.2.2)

which can be also written in the form of density matrix, 

$$
\rho'_{\phi} = |\phi'\rangle \langle \phi'|= \frac{M_m|\phi\rangle \langle \phi| M^{\dagger}_m}{p(m)} = \frac{M_m\rho_{\phi} M^{\dagger}_m}{{\rm tr}\left( M^{\dagger}_mM_m \rho_{\phi}\right)}
$$(eqn:6.2.3)


#### Probability of measurement

Suppose density matrix $\rho$ describes an ensemble of pure states $\{q(j), |\psi_j\rangle\}$, 

$$
\rho = \sum_j q(j)|\psi_j\rangle\langle \psi_j | = \sum_j q(j)\rho_j
$$(eqn:6.2.4)

where $\rho_j = |\psi_j\rangle\psi_j|$. The probability of outcome $m$ after measuring the ensemble is given by

$$
P(m) = \sum_j q(j) p(m|j) = \sum_j q(j) {\rm tr}\left( M^{\dagger}_mM_m \rho_{j}\right)
$$(eqn:6.2.5)

This is the product of probability of "getting pure state $|\psi_j\rangle$", or $q_j$, and the probability of "measuring $m$ for $|\psi_j\rangle$", or $p(m|j)$. Here, $p(m|j)$ is obtained from eq. {eq}`eqn:6.2.1`. One can also rewrite eq. {eq}`eqn:6.2.5` as

$$
\begin{split}
P(m) =& \sum_j q(j) {\rm tr}\left( M^{\dagger}_mM_m \rho_{j}\right) = \sum_j q(j) {\rm tr}\left(\rho_{j} M^{\dagger}_mM_m \right) \\
=&  {\rm tr}\left[\sum_j q(j)\rho_{j} M^{\dagger}_mM_m \right] \\
=& {\rm tr}\left(\rho M^{\dagger}_mM_m \right) = {\rm tr}\left(M_m\rho M^{\dagger}_m \right) = {\rm tr}\left(\mathcal{E}(\rho) \right) \\
\end{split} 
$$(eqn:6.2.6)

where $\mathcal{E}(\rho) = M_m\rho M^{\dagger}_m$. 

#### Post-measurement state

After measurement, the new ensemble is described by a new probability distribution and post-measurement states. From eq. {eq}`eqn:6.2.3`, the normalized post-measurement state $\rho'_j$ for each $|\psi_j\rangle$ is given by

$$
\rho'_{j} = \frac{M_m \rho_j M^{\dagger}_m}{{\rm tr}\left( M^{\dagger}_mM_m \rho_{\phi}\right)} = \frac{M_m\rho_{j} M^{\dagger}_m}{p(m|j)}
$$(eqn:6.2.7)

The probability of getting $\rho'_j$ is $q(j)p(m|j)$. However, $\{q(j)p(m|j)\}$ does not give a valid probability distribution since $\sum_j q(j)p(m|j) = P(m) $ is NOT EQUAL TO ONE in general. As a result, we re-normalize and get a new probability distribution for post-measurement ensemble as $\{q(j)p(m|j) / P(m)\}$. In this context, the density matrix that describes post-measurement ensemble is given by

$$
\begin{split}
 \rho' =& \sum_{j} \frac{q(j)p(m|j)}{P(m)} \rho'_{j}  \\
 =& \sum_{j} \frac{q(j)p(m|j)}{P(m)} \frac{M_m\rho_{j} M^{\dagger}_m}{p(m|j)} \\
 =& \sum_{j} \frac{q(j)M_m\rho_{j} M^{\dagger}_m}{P(m)} = \frac{M_m \rho M^{\dagger}_m}{P(m)}
\end{split}
$$(eqn:6.2.8)

which is equivalent with $\mathcal{E}_m (\rho) / {\rm tr}\left(\mathcal{E}(\rho) \right)$. 

<!-- $$
|x\rangle \to (-1)^{\delta_{x_0}}|x\rangle = \begin{cases}
-|x\rangle  & x \neq x_0\\
|x\rangle & x = x_0
\end{cases}
eq. {eq}`eqn:6.1.4`.
$$(eqn:6.1.1) -->
