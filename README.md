# Tesis

De la expresión para la matriz de transferencia correspondiente a un modelo de dispersor delta de Dirac y la propiedad multiplicativa se obtiene la matriz de transferencia de un sistema de n deltas de Dirac situadas cada una en la posición $x=a_m$ con $m=0,1,...,n$

$$M=K(-ka_n)N\left(\frac{\eta_n}{k}\right)K(kd_n)N\left(\frac{\eta_{n-1}}{k}\right)K(kd_{n-1})\cdots K(kd_1)N\left(\frac{\eta_0}{k}\right)K(kd_0)$$

donde $d_m=a_m-a_{m-1}$ y $d_0=a_0$.

Si se asume que $kd_m=2\pi z_m$ con $z_m\in \mathbb{Z}$ entonces $D(kd_m)=I$ y por tanto

$$M=N_nN_{n-1}\cdots N_{1}N_{0}$$

es decir

$$M=\begin{pmatrix}
        1-i\frac{\sum\eta_j}{2k} & -i\frac{\sum\eta_j}{2k}\\
        i\frac{\sum\eta_j}{2k} & 1+i\frac{\sum\eta_j}{2k}
  \end{pmatrix}.$$

Se pueden obtener dos casos extremos si se introduce desorden en el sistema.

Si $\{\eta_j\}$ son variables aleatorias i.i.d con distribución Normal $\mathcal{N}(0, \sigma_\eta)$ y $\{d_j\}$ son variables aleatorias i.i.d con distribución Normal $\mathcal{N}(\frac{2\pi}{k}, \sigma_d)$ entonces los casos límite serán 
* $\sigma_d \approx 0$. 
    Donde se puede realizar la aproximación $K(kd_j)\approx I$ y por lo tanto $\text{Im}[M_{12}]\approx \frac{1}{2k}\sum \eta_j$ de modo que es posible demostrar\footnote{Véase el apéndice D.} $\text{Im}[M_{12}]^2=\lambda \sim \frac{N\sigma_\eta^2}{4k^2} \cdot \chi_1^2$. Obteniéndose la función de densidad de probabilidad
  
$$\rho(\lambda)=\frac{2k}{\sqrt{2\pi N\sigma_\eta^2 \lambda}}e^{-\frac{4k\lambda}{2N\sigma_\eta^2}}, \quad \lambda>0.$$
    
* $\sigma_d \lessapprox 2\pi$. La desivación estandar es comparable con la media.
