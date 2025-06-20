
Si bien el enlace covalente en moléculas diferentes al $\text{H}_2$, tanto diatómicas como poliatómicas es mas complicado, es posible estudiarlo gracias a que cualquier alteración en la estructura electrónica de un átomo debido a la proximidad de otro esta limitada a la capa externa. 

Para estudiar la estructura molecular se puede recurrir al *método de los orbitales moleculares* que describiremos a continuación. En lugar de comenzar con átomos definidos partimos de una configuración en la que los núcleos se encuentran en sus respectivas posiciones de equilibrio y se analiza el efecto de ir agregando los electrones a estos.

Así como los electrones de un átomo tienen orbitales definidos por los números cuánticos $n, l, m$ y ocupan los niveles de energía mas bajos de acuerdo a las reglas de Hund, las moléculas tienen *orbitales moleculares* y números cuánticos definidos. 

Los estados electrónicos moleculares pueden ser expresados como combinaciones lineales de orbitales moleculares, luego para determinar su configuración electrónica, se puede asignar cada electrón a un orbital molecular

Podemos expresar el estado electrónico $\ket{\psi_e}$ de una molécula en términos de sus orbitales moleculares $\ket{\psi}$:

$$ 
\ket{\psi_e} = \sum_r \psi_r \ket{\psi_r}
$$

Los cuales a su vez se pueden escribir como una combinación de orbitales atómicos $\ket{\phi}$, es decir: 

$$
\quad \ket{\psi_r} = \sum_{i}\phi_{ri} \ket{\phi_{ri}} 
$$

Luego, los orbitales moleculares se llenan con electrones, teniendo en cuenta el principio de exclusión de Pauli.  Volvamos al caso del ion de hidrogeno, habíamos encontrado que podíamos aproximar sus orbitales como:

$$
\ket{\psi_+} \sim \ket{\phi_a} + \ket{\phi_b} \qquad \ket{\psi_-} \sim \ket{\phi_a} - \ket{\phi_b}
$$

En el átomo de hidrogeno, los electrones tienen un momento angular orbital $\vec{L}$ y sus funciones son autoestados de los operadores $\hat{L}^2$ y $\hat{L}_z$. Debido a la simetría cilíndrica de la molécula, se puede afirmar que la función de onda $\ket{\psi_{+}}$ sigue siendo auto-estado del operador $\hat{L}_z$ ya que esta es una combinación lineal de los orbitales atómicos del átomo de hidrogeno. 

Dada entonces las auto-energías $\hbar m$ del operador $\hat{L}_z$, con $m = 0, \pm 1, \pm 2 ...$ denotamos los orbitales de sus correspondientes auto-estados como $\sigma, \pi, \delta,...$. Llenando entonces el orbital $\sigma_{1s}$ del ion $\text{H}_2^+$ se obtiene su estado fundamental. 

Se puede generalizar este esquema para tratar la molécula de $\text{H}_2$. A partir de los orbitales moleculares construidos para el $\text{H}_2^+$ se pueden construir dos esquemas:

![Orbitales del hidrogeno](../assets/20250318060913.png)

El primero corresponde a dos electrones en estado ligante $\sigma_{1s}$ y el segundo a electrones en estado anti-ligante $\sigma^*_{1s}$ y corresponde a un *orbital de anti-enlace*. En el primer caso, cada electrón, podemos escribir su función de onda como:

$$ 
\ket{\psi^{(1)}} \sim c_1\ket{\phi^{(1)}_a} + c_2\ket{\phi^{(1)}_b} \qquad 
\ket{\psi^{(2)}} \sim c_1\ket{\phi^{(2)}_a} + c_2\ket{\phi^{(2)}_b}
$$

Luego la función de onda electronica de la molécula será:

$$ 
\ket{\psi_e} \sim c_1^2 \ket{\phi_a, \phi_a} + c_2^2 \ket{\phi_b, \phi_b} + c_1c_2(\ket{\phi_a, \phi_b} + \ket{\phi_b, \phi_a})
$$

Si se compara con la función de onda obtenida bajo la aproximación de Heitler-London:

$$
\ket{\psi_S} \sim \ket{\phi_a, \phi_b} + \ket{\phi_b, \phi_a}
$$

Vemos que esta ultima desprecia los términos iónicos $\ket{\phi_a, \phi_a}$ y $\ket{\phi_b, \phi_b}$ para los cuales los electrones se encuentran ambos en las proximidades de uno u otro núcleo. En la practica la aproximación de Heitler-London tiende a subestimar el peso de la interacción iónica, mientras que el método de los orbitales moleculares tiende a sobreestimarlo. 

### Ejemplo: Molécula de $\text{LiF}$

Veamos un ejemplo. La función de onda que describe el orbital ligante de la molécula de $\text{LiF}$ puede expresarse de la siguiente forma:

$$ 
\ket{\psi} = [\frac{A}{\sqrt{2}}(\ket{\phi_{2s}, \phi_{2p_z}} + \ket{\phi_{2p_z} ,\phi_{2s}})+ B\ket{\phi_{2s},\phi_{2s}} + C\ket{\phi_{2_{p_z}},\phi_{2_{p_z}}}] \ket{\chi_S}
$$

En donde los orbitales atómicos $\phi_{2s}$ y $\phi_{2p_z}$ corresponden a los átomos $\text{Li}$ y $\text{F}$, respectivamente. Verifiquemos que $\ket{\psi}$ esta normalizada si $A^2 + B^2 + C^2 = 1$. Escribamos los orbitales atómicos que intervienen en la función de onda propuesta.  

$$
\begin{aligned} 
\langle \psi \ket {\psi} = \frac{A^2}{2} [2 \langle \phi_{1s},\phi_{2p_z}\ket{\phi_{1s},\phi_{2p_z}} + 2\langle \phi_{2p_z},\phi_{1s}\ket{\phi_{1s},\phi_{2p_z}}]
\\ \\
+ B^2 \langle{\phi_{2s},\phi_{2s}} \ket{\phi_{2s},\phi_{2s}} 
+ C^2 \langle \phi_{2_{p_z}},\phi_{2_{p_z}} \ket{\phi_{2_{p_z}},\phi_{2_{p_z}}} 
\\ \\
+ \frac{AB}{\sqrt{2}} \langle \phi_{1s},\phi_{2p_z}\ket{\phi_{2s},\phi_{2s}} 
+ \frac{AB}{\sqrt{2}} \langle \phi_{2p_z},\phi_{1s}\ket{\phi_{2s},\phi_{2s}}
\\ \\
+ \frac{AC}{\sqrt{2}} \langle \phi_{1s},\phi_{2p_z}\ket{\phi_{2p_z},\phi_{2p_z}} 
+ \frac{AC}{\sqrt{2}} \langle \phi_{2p_z},\phi_{1s}\ket{\phi_{2p_z},\phi_{2p_z}} 
\\ \\
+ BC \langle{\phi_{2_{p_z}}, \phi_{2_{p_z}}} \ket{\phi_{2s},\phi_{2s}} + CB \langle \phi_{2s},\phi_{2s} \ket{\phi_{2_{p_z}}, \phi_{2_{p_z}}}
\end{aligned} 

$$

En donde los orbitales atómicos se pueden escribir como:

$$
\phi_{1s}(\vec{r}) = R_{10}(r)Y_0^0 = \frac{1}{\sqrt{\pi a_0^3}} e^{-r/a_0}
$$

$$ 
\phi_{2s}(\vec{r}) = R_{20}(r) Y_0^0(\theta, \phi) =  \frac{1}{\sqrt{\pi}}\left( \frac{1}{2a_0} \right)^{3/2} \left(1 - \frac{r}{2a_0}\right) e^{-r/2a_0}
$$

$$ 
\phi_{2p_z}(\vec{r}) = R_{21}(r) Y_1^0(\theta, \phi) = \sqrt{\frac{1}{4\pi}} \left( \frac{1}{3a_0} \right)^{3/2} \frac{r}{a_0} e^{-r/2a_0} \cos\theta
$$

En la expresión de $\ket{\psi}$ podemos ver que hay términos cruzados que contienen un solo orbital $\phi_{p_z}$ y se anulan ya que van como $\sim \int \cos \theta d\Omega = 0$ de modo que:

$$ 
\langle\psi\ket{\psi} = A^2 \langle \phi_{1s},\phi_{2p_z}\ket{\phi_{1s},\phi_{2p_z}} +  
B^2 \langle{\phi_{2s},\phi_{2s}} \ket{\phi_{2s},\phi_{2s}} +C^2 \langle \phi_{2_{p_z}},\phi_{2_{p_z}} \ket{\phi_{2_{p_z}},\phi_{2_{p_z}}}
$$

Como los orbitales atómicos del átomo de hidrogeno son ortogonales vemos que:

$$ 
|\psi(\vec{r})|^2 = A^2 + B^2+C^2 = 1
$$

Y la función de onda esta normalizada cuando $A^2 + B^2+C^2 = 1$. El primer termino en la función de onda propuesta es la contribución covalente, que involucra al electrón externo del $\text{Li}$ y un electrón en el orbital correspondiente a $p_z$ de la capa externa del $\text{F}$. 

Se sabe que el término proporcional $B$ es muy pequeño comparado con la otra contribución iónica, es decir el término proporcional a $C$. Debido a que la probabilidad de que los dos electrones se encuentren en las proximidades del átomo de litio es muy baja. Esto se debe a la baja afinidad electrónica del $\text{Li}$, mientras que la energía de ionización del $\text{F}$ es alta, por lo que se puede asumir $B \approx 0$. En esta aproximación el momento dipolar de la molécula es $p = C^2 e R_0$ en donde $R_0$ es la separación de equilibrio entre los átomos.

Un valor experimental medido del momento dipolar $p$ de la molécula de $\text{LiF}$ es $p=0.85eR$ siendo $R$ la separación de equilibrio entre el $\text{Li}$ y el $\text{F}$. Entonces $C \approx 0.9$ y $A \approx 0.4$. Luego el carácter iónico de la molécula de $\text{LiF}$ es predominante, con una pequeña contribución covalente y podemos escribir su función de onda electronica como:

$$ 
\ket{\psi} \approx  [0.113(\ket{\phi_{2s}, \phi_{2p_z}} + \ket{\phi_{2p_z} ,\phi_{2s}}) + 0.9\ket{\phi_{2_{p_z}},\phi_{2_{p_z}}}] \ket{\chi_S}
$$

La cual esta normalizada ya que $0.4^2 + 0.9^2 \approx 1$.