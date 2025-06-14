Las interacciones de Van Der Waals describen las fuerzas intermoleculares que surgen entre átomos y moléculas neutras. Estas fuerzas, aunque más débiles que los enlaces químicos covalentes o iónicos, desempeñan un papel fundamental en la estructura y comportamiento de sistemas físicos y biológicos. Dentro de estas interacciones se incluyen las fuerzas de dispersión de London, las fuerzas dipolo-dipolo y las fuerzas dipolo inducido.

Una forma común de modelar las interacciones de Van Der Waals entre dos átomos o moléculas es mediante el potencial de Lennard-Jones, que es un potencial fenomenológico que modela tanto la atracción debida a las fuerzas de dispersión como la repulsión a cortas distancias debido al principio de exclusión de Pauli. Este potencial puede expresarse como: 

$$
V(R) = 4\epsilon \left[ \left( \frac{\sigma}{R} \right)^{12} - \left( \frac{\sigma}{R} \right)^{6} \right]
$$

Donde $R$ es la distancia entre los dos átomos o moléculas, $\epsilon$ y $\sigma$ dos parámetros del potencial. El primer término en la ecuación representa la repulsión a cortas distancias (exponente 12), mientras que el segundo término modela la atracción de Van Der Waals (exponente 6). 

--- 
### Ejemplo

Discutamos la posibilidad de formarse la posibilidad de formarse la moléculas de $\text{Ar}_2$ y $\text{He}_2$ utilizando el potencial de Lennard-Jones y su energía de punto cero. Los parámetros del potencial para el $\text{Ar}$ y $\text{He}$ son $\sigma = 0.340 \text{nm}$, $\epsilon = 10.5 \text{meV}$ y $\sigma = 0.256 \text{nm}$, $\epsilon = 0.879 \text{meV}$ respectivamente. 

Hallemos primero el mínimo del potencial, la tasa de crecimiento del potencial con respecto a la separación inter-nuclear será: 

$$
V'(R) = 24 \epsilon_0 \left( -2 \frac{\sigma^{12}}{R^{13}} + \frac{\sigma^6}{R^7} \right)
$$

Podemos hallar de esta forma, la separación de equilibrio $R_0$, tomando $V'(R_0) = 0$:

$$ 
24 \epsilon \left( -2 \frac{\sigma^{12}}{R_0^{13}} + \frac{\sigma^6}{R_0^7} \right) = 0 \Rightarrow -2 \frac{\sigma^{6}}{R_0^{6}} + 1 = 0 \Rightarrow R_0 = 2^{1/6}\sigma
$$

Reemplazando en el potencial:
 
$$
V(R_0) = 4\epsilon \left[ \left( \frac{\sigma}{ 2^{1/6}\sigma} \right)^{12} - \left( \frac{\sigma}{ 2^{1/6}\sigma} \right)^{6} \right] = 4\epsilon(\frac{1}{2^2} - \frac{1}{2}) = - \epsilon
$$


Esto nos indica que la energía de disociación (desde el mínimo hasta $R \to \infty$) es simplemente $\epsilon$ es decir  $10.5, \text{meV}$ para el $\text{Ar}_2$ y $0.879, \text{meV}$ para el $\text{He}_2$. 
 
Para que estas moléculas existan y sean estables a cierta temperatura, la energía térmica $k_b T$ no debe superar esta profundidad del pozo de potencial; de lo contrario, el enlace se rompería fácilmente. A temperatura ambiente, la energía térmica es aproximadamente:

$$
k_B T \approx 24\text{meV}$$

Dado que $\epsilon_{\text{Ar}} = 10.5, \text{meV} < k_B T$ y $\epsilon_{\text{He}} = 0.879, \text{meV} \ll k_B T$, concluimos que **ninguna de estas moléculas es estable a temperatura ambiente**, pues la energía térmica es suficiente para romper el enlace.

Sin embargo, esta conclusión solo considera el efecto de la energía térmica. A temperaturas suficientemente bajas, cuando la energía térmica ya no es significativa, puede preguntarse si estas moléculas podrían formar **estados ligados cuánticos**. Para responder a esto, es necesario considerar la **energía de punto cero** del sistema.

Cuando dos átomos están ligados, incluso en su estado fundamental, **no permanecen fijos en la distancia de equilibrio**, sino que vibran en torno a ella debido al principio de incertidumbre. Esta vibración mínima tiene una energía asociada conocida como **energía de punto cero**, la cual puede ser estimada modelando la interacción como un **oscilador armónico** alrededor del mínimo del potencial de Lennard-Jones.

Si esta energía de punto cero es **menor que la energía de enlace (i.e. menor que $\epsilon$)**, entonces existe al menos un estado ligado. En caso contrario, el estado más bajo del sistema aún se encuentra por encima del nivel de disociación, por lo que la molécula **no puede existir ni siquiera a temperatura cero absoluto**.

Para bajas energías, el movimiento del par de átomos de las moléculas, puede describirse como oscilaciones alrededor de su distancia de equilibrio $R_0$. Veamos esto, para ello desarrollemos el potencial de Lennard-Jones hasta segundo orden, al rededor de $R_0$:

$$
V(R) = V(R_0) + V'(R_0)(R-R_0) + \frac{1}{2}V''(R_0)(R-R_0)^2
$$

El termino de orden uno, es nulo en la posición de equilibrio y el segundo termino lo podemos hallar derivando y evaluando en $R_0$:

$$
V''(R) = 24 \epsilon \left( 26\frac{\sigma^{12}}{R^{14}} - 7\frac{\sigma^6}{R^8} \right)
$$

$$
V''(R_0) = 24\epsilon \left( 26\frac{\sigma^{12}}{(2^{1/6}\sigma)^{14}} - 7\frac{\sigma^6}{(2^{1/6}\sigma)^8} \right) = 24\frac{\epsilon}{\sigma^2} \left( \frac{26}{2^{14/6}} - \frac{7}{2^{8/6}} \right)
$$

$$
= 12 \frac{\epsilon}{\sigma^2}\left( \frac{13}{2^{2/6}} - \frac{7}{2^{2/6}} \right) = \frac{12(13-7)}{2^{1/3}} \frac{\epsilon}{\sigma^2} = \frac{72}{2^{1/3}}\frac{\epsilon}{\sigma^2} \Rightarrow V''(R_0) = 72 \frac{\epsilon}{R_0^2}
$$

Podemos entonces escribir el potencial de interacción entre los átomos a segundo orden como:

$$
V(R) \approx -\epsilon + 36 \frac{\epsilon}{R_0^2}\left(R - R_0 \right)^2 
$$

Tomando ahora la posición relativa a la posición de equilibrio $r \equiv R - R_0$, y a la curvatura del potencial como constante elástica $k \equiv 72\epsilon /R_0^2$, podemos escribir el hamiltoniano del sistema como: 

$$
\hat{H} = -\frac{\hbar^2}{2\mu}\nabla^2 + \frac{1}{2}kr^2
$$

El cual es el hamiltoniano del oscilador armónico, con $\mu$ la masa reducida de la molécula (igual a $m/2$ ya que hablamos de moléculas diatómicas), la frecuencia tal que $\mu \omega^2 = k$ y auto-energías conocidas, con valor:

$$
E_{n} = \hbar \omega \left(n + \frac{1}{2} \right) \qquad n = 0, 1, 2,...
$$

La energía de punto cero, será entonces la energía del estado fundamental $E_0 = \frac{\hbar \omega}{2}$, la cual podemos hallar reemplazando:

$$ 
E_0 = \frac{\hbar}{2} \sqrt{\frac{72\epsilon}{R_0^2}\frac{2}{m}} = \frac{6\hbar}{2^{1/6}\sigma}\sqrt{\frac{\epsilon}{m}} 
$$
 
 Reemplazando para el $\text{Ar}_2$:
  
- $\hbar = 4.135 \times 10^{-15} \text{eV}\cdot \text{s}$
- $\sigma = 0.340 \times 10^{-9} \text{m}$
- $\epsilon = 10.5 \times 10^{-3} \text{eV}$
- $m = 39.948 \text{u}$

Obtenemos $E_0 \approx 10.36 \text{meV} \lt \epsilon$ esto nos dice que a temperaturas cercanas a $0 \text{K}$ la molécula de $\text{Ar}_2$ puede formarse. De echo esta molécula fue sintetizada experimentalmente. Por otra parte para el $\text{He}_2$ reemplazando:

- $\sigma = 0.256 \times 10^{-9} \text{m}$
- $\epsilon = 0.879 \times 10^{-3} \text{eV}$
- $m = 4.002\text{u}$

Obtenemos que $E_0 \approx 12.58 \text{meV} \gt \gt \epsilon$ por lo que la molécula no podría formarse ni siquiera a $\text{0}K$ ya que su energía mínima posible es mayor a la profundidad del pozo. 