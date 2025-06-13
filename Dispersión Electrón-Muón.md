El muón es una partícula elemental masiva similar al electrón, con la misma carga eléctrica de $-e$  y un espín de $1/2$, pero con una masa mucho mayor, unas $206.7682830(46)$ veces la del electrón.  Se clasifica como leptón y al igual que otros leptones, está no esta compuesto por ninguna partícula más simple. 

Sean $m$ la masa del electrón y $M$ la masa del muón.  Consideremos el experimento de dispersión de Mott ($m << M$):

$$ 
e^- + \mu^- \rightarrow e^- + \mu^-
$$

Denotamos $p_1$ y $p_3$ a los $4$-momentos inicial y final del electrón y $p_2$ y $p_4$ a los $4$-momentos inicial y final el muón. Considerando el marco de referencia en el muón e ignorando el impulso de este, podemos escribir:

$$
p_1 = (\frac{E_1}{c}, \vec{p}_1) \qquad p_2 = (Mc, 0) \qquad p_3 = (\frac{E_1}{c}, \vec{p}_3) \qquad p_4 = (Mc, 0)
$$

Hallamos ahora el factor de flujo. Para ello partimos del producto de los momentos iniciales y manipulamos la expresión para hallar el factor de flujo $F$:

$$
p_1 \cdot p_2 = \frac{E_1}{c} Mc = \sqrt{|\vec{p}_1|^2 + (mc)^2} Mc
$$

$$
(p_1 \cdot p_2)^2 = |\vec{p}_1|^2 M^2 c^2 + m^2 M^2 c^4
$$

$$
(p_1 \cdot p_2)^2 - (mMc^2)^2 = |\vec{p}_1|^2 M^2 c^2
$$

$$
F = 4\sqrt{(p_1 \cdot p_2)^2 - (mMc^2)^2} = 4M c  |\vec{p}_1|
$$

La sección transversal del proceso estará dada por:

$$
\begin{aligned}
\sigma = \frac{\hbar^2S}{F} \int |\mathcal{M}|^2 (2\pi)^4 \delta^4(p_1+p_2-p_3-p_4) 
\\
(2\pi) \big[ \delta(p_3^2 - m^2c^2) \theta(p_3^0) \big]
(2\pi) \big[ \delta(p_4^2 - M^2c^2) \theta(p_4^0) \big] \frac{d^4 p_3}{(2\pi)^4} \frac{d^4 p_4}{(2\pi)^4}
\end{aligned}
$$

$$
\begin{aligned}
\sigma = \frac{\hbar^2}{4M c  |\vec{p}_1|} \frac{1}{(2\pi)^2}
\int |\mathcal{M}|^2 \delta(p^0_1+p^0_2-p^0_3-p^0_4) \delta^3(\vec{p}_1 - \vec{p}_3) 
\\
\frac{\delta(p^0_3 - \sqrt{|\vec{p}_3|^2 + m^2c^2})}{2\sqrt{|\vec{p}_3|^2 + m^2c^2}} 
\frac{\delta(p^0_4 - Mc)}{2Mc} dp^0_3 d^3\vec{p}_3
\end{aligned}
$$

$$
\sigma = \left(\frac{\hbar}{8\pi}\right)^2 \frac{1}{Mc |\vec{p}_1|}
\int |\mathcal{M}|^2 \frac{\delta(E_1/c - \sqrt{|\vec{p}_3| + (mc)^2})}{\sqrt{|\vec{p}_3|^2 + m^2c^2} Mc} \delta^3(\vec{p}_1 - \vec{p}_3) d^3 \vec{p}_3
$$

Nos interesa la sección transversal diferencia $d\sigma / d\Omega$. Derivando ambos miembros:

$$
\frac{d \sigma}{d\Omega} = \left(\frac{\hbar}{8\pi} \frac{|\mathcal{M}|}{Mc} \right)^2  \frac{1}{ |\vec{p}_1| }
\int
\frac{\delta(E_1/c - \sqrt{p^2 + m^2c^2})}{\sqrt{p^2 + m^2c^2}} p^2 \delta(|\vec{p}_1| - p)dp
$$

Reemplazamos ahora:

$$
u \equiv \sqrt{p^2 + m^2c^2} \Rightarrow \frac{du}{dp} = \frac{p}{\sqrt{p^2+ m^2c^2}} = \frac{p}{u} \Rightarrow pudu = p^2dp
$$

$$
\frac{d \sigma}{d\Omega} = \left(\frac{\hbar}{8\pi} \frac{|\mathcal{M}|}{Mc} \right)^2 \frac{1}{ |\vec{p}_1| }
\int
\frac{\delta(E_1/c - u)}{u} |\vec{p}_1| u du 
$$

En donde el modulo del $4$-momento $p_1$ se cancela y la integral de la delta es simplemente uno. Finalmente la sección transversal diferencial para la dispersión de Mott electrón-muón será simplemente: 

$$
\frac{d \sigma}{d\Omega} = \left(\frac{\hbar}{8\pi} \frac{|\mathcal{M}|}{Mc} \right)^2 
$$

Hallemos ahora la amplitud $\mathcal{M}$ usando el ritual de Feynman. Notemos que para  el proceso $e^- + \mu^- \rightarrow e^- + \mu^-$ hay un solo diagrama de Feynman de orden dos:

![](images/20250612221751.png)

Asociamos al diagrama:
- $4$-momentos $p_1$, $p_2$, $p_3$ y $p_4$ a las líneas externas y $q$ a la línea interna. 
	
- Espinores $u^{(s_1)}$,  $\bar{u}^{(s_2)}$, $u^{(s_3)}$ y $\bar{u}^{(s_4)}$.
	
- Constantes de acople $ig_e \gamma^{\mu}$ y $ig_e \gamma^{\nu}$ en donde $g_e$ es la constante de acoplamiento $g_e = \sqrt{4\pi \alpha}$.
	
- El propagador correspondiente a un fotón $-ig_{\mu\nu}/ q^2$
	
- Términos asociados a la conservación del momento y energía $(2\pi)^4\delta^4(p_1 - q - p_3)$ y $(2\pi)^4\delta^4(p_2 + q - p_4)$.


Integramos hacia atrás partiendo del electrón que emerge:

$$\begin{aligned}
i(2\pi)^4 \delta^4(p_1+p_2-p_3-p_4) \mathcal{M} 
= 
\int \big[\bar{u}^{(s_3)}(p_3) (ig_e\gamma^{\mu}) u^{(s_1)}(p_1)\big] (2\pi)^4\delta^4(p_1 - q - p_3)
\\
(-\frac{ig_{\mu\nu}}{q^2}) (2\pi)^4\delta^4(p_2 + q - p_4) 
\big[ \bar{u}^{(s_4)}(p_4) (ig_e\gamma^{\nu}) u^{(s_2)}(p_2) \big]
\end{aligned}
$$

Finalmente se cancelan las deltas y la unidad imaginaria, luego la amplitud del proceso será:

$$
\mathcal{M} = -\frac{g_e^2}{(p_1 - p_3)^2}\big[\bar{u}^{(s_3)}(p_3) \gamma^{\mu} u^{(s_1)}(p_1)\big] \big[\bar{u}^{(s_4)}(p_4) \gamma_{\mu} u^{(s_2)}(p_2)\big] 
$$
