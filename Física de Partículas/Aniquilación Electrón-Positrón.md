Consideramos el proceso:

$$
e^{-} + e^{+} \rightarrow \gamma + \gamma
$$

Y denotamos $p_1, p_2$ a los $4$-momentos del electrón y el positrón respectivamente y $p_3, p_4$ a los $4$-momentos de los fotones que emergen del proceso. Considerando el marco de referencia en el centro de masa:

$$
p_1 = (E/c, \vec{p}) \qquad p_2 = (E/c, -\vec{p}) \qquad p_3 = (\hbar k_3, \hbar\vec{k}_3) \qquad p_4 = (\hbar k_4, \hbar\vec{k}_4)
$$

Hallamos el factor el factor de flujo. Notemos que:

$$
p_1 \cdot p_2 = \frac{E^2}{c^2} + |\vec{p}|^2 = m^2c^2 + 2|\vec{p}|^2
$$

$$
(p_1 \cdot p_2)^2 = m^4 c^4 + 4|\vec{p}|^2 m^2 c^2 + 4|\vec{p}|^4
$$

$$
(p_1 \cdot p_2)^2 - (m^2c^2)^2 = 4|\vec{p}|^2(|\vec{p}|^2 + (mc)^2) = 4|\vec{p}|^2  E^2 / c^2
$$

$$
F = 4\sqrt{(p_1 \cdot p_2)^2 - (m^2c^2)^2 } = 8 |\vec{p}| E/c
$$

La sección transversal del proceso puede hallarse como:

$$
\begin{aligned}
\sigma = \frac{\hbar^2 S}{F} \int \mathcal{M}^2 (2\pi)^4 \delta^4(p_1+p_2-p_3-p_4) \\
(2\pi) \frac{\delta(p_3^0 - |\vec{p}_3|)}{2|\vec{p}_3|} 
(2\pi) \frac{\delta(p_4^0 - |\vec{p}_4|)}{2|\vec{p}_4|} \frac{d^4p_3}{(2\pi)^4} \frac{d^4p_4}{(2\pi)^4}
\end{aligned}
$$

$$
\sigma = \frac{\hbar^2Sc}{8|\vec{p}|E} \left(\frac{1}{4\pi}\right)^2 \int \mathcal{M}  \frac{\delta(p^0_1+p^0_2-p^0_3-p^0_4) } {|\vec{p}_3| |\vec{p}_4|} \delta(\vec{p_3} + \vec{p_4}) dp^0_3  dp^0_4  d^3\vec{p}_3 d^3\vec{p}_4\\
$$

$$
\sigma = \left(\frac{1}{8\pi}\right)^2 \frac{\hbar^2 Sc}{2|\vec{p}|E} \int \mathcal{M}^2
  \frac{\delta(2E/c- 2|\vec{p}_3|) } {|\vec{p}_3|^2} d^3\vec{p_3}
$$

Nos interesa la sección transversal diferencial:

$$
\frac{d\sigma}{d\Omega}= \left(\frac{1}{8\pi}\right)^2 \frac{\hbar^2 Sc}{2|\vec{p}|E} \mathcal{M}^2 \int 
\frac{\delta(2E/c- 2|\vec{p}_3|) } {|\vec{p}_3|^2} |\vec{p}_3|^2 d\vec{p_3}
$$

Finalmente la sección transversal diferencial para este proceso será simplemente:

$$
\frac{d\sigma}{ d\Omega} = \left(\frac{\hbar c}{16\pi}\right)^2 \frac{\mathcal{M}^2}{2|\vec{p}|cE}
$$

Hallemos ahora la amplitud $\mathcal{M}$ usando el ritual de Feynman. Notemos que para el proceso $e^{-} + e^{+} \rightarrow \gamma + \gamma$ hay dos diagramas de Feynman de segundo orden. 

![](../assets/20250616184552.png)

Siguiendo el ritual de Feynman asociamos a los diagramas: 
	
- $4$-momentos $p_1$, $p_2$, $p_3$ y $p_4$ a las líneas externas y $q$ a la línea interna. 
	
- Estados $u^{(s_1)}$,  $\bar{v}^{(s_2)}$, $\epsilon^{*(s_3)}$ y $\epsilon^{*(s_4)}$.
	
- Constantes de acople $ig_e \gamma^{\mu}$ y $ig_e \gamma^{\nu}$ en donde $g_e$ es la constante de acoplamiento $g_e = \sqrt{4\pi \alpha}$.
	
- El propagador correspondiente a un fermión $i \frac{\gamma^{\mu} q_{\mu} + mc}{q^2 - (mc)^2}$.
	
- Términos asociados a la conservación del momento y energía $(2\pi)^4\delta^4(p_1 - q - p_3)$ y $(2\pi)^4\delta^4(p_2 + q - p_4)$ al primer diagrama y  $(2\pi)^4\delta^4(p_1 - q - p_4)$ y $(2\pi)^4\delta^4(p_2 + q - p_3)$ al segundo diagrama. 

Integramos hacia atrás partiendo del positrón que ingresa:

$$
\begin{aligned}
i(2\pi)^4 \delta(p_1+p_2-p_3-p_4) \mathcal{M}_1 = \int [\bar{v}^{(s_2)}(p_2)(ig_e \gamma^{\nu} )\epsilon_{\nu}^{*(s_4)}(p_4)] (2\pi)^4\delta(p_2+q-p_4) \\
i \frac{\gamma^{\mu} q_{\mu} + mc}{q^2 - (mc)^2} (2\pi)^4 \delta^4(p_1-q-p_3)
[\epsilon_{\mu}^{*(s_3)}(p_3) (ig_e\gamma^{\mu}) u^{(s_1)}(p_1)]
\end{aligned}
$$

$$
\mathcal{M_1} = \frac{-g_e^2}{(p_1 - p_3)^2-(mc)^2} \bar{v}(3) \cancel{\epsilon_4^*}(\cancel{p_1} - \cancel{p_3} + mc) \cancel{\epsilon_3^*} u(1)
$$

Por una parte notemos que podemos simplificar el denominador:

$$
(p_1 - p_3) ^2 - (mc)^2 = (p_1\cdot p_1) -(mc)^2 - 2(p_1\cdot p_3) + (p_3 \cdot p_3) = - 2(p_1\cdot p_3)
$$

Por otra parte la expresión dentro de los estados puede simplificarse como:

$$
(\cancel{p_1} - \cancel{p_3} + mc) \cancel{\epsilon_3^*} u(1) 
=  \cancel{\epsilon_3^*} (-\cancel{p_1} +\cancel{p_3} + mc) u(1) 
= \cancel{\epsilon_3^*} \cancel{p_3} u(1) 
$$

Escribimos entonces $\mathcal{M}_1$ y análogamente $\mathcal{M}_2$ como:

$$
\mathcal{M}_1 = \frac{g_e^2}{2(p_1\cdot p_3)} \bar{v}(2)  \cancel{\epsilon_4^*}  \cancel{\epsilon_3^*} \cancel{p_3} u(1) 
$$

$$
\mathcal{M}_2 = \frac{g_e^2}{2(p_1\cdot p_4)} \bar{v}(2)  \cancel{\epsilon_3^*}  \cancel{\epsilon_4^*} \cancel{p_4} u(1) 
$$

Finalmente la amplitud del proceso se puede escribir como:

$$
\mathcal{M} = \mathcal{M}_1 + \mathcal{M}_2 = \frac{g_e^2}{2}  \bar{v}(2)  
\left( \frac{
\cancel{\epsilon_4^*}  \cancel{\epsilon_3^*} \cancel{p_3}} {p_1\cdot p_3} +
\frac{
\cancel{\epsilon_3^*}  \cancel{\epsilon_4^*} \cancel{p_4}} {p_1\cdot p_4}
\right) u(1)
$$

Nos interesa sin embargo el valor esperado del modulo cuadrado de la amplitud. El modulo cuadrado de $\mathcal{M}$ será:

$$
|\mathcal{M}|^2 = \mathcal{M}_1 \mathcal{M}_1^* + \mathcal{M}_1 \mathcal{M}_2^* + \mathcal{M}_2 \mathcal{M}_1^* + \mathcal{M}_2 \mathcal{M}^*_2
$$

En donde:

$$
\begin{aligned}
\mathcal{M}_1^* =  \frac{g_e^2}{2(p_1\cdot p_3)} [\bar{v}(2)  \cancel{\epsilon_4^*}  \cancel{\epsilon_3^*} \cancel{p_3} u(1) ]^{*} \equiv ...  [\bar{v}(2) \Gamma_1 u(1) ]^{\dagger}
\\
= ... [v(2) ^{\dagger} \gamma^0  \cancel{\epsilon_4^*}  \cancel{\epsilon_3^*} \cancel{p_3} u(1) ]^{\dagger} 
= ... [u(1)^{\dagger} \gamma^0 \gamma^0 \cancel{p_3}  \cancel{\epsilon_3}  \cancel{\epsilon_4} \gamma^0 u(1) ] \\
= ...
[\bar{u}(1) \cancel{p_3} \cancel{\epsilon_3}  \cancel{\epsilon_4} v(2)] 
\equiv 
\frac{g_e^2}{2(p_1\cdot p_3)} \bar{u}(1) \bar{\Gamma}_1 v(2)
\end{aligned}
$$

Análogamente:

$$
\begin{aligned}
\mathcal{M}_2^* = \frac{g_e^2}{2(p_1\cdot p_4)} 
[\bar{u}(1) \cancel{\epsilon_3^*}  \cancel{\epsilon_4^*} \cancel{p_4} v(2)]^{*}
\equiv ... [\bar{v}(2) \Gamma_2 u(1)]^{\dagger} 
\\
= ...[\bar{u}(1) \cancel{p_4} \cancel{\epsilon_4} \cancel{\epsilon_3} v(2)]
\equiv \frac{g_e^2}{2(p_1\cdot p_4)}\bar{u}(1) \bar{\Gamma}_2 v(2)
\end{aligned}
$$

Luego:

$$
\langle \mathcal{M_1} \mathcal{M}_1^* \rangle = ...\text{Tr}[\Gamma_1(\cancel{p_1} + mc) \bar{\Gamma}_1 (\cancel{p_2} - mc)]
$$

$$
\langle \mathcal{M_1} \mathcal{M}_2^* \rangle =... \text{Tr}[\Gamma_1(\cancel{p_1} + mc) \bar{\Gamma}_2 (\cancel{p_2} - mc)]
$$

$$
\langle \mathcal{M_2} \mathcal{M}_1^* \rangle =... \text{Tr}[\Gamma_2(\cancel{p_1} + mc) \bar{\Gamma}_1 (\cancel{p_2} - mc)]
$$

$$
\langle \mathcal{M_2} \mathcal{M}_2^* \rangle =... \text{Tr}[\Gamma_2(\cancel{p_1} + mc) \bar{\Gamma}_2 (\cancel{p_2} - mc)]
$$

Reemplazando:

$$
\begin{aligned}
\langle|\mathcal{M}|^2\rangle = \frac{g_e^4}{4(p_1\cdot p_3)^2} \text{Tr}[\cancel{\epsilon_4^*} \cancel{\epsilon_3^*} \cancel{p}_3 (\cancel{p}_1+ mc)  \cancel{p_3} \cancel{\epsilon_3}  \cancel{\epsilon_4} (\cancel{p_2} - mc)] \\

\frac{g_e^4}{4(p_1\cdot p_3)(p_1\cdot p_4)} \text{Tr}[\cancel{\epsilon_4^*} \cancel{\epsilon_3^*} \cancel{p}_3 (\cancel{p}_1+ mc)  \cancel{p_4} \cancel{\epsilon_4}  \cancel{\epsilon_3} (\cancel{p_2} - mc)] \\

\frac{g_e^4}{4(p_1\cdot p_4)(p_1\cdot p_3)} \text{Tr}[\cancel{\epsilon_3^*} \cancel{\epsilon_4^*} \cancel{p}_4 (\cancel{p}_1+ mc)  \cancel{p_3} \cancel{\epsilon_3}  \cancel{\epsilon_4} (\cancel{p_2} - mc)] \\

\frac{g_e^4}{4(p_1\cdot p_4)^2} \text{Tr}[\cancel{\epsilon_3^*} \cancel{\epsilon_4^*} \cancel{p}_4 (\cancel{p}_1+ mc)  \cancel{p_4} \cancel{\epsilon_4}  \cancel{\epsilon_3} (\cancel{p_2} - mc)] \\

\end{aligned} 
$$


