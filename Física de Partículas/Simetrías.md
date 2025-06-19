Una simetría se define como una operación que puede ser efectuada en un sistema dejándolo invariante. El conjunto de todas las simetrías tiene las siguientes propiedades:

- *Clausura*: Si $R_i$ y $R_j$ están en el conjunto entonces el producto $R_i R_j$  esta en el conjunto.
	
- *Identidad*: Existe un elemento $I$ tal que $IR_i = R_i I = R_i$ para todos los elementos $R_i$.
	
- *Inversa*: Para cada elemento $R_i$ existe una inversa $R_i^{-1}$ tal que $R_i R_i^{-1} = I$.
	
- *Asociatividad*: Para elementos $R_i$, $R_j$ y $R_k$ se verifica que $(R_i R_j) R_k = R_i (R_j R_k)$.  

Definidas de esta forma, estas propiedades forman lo que se denomina grupo. Nótese que los elementos de un grupo no necesariamente conmutan. Si estos conmutan entonces el grupo se denomina *Abeliano*. 

La mayoría de los grupos de interés en física pueden ser formulados en términos de *grupo de matrices*. Denotamos:

- $U(n)$ al grupo de todas las matrices $n \times n$ unitarias.  
	
- $SU(n)$ al grupo de todas las matrices $n \times n$ unitarias cuyo determinante es $1$. 
	
- $O(n)$ al grupo de todas las matrices $n \times n$ ortogonales. 
	
- $SO(n)$ al grupo de todas las matrices $n\times n$ ortogonales cuyo determinante es $1$. 

Finalmente, cada grupo $G$ puede ser representado por un grupo de matrices, es decir a cada elemento $a \in G$ le corresponde una matriz $M_a$ y la correspondiente operación de multiplicación, es decir si $ab = c$ entonces $M_a M_b = M_c$.

Siempre es posible construir una nueva representación matricial de un grupo combinando otras dos existentes, es decir si $M_a^{(1)}$ y $M_a^{(2)}$ son representaciones de $G$ entonces una nueva representación puede ser construida como:

$$
M_a = \begin{pmatrix} M_a^{(1)} & 0 \\ 0 & M^{(2)}_a \end{pmatrix}
$$

Es por esto que cuando hablamos de la representación de un grupo, nos referimos a las *representaciones irreducibles* de este. 

### Isospín

Si se deja de lado la carga y la pequeña diferencia de masa entre el neutrón y el protón, podemos considerar que ambos pueden ser estados de una misma partícula, el nucleón. Denotemos a estos estados como:

$$
\ket{p} = \begin{pmatrix}1 \\0 \end{pmatrix} \qquad \ket{n} = \begin{pmatrix} 0 \\ 1 \end{pmatrix}
$$

Introducimos entonces al *isospín* $\vec{I}$ como al operador generado de simetrías internas, en este caso asociado al grupo $SU(2)$, que actúa sobre el doblete de nucleones $(p, n)$. Esta construcción es análoga a la del espín en mecánica cuántica, pero en un espacio interno de sabor de las partículas.

Los generadores del grupo $SU(2)$ se representan mediante matrices de Pauli y las componentes del isospín pueden escribirse como:

$$
\hat{I}_i = \frac{1}{2} \hat{\sigma}_i \qquad i=1,2,3
$$

En donde:

$$
\sigma_1 = \begin{pmatrix} 0 & 1 \\  1 & 0 \end{pmatrix} \qquad
\sigma_2 = \begin{pmatrix} 0 & -i \\  i & 0 \end{pmatrix} \qquad
\sigma_3 = \begin{pmatrix} 1 & 0 \\  0 & -1 \end{pmatrix} \qquad
$$
 
 Estos operadores satisfacen las relaciones de conmutación d $SU(2)$. Los autovalores del operador $I_3$​, componente del isospín, permiten distinguir al protón del neutrón como:

$$
\hat{I}_3 p = \frac{1}{2} \ket{p} \qquad \hat{I}_3 n = -\frac{1}{2} \ket{n}
$$

Y podemos usar la misma notación que para los momentos angulares:

$$
\ket{p} = \ket{\frac{1}{2}, \frac{1}{2}} \qquad \ket{n} =  \ket{\frac{1}{2}, \frac{1}{2}} 
$$
 
 Heisenberg propuso que la interacción fuerte es invariante bajo rotaciones en el espacio del isospín. Esto es lo que denominamos una simetría interna. Por ejemplo, una rotación de $180^\circ$ alrededor del eje $1$ en el espacio del isospín convierte a un protón en un neutrón y viceversa. Luego, por el teorema de Noether, se concluye que el isospín se conserva en todas las interacciones fuertes.

La simetría de isospín también es aplicable a todos los estados que conforman los múltipletes de hadrones, generalizando así el tratamiento del protón y el neutrón a otros sistemas. Consideremos por ejemplo el pión, asignamos a estos un isospín $I_3=1$ y denotamos:

$$
\pi^+ = \ket{1,1} \qquad
\pi^0 = \ket{1,0} \qquad
\pi^- = \ket{1,-1} \qquad
$$

De la misma forma para las partículas delta, a las cuales asignamos un isospín $I_3 = 3/2$ y denotamos:

$$
\Delta^{++} = \ket{\frac{3}{2}, \frac{3}{2}} \qquad
\Delta^{+} = \ket{\frac{3}{2}, \frac{1}{2}} \qquad
\Delta^{0} = \ket{\frac{3}{2}, -\frac{1}{2}} \qquad
\Delta^{-} = \ket{\frac{3}{2}, -\frac{3}{2}} \qquad
$$

Para determinar el isospín $I_3$ de un multiplete contamos las partículas que lo contienen. Dado a que los autovalores de $\hat{I}_3$ varían de $-I_3$ hasta $I_3$ en números enteros, el numero de partículas en un multiplete es $2I_3 + 1$. 

La componente $\hat{I}_3$ del isospín puede asociarse a la carga $Q$ de una partícula. Asociamos al máximo autovalor de $\hat{I}_3$ el miembro del multiplete con mayor carga y al mínimo con el de menor carga.  La relación explicita carga isospín es la relación *Gell Mann - Nishijima*:

$$
Q = I_3 + \frac{1}{2}(A + S)
$$

En donde $A$ es el numero bariónico y $S$ la extrañeza de la partícula.


El isospín tiene también implicaciones dinámicas en los hadrones, por ejemplo, si consideramos dos nucleones, podemos construir los siguientes estados combinados de isospín. El **isotriplete simétrico** se expresa como:

$$
\ket{1,1} = \ket{p,p} \qquad 
\ket{1,0} = \frac{\ket{p,n} + \ket{p,n}}{\sqrt{2}} \qquad 
\ket{1,-1} = \ket{n,n}
$$

Mientras que el **isosinglete antisimétrico** es:

$$
\ket{0,0} = \frac{\ket{p,n} - \ket{n,p}}{\sqrt{2}}
$$

Experimentalmente el neutrón y el protón forman un solo estado singlete ligado, el deuterón $\ket{d}$. No hay estado ligado para dos protones o dos neutrones, por lo que el deuterón debe ser el isosinglete. 

---

