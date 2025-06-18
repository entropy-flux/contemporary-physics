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

Donde usamos que $(\cancel{p}_1 - mc) u(1) = 0$, pues $u(1)$ es una espinor de solución de la ecuación de Dirac. Por tanto, podemos reescribir las amplitud $\mathcal{M}_1$ y $\mathcal{M}_2$ como:

$$
\mathcal{M}_1 = \frac{g_e^2}{2(p_1\cdot p_3)} \bar{v}(2)  \cancel{\epsilon_4^*}  \cancel{\epsilon_3^*} \cancel{p_3} u(1) 
\qquad
\mathcal{M}_2 = \frac{g_e^2}{2(p_1\cdot p_4)} \bar{v}(2)  \cancel{\epsilon_3^*}  \cancel{\epsilon_4^*} \cancel{p_4} u(1) 
$$

La amplitud total es simplemente la suma de ambas contribuciones:

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
 
En donde el conjugado $\mathcal{M}_1^*$ puede expresarse como: 

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

En donde $\Gamma = \cancel{\epsilon_4^*}  \cancel{\epsilon_3^*} \cancel{p_3}$ y $\bar{\Gamma} = \cancel{p_3} \cancel{\epsilon_3}  \cancel{\epsilon_4}$. Por otra parte el conjugado $\mathcal{M}_2^*$ puede expresarse de la misma forma:
 
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

Promediando sobre espines iniciales usando el truco de Casimir obtenemos las siguiente expresiones para los términos de $\mathcal{M}$:

$$
\begin{aligned}
\langle \mathcal{M_1} \mathcal{M}_1^* \rangle = ...\text{Tr}[\Gamma_1(\cancel{p_1} + mc) \bar{\Gamma}_1 (\cancel{p_2} - mc)] \\
\\
\langle \mathcal{M_2} \mathcal{M}_1^* \rangle =... \text{Tr}[\Gamma_2(\cancel{p_1} + mc) \bar{\Gamma}_1 (\cancel{p_2} - mc)] \\
\\
\langle \mathcal{M_1} \mathcal{M}_2^* \rangle =... \text{Tr}[\Gamma_1(\cancel{p_1} + mc) \bar{\Gamma}_2 (\cancel{p_2} - mc)] \\ 
\\
\langle \mathcal{M_2} \mathcal{M}_2^* \rangle =... \text{Tr}[\Gamma_2(\cancel{p_1} + mc) \bar{\Gamma}_2 (\cancel{p_2} - mc)]
\end{aligned}
$$

Reemplazando:

$$
\begin{aligned}
\langle|\mathcal{M}|^2\rangle = \frac{g_e^4}{4(p_1\cdot p_3)^2} \text{Tr}[\cancel{\epsilon_4^*} \cancel{\epsilon_3^*} \cancel{p}_3 (\cancel{p_1}+ mc)  \cancel{p_3} \cancel{\epsilon_3}  \cancel{\epsilon_4} (\cancel{p_2} - mc)] \\
\\
\frac{g_e^4}{4(p_1\cdot p_4)(p_1\cdot p_3)} \text{Tr}[\cancel{\epsilon_3^*} \cancel{\epsilon_4^*} \cancel{p_4} (\cancel{p_1}+ mc)  \cancel{p_3} \cancel{\epsilon_3}  \cancel{\epsilon_4} (\cancel{p_2} - mc)] \\
\\
\frac{g_e^4}{4(p_1\cdot p_3)(p_1\cdot p_4)} \text{Tr}[\cancel{\epsilon_4^*} \cancel{\epsilon_3^*} \cancel{p_3} (\cancel{p_1}+ mc)  \cancel{p_4} \cancel{\epsilon_4}  \cancel{\epsilon_3} (\cancel{p_2} - mc)] \\ 
\\
\frac{g_e^4}{4(p_1\cdot p_4)^2} \text{Tr}[\cancel{\epsilon_3^*} \cancel{\epsilon_4^*} \cancel{p_4} (\cancel{p_1}+ mc)  \cancel{p_4} \cancel{\epsilon_4}  \cancel{\epsilon_3} (\cancel{p_2} - mc)] \\
\end{aligned} 
$$

Esta expresión puede simplificarse aun mas usando algebras de Clifford. Hallemos la primera de las trazas.

$$
\begin{aligned}
T \equiv \text{Tr}[\cancel{\epsilon_4^*} \cancel{\epsilon_3^*} 
\cancel{p_3} (\cancel{p}_1+ mc)  \cancel{p_3} \cancel{\epsilon_3}  \cancel{\epsilon_4} (\cancel{p_2} - mc)] \\ 
\\
= \text{Tr}[\cancel{\epsilon_4^*} \cancel{\epsilon_3^*} 
\cancel{p_3} \cancel{p_1}   \cancel{p_3} \cancel{\epsilon_3}  \cancel{\epsilon_4} \cancel{p_2}] - (mc)^2 \text{Tr}[\cancel{\epsilon_4^*} \cancel{\epsilon_3^*} 
\cancel{p_3} \cancel{p_3} \cancel{\epsilon_3}  \cancel{\epsilon_4} ] \\ 
\end{aligned}
$$

Donde se uso que la traza de un numero impar de matrices es cero. Notemos que el momento $p_3$ corresponde a un fotón, por lo que $(p_3 \cdot p_3) = 0$. Teniendo en cuenta esto veamos que:

$$
\cancel{p_3}\cancel{p_3} = \gamma^{\mu} \gamma^{\nu} p_{3\mu} p_{3\nu} = 2(p_3\cdot p_3) - \cancel{p_3}\cancel{p_3} = - \cancel{p_3}\cancel{p_3} =0
$$

Luego el segundo termino de la traza se anula. Podemos usar esta idea para simplificar el primer termino. Notemos que:

$$
\cancel{p_1}\cancel{p_3} = 2(p_1\cdot p_3) - \cancel{p_3} \cancel{p_1}
$$

Luego el termino restante se puede separar en dos sumas, una de las cuales vuelve a tener un termino $\cancel{p_3}\cancel{p_3}$ que la vuelve nula. Esto es:

$$
\begin{aligned}
\Rightarrow T = 2(p_1\cdot p_3) \text{Tr}[\cancel{\epsilon_4^*} \cancel{\epsilon_3^*} 
\cancel{p_3}\cancel{\epsilon_3}  \cancel{\epsilon_4} \cancel{p_2}] - \text{Tr}[\cancel{\epsilon_4^*} \cancel{\epsilon_3^*} 
\cancel{p_3}  \cancel{p_3} \cancel{p_1} \cancel{\epsilon_3}  \cancel{\epsilon_4} \cancel{p_2}]
\\
= 2(p_1\cdot p_3) \text{Tr}[\cancel{\epsilon_4^*} \cancel{\epsilon_3^*} 
\cancel{p_3}\cancel{\epsilon_3}  \cancel{\epsilon_4} \cancel{p_2}] 
\end{aligned}
$$

Ahora, utilizando la transversalidad de la polarización ($p_3 \cdot \epsilon_3 = 0$), obtenemos las expresiones:

$$ 
\cancel{\epsilon_3} \cancel{p_3} = 2(\epsilon_3 \cdot p_3) - \cancel{p_3} \cancel{\epsilon_3} = - \cancel{p_3}  \cancel{\epsilon_3}
$$

$$
\cancel{\epsilon^*_3} \cancel{\epsilon_3} = \gamma^{\mu} \gamma^{\nu} \epsilon^*_{3\mu} \epsilon_{3\nu} = \frac{1}{2} (\gamma^{\mu} \gamma^{\nu}  + \gamma^{\nu} \gamma^{\mu}) \epsilon^*_{3\mu} \epsilon_{3\nu} = g^{\mu\nu }\epsilon^*_{3\mu} \epsilon_{3\nu} = -1
$$

Reemplazando:

$$
T = 2(p_1\cdot p_3) \text{Tr}[\cancel{\epsilon_4^*}
\cancel{p_3} \cancel{\epsilon_4} \cancel{p_2}] 
$$

Desarrollando los términos $\cancel{p_3} \cancel{\epsilon_4}$ de la misma forma, la traza se puede expresar como:

$$
T_1 = 4(p_1\cdot p_3)(p_3\cdot\epsilon_4) \text{Tr}[\cancel{\epsilon_4^*} \cancel{p_2}] - 2(p_1\cdot p_3) \text{Tr}[\cancel{p_3} \cancel{p_2}]
$$

Evaluando las trazas que quedan:

$$
\text{Tr}[\cancel{\epsilon_4^*} \cancel{p_2}] = 4(\epsilon_4^* \cdot p_2)
\qquad
\text{Tr}[\cancel{p_3} \cancel{p_2}] = 4(p_3\cdot p_2)
$$

Obtenemos una expresión explicita para la traza en términos de los momentos. 

$$
T_1 = 16(p_1\cdot p_3)(p_3\cdot\epsilon_4)(\epsilon_4^* \cdot p_2) - 8(p_1\cdot p_3) (p_3\cdot p_2)
$$

Usando la conservación del momento:

$$
p_1 + p_2 = p_3 + p_4
$$

$$
p_3 = p_1 + p_2 - p_4
$$

$$
p_3 \cdot \epsilon_4 = ( p_1 + p_2 - p_4) \cdot \epsilon_4 = p_2 \cdot \epsilon_4
$$

$$
(p_3\cdot\epsilon_4)(\epsilon_4^* \cdot p_2) = (p_2 \cdot \epsilon_4)(\epsilon_4^* \cdot p_2)  = (p_2 \cdot\epsilon_4)^2
$$

Por otra parte:

$$
p_1 - p_4 = p_3 - p_2
$$

$$
(p_1 - p_4)^2 = (p_3 - p_2)^2
$$

$$
m^2c^2 -2(p_1\cdot p_4) = m^2c^2 - 2(p_3 \cdot p_2)
$$

$$
p_3 \cdot p_2 = p_1 \cdot p_4
$$

Finalmente:

$$
\langle \mathcal{M}_1 \mathcal{M}^*_1 \rangle = 2g_e^4 \left[ 2 \frac{(p_2\cdot\epsilon_4)^2}{(p_1\cdot p_3)} - \frac{(p_1\cdot p_4)}{(p_1\cdot p_3)} \right]
$$

De la misma forma se puede hallar $\langle \mathcal{M}_2 \mathcal{M}^*_2 \rangle$ sustituyendo el orden de los fotones $3 \leftrightarrow 4$ como en los diagramas, y obtenemos que:

$$
\langle \mathcal{M}_2 \mathcal{M}^*_2 \rangle = 2g_e^4 \left[2\frac{(p_2\cdot\epsilon_3)^2}{(p_1\cdot p_4)} - \frac{(p_1\cdot p_3)}{(p_1\cdot p_4)} \right]
$$

Nos quedan hallar las trazas correspondientes a los términos cruzados. Veamos la segunda traza:

$$
T_2 = \text{Tr}[\cancel{\epsilon_3^*} \cancel{\epsilon_4^*} \cancel{p_4} (\cancel{p_1}+ mc)  \cancel{p_3} \cancel{\epsilon_3}  \cancel{\epsilon_4} (\cancel{p_2} - mc)]
$$

Usando la conservación del momento, notemos que:

$$
\cancel{p_2} = \cancel{p_3} + \cancel{p_4} - \cancel{p_1} 
$$

Luego:

$$
\begin{aligned} 
T_2 = - \text{Tr}[\cancel{\epsilon_3^*} \cancel{\epsilon_4^*} \cancel{p_4} (\cancel{p_1} + mc)  \cancel{p_3} \cancel{\epsilon_3}  \cancel{\epsilon_4} (\cancel{p_1}+ mc) ] \\
+ \text{Tr}[\cancel{\epsilon_3^*} \cancel{\epsilon_4^*} \cancel{p_4} (\cancel{p}_1+ mc)  \cancel{p_3} \cancel{\epsilon_3}  \cancel{\epsilon_4} (\cancel{p_3} + \cancel{p_4} ) ] \\ \\
= - \text{Tr}[\cancel{\epsilon_3^*} \cancel{\epsilon_4^*} \cancel{p_4} \cancel{p_1}  \cancel{p_3} \cancel{\epsilon_3}  \cancel{\epsilon_4} \cancel{p_1} ] - (mc)^2 \text{Tr}[\cancel{\epsilon_3^*} \cancel{\epsilon_4^*} \cancel{p_4} \cancel{p_3} \cancel{\epsilon_3}  \cancel{\epsilon_4}] \\
+ \text{Tr}[\cancel{\epsilon_3^*} \cancel{\epsilon_4^*} \cancel{p_4} \cancel{p_1} \cancel{p_3} \cancel{\epsilon_3}  \cancel{\epsilon_4} (\cancel{p_3} + \cancel{p_4}  ) ]  
\end{aligned} 
$$

En donde los términos con un numero impar de matrices nuevamente se anulan. Usamos que:

$$
\cancel{\epsilon_3} \cancel{p_1}  = - \cancel{p_1} \cancel{\epsilon_3}  \qquad 
\cancel{\epsilon_4} \cancel{p_1} =  - \cancel{p_1} \cancel{\epsilon_4}     
$$

$$
\cancel{p_1} \cancel{p_3} \cancel{p_1} = 2(p_1\cdot p_3) \cancel{p_1} - \cancel{p_3} \cancel{p_1} \cancel{p_1} =  2(p_1\cdot p_3) \cancel{p_1} - (mc)^2\cancel{p_3}
$$

Y la propiedad cíclica de la traza, podemos permutar las polarizaciones como:

$$
\begin{aligned} 
\text{Tr}[\cancel{\epsilon_3^*} \cancel{\epsilon_4^*} \cancel{p_4} \cancel{p_1}  \cancel{p_3} \cancel{\epsilon_3}  \cancel{\epsilon_4} \cancel{p_1} ] = 
\text{Tr}[ \cancel{p_4} \cancel{p_1}  \cancel{p_3} \cancel{p_1}
\cancel{\epsilon_3}  \cancel{\epsilon_4}
\cancel{\epsilon_3^*} \cancel{\epsilon_4^*} ]
\\ \\
= - 2(p_1 \cdot p_3 )\text{Tr}[ \cancel{p_4} \cancel{p_1}
\cancel{\epsilon_3}  \cancel{\epsilon_4}
\cancel{\epsilon_3^*} \cancel{\epsilon_4^*} ] 
+ (mc)^2 \text{Tr}[ \cancel{p_4} \cancel{p_3}
\cancel{\epsilon_3}  \cancel{\epsilon_4}
\cancel{\epsilon_3^*} \cancel{\epsilon_4^*} ]
\end{aligned} 
$$

El ultimo termino se anula con otro de la expresión principal, mientras que para el primero podemos permutar $\cancel{p_1}$ con las polarizaciones usando las identidades arriba descritas, por lo que:

$$
\text{Tr}[ \cancel{p_4} \cancel{p_1}
\cancel{\epsilon_3}  \cancel{\epsilon_4}
\cancel{\epsilon_3^*} \cancel{\epsilon_4^*} ] = \text{Tr}[ \cancel{p_1} \cancel{p_4}
\cancel{\epsilon_3}  \cancel{\epsilon_4}
\cancel{\epsilon_3^*} \cancel{\epsilon_4^*} ]  = \text{Tr}[  \frac{1}{2}(\cancel{p_1} \cancel{p_4} + \cancel{p_4} \cancel{p_1})
\cancel{\epsilon_3}  \cancel{\epsilon_4}
\cancel{\epsilon_3^*} \cancel{\epsilon_4^*} ]
$$

Luego podemos reemplazar el termino simétrico usando que el anti conmutador de las matrices de Dirac esta dado por la métrica:

$$
 \frac{1}{2}(\cancel{p_1} \cancel{p_4} + \cancel{p_4} \cancel{p_1}) = p_{1\mu} p_{4\nu}  \frac{1}{2} (\gamma^{\mu} \gamma^{\nu} + \gamma^{\nu} \gamma^{\mu}) =   p_{1\mu} p_{4\nu} g^{\mu \nu} =(p_1 \cdot p_4)
$$

Luego 

$$
\begin{aligned}
\text{Tr}[\cancel{\epsilon_3}  \cancel{\epsilon_4}\cancel{\epsilon_3^*} \cancel{\epsilon_4^*}] = \epsilon_{3\mu} \epsilon_{4\nu}  \epsilon^*_{3\lambda} \epsilon^*_{4\sigma} 4(g^{\mu \nu}g^{\lambda \sigma} - g^{\mu \lambda}g^{\nu \sigma} + g^{\mu \sigma}g^{\nu \lambda}) \\ \\
= 4(\epsilon_3\cdot \epsilon_4)(\epsilon^*_3\cdot \epsilon^*_4) - 4(\epsilon_3\cdot \epsilon^*_3)(\epsilon_4\cdot \epsilon^*_4) + 4(\epsilon_3\cdot \epsilon^*_4) (\epsilon^*_3\cdot \epsilon_4) \\ \\
= 16(\epsilon_3\cdot \epsilon_4)^2 - 8\\
\end{aligned}
$$

Reemplazando obtenemos el primer termino de la traza:

$$ 
\begin{aligned} - 
\text{Tr}[\cancel{\epsilon_3^*} \cancel{\epsilon_4^*} \cancel{p_4} \cancel{p_1}  \cancel{p_3} \cancel{\epsilon_3}  \cancel{\epsilon_4} \cancel{p_1} ] - (mc)^2 \text{Tr}[\cancel{\epsilon_3^*} \cancel{\epsilon_4^*} \cancel{p_4} \cancel{p_3} \cancel{\epsilon_3}  \cancel{\epsilon_4}] \\ \\ 
= -8(p_1\cdot p_3)(p_1\cdot p_4)\big(2(\epsilon_3\cdot \epsilon_4)^2 - 1 \big)
\end{aligned}
$$

Veamos ahora el segundo termino:

$$
\text{Tr}[\cancel{\epsilon_3^*} \cancel{\epsilon_4^*} \cancel{p_4} \cancel{p_1} \cancel{p_3} \cancel{\epsilon_3}  \cancel{\epsilon_4} (\cancel{p_3} + \cancel{p_4}  ) ]  = 
\text{Tr}[\cancel{p_4} \cancel{p_1} \cancel{p_3} \cancel{\epsilon_3}  \cancel{\epsilon_4} (\cancel{p_3} + \cancel{p_4}  ) \cancel{\epsilon_3^*} \cancel{\epsilon_4^*} ]
$$

Desarrollando los últimos términos dentro de la traza:

$$
(\cancel{p_3} + \cancel{p_4}) \cancel{\epsilon_3^*} \cancel{\epsilon_4^*} = - \cancel{\epsilon^*_3} \cancel{p_3} \cancel{\epsilon^*_4} + \cancel{p_4} \cancel{\epsilon^*_3} \cancel{\epsilon^*_4} = - \cancel{\epsilon^*_3} \cancel{p_3} \cancel{\epsilon^*_4} + 2(p_4 \cdot \epsilon^*_3) \cancel{\epsilon^*_4} - \cancel{\epsilon^*_3} \cancel{p_4} \cancel{\epsilon^*_4}
$$
La traza será:

$$
\begin{aligned}
...= 2(p_4 \cdot \epsilon^*_3) \text{Tr}[\cancel{p_4} \cancel{p_1} \cancel{p_3} \cancel{\epsilon_3}  \cancel{\epsilon_4} \cancel{\epsilon_4^*} ] - \text{Tr}[\cancel{p_4} \cancel{p_1} \cancel{p_3} \cancel{\epsilon_3}  \cancel{\epsilon_4} \cancel{\epsilon_3^*} (\cancel{p_3} + \cancel{p_4})\cancel{\epsilon_4^*} ] \\ \\
= 
2(p_4 \cdot \epsilon^*_3) \text{Tr}[\cancel{p_4} \cancel{p_1} \cancel{p_3} \cancel{\epsilon_3}  \cancel{\epsilon_4} \cancel{\epsilon_4^*} ] - \text{Tr}[\cancel{p_4} \cancel{p_1} \cancel{p_3} \cancel{\epsilon_3}  \cancel{\epsilon_4} \cancel{\epsilon_3^*} \cancel{p_3}\cancel{\epsilon_4^*} ] \\ \\
= -
2(p_4 \cdot \epsilon^*_3) \text{Tr}[\cancel{p_4} \cancel{p_1} \cancel{p_3} \cancel{\epsilon_3} ] + \text{Tr}[\cancel{p_4} \cancel{p_1} \cancel{p_3} \cancel{\epsilon_3}  \cancel{\epsilon_4} \cancel{p_3} \cancel{\epsilon_3^*} \cancel{\epsilon_4^*} ]
\end{aligned}
$$

En donde se utilizó que $\cancel{p_4} \cancel{\epsilon^*_4} = - \cancel{\epsilon^*_4}\cancel{p_4}$ y $\cancel{p_4} \cancel{p_4} = 0$ para simplificar.   

$$
\begin{aligned}
\text{Tr}[\cancel{p_4} \cancel{p_1} \cancel{p_3} \cancel{\epsilon_3}  \cancel{\epsilon_4} \cancel{p_3} \cancel{\epsilon_3^*} \cancel{\epsilon_4^*} ] \\ \\
= 2(\epsilon_4\cdot p_3) 
\text{Tr}[\cancel{p_4} \cancel{p_1} \cancel{p_3} \cancel{\epsilon_3} \cancel{\epsilon_3^*} \cancel{\epsilon_4^*} ] +
\text{Tr}[\cancel{p_4} \cancel{p_1} \cancel{p_3} \cancel{p_3} \cancel{\epsilon_3}  \cancel{\epsilon_4} \cancel{\epsilon_3^*} \cancel{\epsilon_4^*} ] \\ \\
= 2(\epsilon_4\cdot p_3) 
\text{Tr}[\cancel{p_4} \cancel{p_1} \cancel{p_3} \cancel{\epsilon_3} \cancel{\epsilon_3^*} \cancel{\epsilon_4^*} ] = - 2(\epsilon_4\cdot p_3) 
\text{Tr}[\cancel{p_4} \cancel{p_1} \cancel{p_3} \cancel{\epsilon_4^*} ]
\end{aligned}
$$

Luego la traza será:

$$
... = -
2(p_4 \cdot \epsilon^*_3) \text{Tr}[\cancel{p_4} \cancel{p_1} \cancel{p_3} \cancel{\epsilon_3} ] - 2(\epsilon_4\cdot p_3) 
\text{Tr}[\cancel{p_4} \cancel{p_1} \cancel{p_3} \cancel{\epsilon_4^*} ] \\ \\
$$

Evaluando:

$$
\begin{aligned}
\text{Tr}[\cancel{p_4} \cancel{p_1} \cancel{p_3} \cancel{\epsilon_3} ] = p_{4\mu} p_{1\nu} p_{3\lambda} \epsilon_{3 \sigma} \text{Tr}[\gamma^{\mu} \gamma^{\nu} \gamma^{\lambda} \gamma^{\sigma}] 
\\ \\ 
= p_{4\mu} p_{1\nu} p_{3\lambda} \epsilon_{3 \sigma}  4(g^{\mu\nu} g^{\lambda \sigma} - g^{\mu\lambda} g^{\nu \sigma} + g^{\mu\sigma} g^{\nu \lambda}) 
\\ \\
= 4(p_4\cdot p_1)( p_3 \cdot \epsilon_3) - 4(p_4 \cdot p_3)(p_1 \cdot \epsilon_3) + 4(p_4 \cdot \epsilon_3) (p_1\cdot p_3)
\end{aligned}
$$


$$
\begin{aligned}
\text{Tr}[\cancel{p_4} \cancel{p_1} \cancel{p_3} \cancel{\epsilon^*_4} ] = p_{4\mu} p_{1\nu} p_{3\lambda} \epsilon_{4 \sigma} \text{Tr}[\gamma^{\mu} \gamma^{\nu} \gamma^{\lambda} \gamma^{\sigma}] 
\\ \\ 
= p_{4\mu} p_{1\nu} p_{3\lambda} \epsilon^*_{4 \sigma}  4(g^{\mu\nu} g^{\lambda \sigma} - g^{\mu\lambda} g^{\nu \sigma} + g^{\mu\sigma} g^{\nu \lambda}) 
\\ \\
= 4(p_4\cdot p_1)( p_3 \cdot \epsilon^*_4) - 4(p_4 \cdot p_3)(p_1 \cdot \epsilon^*_4) + 4(p_4 \cdot \epsilon^*_4) (p_1\cdot p_3)
\end{aligned}
$$

Usando que $p_3\cdot \epsilon_3 = p_4 \cdot \epsilon_4 = 0$ y reemplazando:

$$
\begin{aligned}
... = -8(p_4 \cdot \epsilon^*_3) \big(- (p_4 \cdot p_3)(p_1 \cdot \epsilon_3) + (p_4 \cdot \epsilon_3) (p_1\cdot p_3)\big) \\ \\
-8 (\epsilon_4\cdot p_3) \big( (p_4\cdot p_1)( p_3 \cdot \epsilon^*_4) - (p_4 \cdot p_3)(p_1 \cdot \epsilon^*_4) \big)
\end{aligned}
$$

$$\begin{aligned}
= 
- 8(p_4 \cdot \epsilon_3)^2(p_1\cdot p_3) - 8 (\epsilon_4\cdot p_3) ^2(p_1\cdot p_4) \\ \\+ 8(p_4 \cdot \epsilon^*_3) (p_4 \cdot p_3)(p_1 \cdot \epsilon_3) + 8(\epsilon_4\cdot p_3)(p_4 \cdot p_3)(p_1 \cdot \epsilon^*_4)
\end{aligned}
$$

Usando además que $p_1 \cdot \epsilon_3 = p_1 \cdot \epsilon_4^* = 0$ los últimos dos términos se cancelan. Reemplazando todo, la segunda traza será:

$$
\begin{aligned}
... = -8 \big[ (p_1\cdot p_3)(p_1\cdot p_4)\big(2(\epsilon_3\cdot \epsilon_4)^2 - 1 \big) - (p_4 \cdot \epsilon_3)^2(p_1\cdot p_3) - (\epsilon_4\cdot p_3)^2(p_1\cdot p_4) \big] \\ \\
= (p_1\cdot p_3)( p_1\cdot p_4) \big[ 
	2(\epsilon_3\cdot \epsilon_4)^2 - 1 + \frac{(p_4\cdot \epsilon_3)^2}{(p_1 \cdot p_4)}+ \frac{(\epsilon_3 \cdot p_4)^2}{(p_1 \cdot p_3)}
\big]
\end{aligned}
$$

$$
\langle \mathcal{M}_2 \mathcal{M}_1^* \rangle = 2g_e^2 \big[ 
	2(\epsilon_3\cdot \epsilon_4)^2 - 1 + \frac{(p_4\cdot \epsilon_3)^2}{(p_1 \cdot p_4)}+ \frac{(\epsilon_4 \cdot p_3)^2}{(p_1 \cdot p_3)}
\big]
$$

Al igual que en el primer caso, podemos reemplazar los fotones como $3 \leftrightarrow 4$ y obtener el termino restante.

$$
\langle \mathcal{M}_1 \mathcal{M}_2^* \rangle = 2g_e^2 \big[ 
	2(\epsilon_4\cdot \epsilon_3)^2 - 1 + \frac{(p_3\cdot \epsilon_4)^2}{(p_1 \cdot p_3)}+ \frac{(\epsilon_3 \cdot p_4)^2}{(p_1 \cdot p_4)}
\big] = 
\langle \mathcal{M}_2 \mathcal{M}_1^* \rangle
$$

Trayendo nuevamente los términos hallados al principio:

$$
\langle \mathcal{M}_1 \mathcal{M}^*_1 \rangle = 2g_e^4 \left[ 2 \frac{(p_2\cdot\epsilon_4)^2}{(p_1\cdot p_3)} - \frac{(p_1\cdot p_4)}{(p_1\cdot p_3)} \right]
$$

$$
\langle \mathcal{M}_2 \mathcal{M}^*_2 \rangle = 2g_e^4 \left[2\frac{(p_2\cdot\epsilon_3)^2}{(p_1\cdot p_4)} - \frac{(p_1\cdot p_3)}{(p_1\cdot p_4)} \right]
$$

El modulo cuadrado de la amplitud será:

$$ 
\langle |\mathcal{M}| ^2 \rangle = \langle |\mathcal{M}_1|^2 \rangle + \langle |\mathcal{M}_2|^2 \rangle + 2\langle \mathcal{M}_1 \mathcal{M}_2^* \rangle
$$

--- 