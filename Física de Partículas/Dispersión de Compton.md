El efecto Compton (o dispersión Compton) consiste en el aumento de la longitud de onda de un fotón cuando choca con un electrón libre y pierde parte de su energía. 

Este proceso puede escribirse como $e^- + \gamma \rightarrow e^- + \gamma$.  Escribamos sus $4$-momentos desde un marco de referencia para el cual la $3$-velocidad inicial del electrón es nula y en el cual el fotón viaja sobre el eje $z$.

$$
p_1 = (mc, \vec0) \quad p_2 = (\hbar \omega /c, \hbar \vec{k}) \quad p_3 =(E/c, \vec p) \quad p_4 = (\hbar \omega'/c, \hbar \vec k')
$$

Como el fotón no tiene masa, el factor de flujo se reduce a $4(p_1\cdot p_2) = 4m_ec \hbar\omega$ . Luego la sección transversal será:

$$ 
\begin{aligned}
\sigma = \frac{\hbar^2 S}{4mc \hbar\omega}\int(2\pi)^4|\mathcal{M}|^2 \delta^4(p_1+p_2-p_3-p_4) \\
\times 2 \pi \delta(p_3^2 - m_e^2c^2)\theta(p^0_3) 2 \pi \delta(p_4^2)\theta(p^0_4) \frac{d^4p_3}{(2\pi)^4} \frac{d^4p_4}{(2\pi)^4}
\end{aligned}
$$

$$ 
\begin{aligned}
\sigma = \frac{\hbar^2 S}{4\hbar\omega m} \frac{1}{(2\pi)^2} \int |\mathcal{M}^2| \delta(mc + \hbar|\vec{k}| - p_3^0 -p_4^0) \delta^3(\hbar \vec{k} - \vec{p}_4 - \vec{p_3}) \\
\times \frac{\delta(p^0_3-\sqrt{|\vec{p_3}|^2+m^2c^2})}{2\sqrt{|\vec{p_3}|^2+m^2c^2}} \frac{\delta(p_4^0- |\vec{p}_4|)}{2|\vec{p}_4|} d^4p_3 d^4p_4
\end{aligned}
$$

$$
\sigma = \left(\frac{\hbar}{8\pi} \right)^2 \frac{S}{\hbar m\omega} \int 
|\mathcal{M}|^2 \frac
{\delta(mc + \hbar|\vec{k}| - \sqrt{|\vec{p_3}|^2+(mc)^2} + |\vec{p_4}|)}
{\sqrt{|\vec{p_3}|^2 + (mc)^2} |\vec{p}_4|} \delta(\vec{p}_3 + \vec{p}_4 - \hbar\vec{k}) d^3 \vec{p}_3 d^3 \vec{p_4}
$$

Analicemos la delta de Dirac restante. Sea $\theta$ el ángulo entre el fotón incidente y el dispersado. Notemos que podemos escribir $\vec{p}_4$ como:

$$
\vec{p_3} = \hbar \vec{k} - \vec{p}_4 \Rightarrow |\vec{p}_3
| = \sqrt{(\hbar|\vec{k}|)^2 + |\vec{p}_4| - 2 \hbar|\vec{k}||\vec{p}_4| \cos \theta }$$

$$
\Rightarrow \sqrt{|\vec{p}_3|^2 + (mc)^2} = \sqrt{(\hbar|\vec{k}|)^2 + |\vec{p}_4| - 2 \hbar|\vec{k}||\vec{p}_4| \cos \theta + (mc)^2} 
$$

Tomando $u = \sqrt{|\vec{p}_3|^2+(mc)^2} + |\vec{p}_4|$ y reemplazando lo anterior:

$$
u = \sqrt{(\hbar|\vec{k}|)^2 + |\vec{p}_4|^2 - 2 \hbar|\vec{k}||\vec{p}_4| \cos \theta + (mc)^2} + |\vec{p}_4|
$$

$$
\frac{du}{d|\vec{p_4}|} = \frac{|\vec{p}_4| - \hbar{\vec{k} \cos \theta}}{u - |\vec{p}_4|} + 1 =  \frac{u - \hbar{\vec{k} \cos \theta}}{u - |\vec{p}_4|} 
$$

Integrando sobre $\vec{p}_3$ y derivando sobre el ángulo solido $\Omega$, la integral queda solo en términos del modulo $|\vec{p}_4|$. Reemplazando $u$ en la integral: 

$$
\frac{d\sigma}{d\Omega} = \left(\frac{\hbar}{8\pi}\right)^2 \frac{S}{\hbar\omega m} |\mathcal{M}|^2 
\int_0^{\infty} \frac{\delta(mc + \hbar|\vec{k}| - u)}{(u-|\vec{p}_4|)|\vec{p}_4|} |\vec{p}_4|^2 d|\vec{p}_4|
$$

Haciendo el cambio de variable:

$$ 
\frac{d\sigma}{d\Omega} = \left(\frac{\hbar}{8\pi}\right)^2 \frac{S}{\hbar\omega m} |\mathcal{M}|^2 \int_0^{\infty} \frac{\delta(mc + \hbar|\vec{k}| - u)}{ u - \hbar |\vec{k}| \cos\theta} |\vec{p}_4|^2 du
$$

Al integrar la delta Dirac nos genera la siguiente igualdad. 

$$ 
u = mc + \hbar|\vec{k}| = \sqrt{(\hbar|\vec{k}|)^2 + |\vec{p}_4|^2 - 2 \hbar|\vec{k}||\vec{p}_4| \cos \theta + (mc)^2} + |\vec{p}_4|
$$

$$
(mc + \hbar|\vec{k}| - |\vec{p}_4|)^2 = (\hbar|\vec{k}|)^2 + |\vec{p}_4|^2 - 2\hbar|\vec{k}| |\vec{p_4}| \cos \theta + (mc)^2
$$

$$
mc \hbar|\vec{k}| - mc |\vec{p}_4| - \hbar|\vec{k}| |\vec{p}_4|= -\hbar|\vec{k}| |\vec{p}_4| \cos \theta
$$

$$
mc\hbar|\vec{k}| = |\vec{p}_4|(mc+\hbar|\vec{k}|-\hbar|\vec{k}|\cos\theta)
$$

$$
|\vec{p}_4| = \frac{mc\hbar|\vec{k}|}{mc+\hbar|\vec{k}|(1-\cos\theta)} = \frac{mc\hbar |\vec{k}|}{u - \hbar|\vec{k}|\cos \theta}
$$

Podemos finalmente reemplazara en la sección eficaz diferencial este valor de $|\vec{p}_4|$, y $S = 1$ y obtenemos:

$$ 
\frac{d\sigma}{d\Omega} = \left(\frac{\hbar}{8\pi}\right)^2 \frac{S}{\hbar\omega m} |\mathcal{M}|^2 \int_0^{\infty} \frac{\delta(mc + \hbar|\vec{k}| - u)}{(u - \hbar |\vec{k}| \cos\theta)^2}  mc\hbar|\vec{k}| du
$$

Integrando sobre $u$ la sección transversal diferencial será:

$$
\frac{d\sigma}{d\Omega} = \left(\frac{\hbar c}{8\pi}\right)^2 \frac{|\mathcal{M}|^2} {[mc^2 + \hbar \omega(1-\cos\theta)]^2} 
$$

![Efecto Compton](../assets/20250226010357.png)