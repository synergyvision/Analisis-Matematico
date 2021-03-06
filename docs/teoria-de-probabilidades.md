--- 
title: "Introducción al análisis funcional y a la teoría de la medida"
subtitle: "Ciencia de los Datos Financieros"
author: "Synergy Vision"
date: "2019-03-21"
knit: "bookdown::render_book"
documentclass: krantz
bibliography: [book.bib, packages.bib]
biblio-style: apalike
link-citations: yes
colorlinks: yes
lot: yes
lof: yes
fontsize: 12pt
monofontoptions: "Scale=0.8"
keep_md: yes
site: bookdown::bookdown_site
description: ""
url: 'http\://synergy.vision/Analisis-y-Medida/'
github-repo: synergyvision/Analisis-y-Medida/
cover-image: images/cover.png
---

# Prefacio {-}

Placeholder


## ¿Por qué  leer este libro? {-}
## Estructura del libro {-}
## Información sobre los programas y convenciones {-}
## Prácticas interactivas con R {-}
## Agradecimientos {-}

<!--chapter:end:index.Rmd-->


# Acerca del Autor {-}

Este material es un esfuerzo de equipo en Synergy Vision, (<http://synergy.vision/nosotros/>).		 

El propósito de este material es ofrecer una experiencia de aprendizaje distinta y enfocada en el estudiante. El propósito es que realmente aprenda y practique con mucha intensidad. La idea es cambiar el modelo de clases magistrales y ofrecer una experiencia más centrada en el estudiante y menos centrado en el profesor. Para los temas más técnicos y avanzados es necesario trabajar de la mano con el estudiante y asistirlo en el proceso de aprendizaje con prácticas guiadas, material en línea e interactivo, videos, evaluación contínua de brechas y entendimiento, entre otros, para procurar el dominio de la materia.
  		  
Nuestro foco es la Ciencia de los Datos Financieros y para ello se desarrollará material sobre: **Probabilidad y Estadística Matemática en R**, **Programación Científica en R**, **Mercados**, **Inversiones y Trading**, **Datos y Modelos Financieros en R**, **Renta Fija**, **Inmunización de Carteras de Renta Fija**, **Teoría de Riesgo en R**, **Finanzas Cuantitativas**, **Ingeniería Financiera**, **Procesos Estocásticos en R**, **Series de Tiempo en R**, **Ciencia de los Datos**, **Ciencia de los Datos Financieros**, **Simulación en R**, **Desarrollo de Aplicaciones Interactivas en R**, **Minería de Datos**, **Aprendizaje Estadístico**, **Estadística Multivariante**, **Riesgo de Crédito**, **Riesgo de Liquidez**, **Riesgo de Mercado**, **Riesgo Operacional**, **Riesgo de Cambio**, **Análisis Técnico**, **Inversión Visual**, **Finanzas**, **Finanzas Corporativas**, **Valoración**, **Teoría de Portafolio**, entre otros.

Nuestra cuenta de Twitter es (https://twitter.com/bysynergyvision) y nuestros repositorios están en GitHub (https://github.com/synergyvision).
  		  
 **Somos Científicos de Datos Financieros**

<!--chapter:end:000-author.Rmd-->

\mainmatter

# Introducción 






<!--chapter:end:010-introduction.Rmd-->


# Conjuntos

Placeholder


## Operaciones conjuntistas
## Operaciones conjuntistas
## Sistemas numéricos
## Relaciones  
## Cardinalidad

<!--chapter:end:011-Conjuntos.Rmd-->

# Sistema numérico real y complejo

## Introducción

En este capítulo se introducen las nociones esenciales para el estudio del sistema numérico real, el cual proveerá el basamento teórico para introducir la noción de límite. Por sistema numérico real entendemos a un conjunto no vacío $\mathbb{R}$, junto con dos operaciones binarias, llamadas suma y producto, y una relación de orden total, satisfaciendo tres tipos de axiomas: los axiomas de cuerpo, los axiomas de orden y el axioma de completitud.

Existen varias maneras de construir reigurosamente al conjunto de los números reales. Una de ellas consiste primero en definir al conjunto de los números naturales $\mathbb{N}$, luego a los enteros $\mathbb{Z}$, siguiendo con los racionales $\mathbb{Q}$ y finalmente llegando a los números reales $\mathbb{R}$. En esta construcción, se pide que el conjunto de los números naturales satisfagan una serie de axiomas, llamados axiomas de Peano, los cuales permiten definir las operaciones de suma y producto entre naturales. La resta se introduce luego, agrandando el sistema numérico de los naturales a $\mathbb{Z}$, y permitiendo resolver ecuaciones de la forma $x+m=n$ para una indeterminada $x$, y $m,n \in \mathbb{N}$. Para obtener la división, se identifica el cociente $m/n$, para $m,n \in \mathbb{Z}$ y $n \neq 0$, con la clase $[(m,n)]$ definida a partir de la relación $\sim$ en $\mathbb{Z} \times (\mathbb{Z}\setminus\{0\})$ dada por
\begin{equation}
(m,n) \sim (m',n') \Longleftrightarrow mn'=nm'.
\end{equation}
En este sistema numérico, las ecuaciones del tipo $ax+b=c$, con $a,b,c \in \mathbb{Z}$ y $a\neq 0$, poseen solución. El último paso, la construcción de $\mathbb{R}$ a partir de $\mathbb{Q}$, se realiza (informalmente) llenando los vacíos entre números racionales, mediante la incorporación de los números irracionales. Este es el principio del axioma de completitud.




## Propiedades algebraicas de $\mathbb{R}$

## Estructura de orden de $\mathbb{R}$

## Propiedades de completitud de $\mathbb{R}$

## Inducción matemática

## Espacios euclídeos

<!--chapter:end:101-realesycomplejos.Rmd-->

# Estructuras algebraicas

## Semigrupos y grupos

## Espacios vectoriales

## Transformaciones lineales

## Espacios vectoriales cocientes

## Álgebras

<!--chapter:end:1011-estructurasalgebraicas.Rmd-->

# Sucesiones numéricas

## Límite de una sucesión

## Sucesiones monótonas

## Subsucesiones y sucesiones de Cauchy

## Límites inferior y superior

<!--chapter:end:102-sucesionesnumericas.Rmd-->

# Sucesiones y series

## Límite de una función

## Límites inferior y superior

## Funciones contínuas

## Propiedades de las funciones contínuas

## Continuidad uniforme

<!--chapter:end:103-limiteycontinuidad.Rmd-->


# Diferenciación

Placeholder


## Definición y ejemplos
##  El teorema del valor medio
## Funciones convexas
## Funciones inversas
## Regla de L'Hospital
## Teorema de Taylor en $\mathbb{R}$
## Método de Newton

<!--chapter:end:104-diferenciacionR.Rmd-->


# Integración de Riemann

Placeholder


## Integral de Riemann-Darboux
## Propiedades de la integral
## Evaluación de la integral
## Fórmula de Stirling
## Teoremas del valor medio, versión integral
## Estimación de la integral
## Integrales impropias
## La integrabilidad según Riemann
## Funciones a variación acotada
## La integral de Riemann-Stieltjes

<!--chapter:end:105-integracionR.Rmd-->

# Series numéricas infinitas

## Definición y ejemplos

## Series con términos no-negativos

## Criterios de convergencia

## Convergencia condicional y absoluta

## Sucesiones dobles y series

<!--chapter:end:106-seriesinfinitas.Rmd-->

# Sucesiones y series de funciones

## Convergencia de sucesiones de funciones

## Propiedades del límite de funciones

## Convergencia de las series de funciones

## Series de potencias

<!--chapter:end:107-sucesionesseriesfunciones.Rmd-->

# Funciones en varias variables

## Transformaciones lineales

## Diferenciación

## El principio de la contracción

## El teorema de la función inversa

## El teorema de la función implícita

## Teorema del rango

## Determinantes

## Derivadas de orden superior

## Diferenciación de integrales 

<!--chapter:end:109-funcionesvariasvariables.Rmd-->


# Integración de formas diferenciales

Placeholder


## Integración
## Aplicaciones primitivas
## Cambio de variables
## Formas diferenciales
## Cadenas y símplices
## Teorema de Stoke
## Formas cerradas y formas exactas
## Análisis vectorial

<!--chapter:end:110-integracionformas.Rmd-->

# Funciones especiales

## Series de potencia

## Funciones exponenciales y logarítmicas

## Funciones trigonométricas

## Completitud algebraica del cuerpo de los complejos

## Series de Fourier


<!--chapter:end:201-espaciosmetricos.Rmd-->

# Espacios lineales normados

## Normas y seminormas

## Completación de un espacio normado

## Series infinitas en espacios normados

## Sumas no ordenadas en espacios normados

## Trnasformaciones lineales acotadas

## Álgebras de Banach

<!--chapter:end:2011-espacioslinealesnormados.Rmd-->

# Espacios topológicos

## Abiertos y cerrados

## Sistemas de entornos

## Bases de entornos

## Topología relativa

## Nets

<!--chapter:end:2012-espaciostopologicos.Rmd-->

# Continuidad en espacios topológicos

## Propiedades generales

## Topologías iniciales

## Topología producto

## Topología cociente

## Espacio de funciones contínuas

## Conjuntos F-sigma y G-delta 

<!--chapter:end:2013-continuidadespaciostopológicos.Rmd-->

# Espacios topológicos normados

## Lema de Urysohn

## Teorema de extensión de Tietze

<!--chapter:end:2014-espaciostopologicosnormados.Rmd-->

# Espacios topológicos compactos

## Convergencia en espacios compactos

## Compacidad del producto cartesiano

## Continuidad y compacidad

<!--chapter:end:2015-espaciostopologicoscompactos.Rmd-->

# Espacios métricos totalmente acotados

<!--chapter:end:2016-emtotalmenteacotados.Rmd-->

# Equicontinuidad

<!--chapter:end:2017-equicontinuidad.Rmd-->

# El teorema de Stone-Weierstrass

<!--chapter:end:2018-stoneweierstrass.Rmd-->

# Espacios toplógicos localmente compactos

## Propiedades generales

## Funciones a soporte compacto

## Funciones que se anulan al infinito

## Compactificación a un punto

<!--chapter:end:2019-etlocalmentecompactos.Rmd-->

# Espacios de Hilbert

## Definición y ejemplos

## Ortogonalidad

## Separación de conjuntos convexos

## Bases ortonormadas

## Convergencia débil

## Operadores contínuos y compactos

## Teorema espectral de Hilbert

<!--chapter:end:202-diferenciacionRn.Rmd-->

# Espacio de funciones diferenciables

<!--chapter:end:2020-funcionesdiferenciables.Rmd-->

# Particiones de la unidad

<!--chapter:end:2021-particiondelaunidad.Rmd-->


# Conexidad

Placeholder



<!--chapter:end:2023-conexidad.Rmd-->

# Espacios de Banach

## Espacios normados

## Separación de conjuntos convexos

## Teorema de prolongamiento

## Duales de los espacios $\ell^p$

## Convergencia débil

## Teorema de Banach-Steinhaus

## Espacios reflexivos

## Operadores contínuos y compactos

## Teorema de Fredholm-Riesz

## Aplicaciones abiertos y grafos cerrados

## Caso complejo

<!--chapter:end:203-medidadelebesgueRn.Rmd-->

# Espacios convexos

## Familias de seminormas

## Teorema de separación y de prolongamiento

## Teorema de Krein-Milman

<!--chapter:end:204-integracionlebesgueRn.Rmd-->


<!--chapter:end:205-curvasysuperficiesRn.Rmd-->


<!--chapter:end:206-integracionensuperficies.Rmd-->

# Conjuntos medibles

## Introducción

## Espacios medibles

## Medidas

## Espacios medibles completos

## Medida externa y medibilidad

## Extensión de una medida

## Medida de Lebesgue

## Medida de Lebesgue Stieltjes

## Conjuntos especiales

<!--chapter:end:301-conjuntosmedibles.Rmd-->

# Funciones medibles

## Transformaciones medibles

## Funciones numéricas medibles

## Funciones simples

## Convergencia de funciones medibles

<!--chapter:end:302-funcionesmedibles.Rmd-->

# Integración

## Construcción de la integral

## Propiedades básicas de la integral

## Conexión con la integral de Riemann en $\mathbb{R}^n$

## Teoremas de convergencia

## Integración sobre una medida producto

## Aplicaciones del teorema de Fubini


<!--chapter:end:303-integracion.Rmd-->

# Espacios $L^p$

## Definición y propiedades generales

## Aproximación en $L^p$

## Convergencia en $L^p$

## Integrabilidad uniforme

## Funciones convexas y desigualdad de Jensen

<!--chapter:end:304-espaciosLp.Rmd-->

# Diferenciación

## Medidas con signo

## Medidas complejas

## Continuidad absoluta de medidas

## Diferenciación de medidas

## Funciones a variación acotada

## Funciones absolutamente contínuas

<!--chapter:end:305-diferenciacion.Rmd-->

# Análisis de Fourier en $\mathbb{R}^n$

## Convolución de funciones

## La transformada de Fourier

## Funciones de rápido decrecimiento

## Análisis de Fourier de medidas en $\mathbb{R}^n$


<!--chapter:end:306-analisidefourier.Rmd-->

# Medidas en espacios localmente compactos

## Medidas de Radon

## El teorema de representación de Riesz

## Productos de medidas de Radon

## El operador dual

## Operadores compactos

<!--chapter:end:307-medidaesploccompactos.Rmd-->

# Espacios localmente convexos

## Propiedades generales

## Funcionales lineales contínuos

## Teoremas de separación de Hahn-Banach

## Algunas construcciones

<!--chapter:end:308-espacioslocconvexos.Rmd-->

# Topologías débiles en espacios normados

## Topología débil

## Topología débil$^*$

## Espacios reflexivos

## Espacios uniformemente convexos

<!--chapter:end:309-topdebespnormados.Rmd-->

# Espacios de Hilbert

## Principios generales

## Ortogonalidad

## Bases ortonormales

## El adjunto del espacio de Hilbert


<!--chapter:end:310-esphilbert.Rmd-->

# Teoría de operadores

## Tipos de operadores

## Operadores compactos y de rango finito

## El teorema espectral para operadores normales compactos

## El álgebra del grupo $L^1$

## Representaciones

## Grupos abelianos localmente compactos

<!--chapter:end:311-teoriadeoperadores.Rmd-->

# Análisis en semigrupos

## Semigrupos con topologías

## Funciones debilmente casi periódicas

## La estructura de los semigrupos compactos

## Funciones fuertemente casi periódicas 

## Semigrupo de operadores

<!--chapter:end:312-analisisdesemigrupos.Rmd-->

# Teoría de probabilidades

##Conjuntos y funciones $\sigma$-aditivas}

Sea un conjunto $\Omega$, y sea $\mathcal{A}$ una $\sigma$-álgebra
sobre $\Omega$. Se dice que $\mathcal{A}$ es una $\sigma$-álgebra si
cumple las siguientes propiedades:
\begin{enumerate}
\item $\Omega \in \mathcal{A}$
\item Si $A \in \mathcal{A} \Rightarrow \overline{A} \in \mathcal{A}$
\item Si $A_1, A_2, A_3\ldots \in \mathcal{A} \Rightarrow
\displaystyle \bigcup_{n \in \mathbb{N}}^{\infty} A_n \in \mathcal{A}$
\end{enumerate}
Es decir, una $\sigma$-álgebra es una clase de conjuntos cerrada para
las operaciones complementario y unión numerable. Existen una serie de
propiedades inmediatas derivadas de las propiedades que definen a la
$\sigma$-álgebra:\\
$\emptyset \in \mathcal{A}$\\
$\mathcal{A}$ es cerrada para la operación intersección numerable.
\subsection*{Espacio medible}
Al par ($\Omega$, $\mathcal{A}$) se le llama espacio medible, y a los
conjuntos que pertenecen a $\mathcal{A}$ se les denomina conjuntos
medibles.
\section{Límites en sucesiones de conjuntos}
\subsection{Límites en sucesiones monótonas}
Si tomamos la relación de inclusión entre conjuntos ($\subseteq$) como
una relación de orden, podemos hablar sin ambiguedad de
sucesiones monótonas. En este sentido, una sucesión creciente de
conjuntos es una sucesión $\{A_n\}_{n \in \mathbb{N}}$ en la que se
cumple que $A_i \subseteq A_{i+1}, \forall i \in \mathbb{N}$. De forma
análoga se puede definir sucesión decreciente de conjuntos.\\
Existe una forma intuitiva de definir el límite de una
sucesión monótona de conjuntos. En particular, el límite de una
sucesión creciente de conjuntos $\{A_n\}_{n \in \mathbb{N} }$ se puede
definir como
$$\lim_{n\to\infty} A_n = \bigcup_{k \in \mathbb{N}}^{\infty} A_k$$
Esta definición aprovecha la relación de orden entre los conjuntos de
la sucesión para afirmar que si un elemento está en el último
conjunto de la sucesión, entonces está en todos los anteriores, y por
tanto en todos, por ello se puede utilizar una intersección
numerable (que está bien definida) para formalizar el
concepto.\\
Con una intuición análoga se define el límite de una sucesión
decreciente de conjuntos. Si $\{A_n\}_{n\in\mathbb{N}}$ es una
sucesión decreciente de conjuntos, entonces:
$$ \lim_{n\to\infty} A_n = \bigcap_{k\in\mathbb{N}}^{\infty} A_k $$
\subsection{Límites superiores e inferiores}
No solo se puede hablar de límites en sucesiones monótonas. Para
definir los límites en sucesiones arbitrarias de conjuntos tenemos que
recurrir a los conceptos de límite inferior y límite superior. La
intuición de estos límites superior e inferior pasan por el concepto
de las colas de la sucesión.\\
Dada una sucesión de conjuntos $\{A_n\}_{n\in\mathbb{N} }$ podemos
considerar el conjunto
$$ B_n = \bigcap_{k=n}^{\infty} A_k $$
y este conjunto contiene aquellos elementos que están en
\textbf{todos} los $A_k$ para $k \geq n$. Es fácil probar que la
sucesión $\{B_n\}_{n\in\mathbb{N}}$ es una sucesión creciente de
conjuntos, y por tanto se puede obtener el límite $\lim_{n\to\infty}
B_n$. Informalmente, ese límite es un conjunto que contiene a todos
los elementos de $A_n$ que están en todos los conjuntos $A_k$ a partir
de cierto $n\in\mathbb{N}$. Definimos el límite inferior de $A_n$ como
$$ \liminf A_n = \lim_{n\to\infty} B_n = \bigcup_{n\in\mathbb{N}}
\bigcap_{k=n}^{\infty} A_n $$
Análogamente, podríamos definir la sucesión de conjuntos
$\{C_n\}_{n\in\mathbb{N}}$ como
$$ C_n = \bigcup_{k=n}^{\infty} A_n $$
Cada $C_n$ contiene todos los elementos que están presentes en algún
$A_k$ para $k \geq n$. Es fácil también ver que la sucesión
$\{C_n\}_{n\in\mathbb{N}}$ es una sucesión decreciente de conjuntos, y
por tanto su límite también está bien definido. Se puede definir
entonces el límite superior de $\{A_n\}_{n\in\mathbb{N}}$ como
$$ \limsup A_n = \lim_{n\to\infty} C_n = \bigcap_{n\in\mathbb{N}}
\bigcup_{k=n}^{\infty} A_n $$
Informalmente se puede pensar en este límite superior de $A_n$ como el
conjunto de los elementos que están en infinitos conjuntos de la
sucesión.\\
A partir de estas definiciones, es fácil comprobar que
$$ \liminf A_n \subseteq \limsup A_n $$
\subsection{Límite de una sucesión de conjuntos}
Diremos que una sucesión de conjuntos tiene límite si su límite
inferior y superior coinciden, y el límite tendrá como valor
efectivamente el de estos límites. Es decir:
$$ \lim A_n = \liminf A_n = \limsup A_n $$
en caso de que límite superior e inferior coincidan.
\section{Funciones sobre conjuntos}
Una vez definidos los conceptos sobre conjuntos con los que vamos a
trabajar, pasamos a definir las funciones sobre conjuntos. Vamos
entonces a definir lo que es una función de conjunto. Sean los
espacios medibles ($\Omega$, $\mathcal{A}$) y($\Omega'$,
$\mathcal{A}'$), definimos la función:
$$ X: \mathcal{A} \to \mathcal{A}'$$
$$ A \longrightarrow X(A)$$
A raíz de esta definición podemos definir también lo que se conoce
como función inversa. Dada una función $X$, la función inversa de $X$,
$X^{-1}$, asigna a cada conjunto $A' \in \mathcal{A}'$ el conjunto $A
\in \mathcal{A}$ tal que $X(A) = A'$. La propiedad básica que cumplen
las funciones inversas es que preservan las operaciones e inclusiones
de conjuntos.
\section{Concepto de $\sigma$-aditividad}
Sea un conjunto $\Omega$ y una $\sigma$-álgebra $\mathcal{A}$ sobre
$\Omega$. Definimos la función de conjunto:
$$\varphi : \mathcal{A} \rightarrow \mathbb{R}$$
\begin{center}
$\varphi (A)$ es único\\
\end{center}
Se dice que $\varphi$ es aditiva si
$\varphi(\displaystyle\sum_{1}^{n}A_k)=\displaystyle\sum_1^n\varphi(A_k)$\\
Se dice que $\varphi$ es $\sigma$-aditiva si
$\varphi(\displaystyle\sum_1^\infty A_k)=\displaystyle\sum_1^\infty
\varphi(A_k)$
\subsubsection{Función subaditiva}
Sea $\varphi$ definida como antes. Se dice que $\varphi$ es
\textbf{subaditiva} si $\varphi(A \cup B) \leq \varphi(A) +
\varphi(B)$
\begin{lemma}
Si $\exists B\, : \, \varphi(B)<\infty \Rightarrow \varphi(\emptyset)=0$
\end{lemma}
\begin{theorem}
Si $\varphi$ es $\sigma$-aditiva y
$\displaystyle\sum\varphi(A_i)<\infty\Rightarrow\displaystyle\sum(\vert
\varphi(A_i)\vert)<\infty$
\end{theorem}
\begin{proof}
Tomemos las sucesiones: \\
Si $\varphi(A_n)\geq 0 \Longrightarrow A_n^{+}=A_n$ y $A_n^{-}=\emptyset$\\
Si $\varphi(A_n)<0 \Longrightarrow A_n^{+}=\emptyset$ y $A_n^{-}=A_n$\\
Entonces $\varphi(\displaystyle\sum
A_n^{+})=\displaystyle\sum\varphi(A_n^{+})$ y
$\varphi(\displaystyle\sum
A_n^{-})=\displaystyle\sum\varphi(A_n^{-})$, ambas finitas. Sumando
ambas cantidades obtenemos que $\displaystyle\sum(\vert
\varphi(A_i)\vert)<\infty$
\qed
\end{proof}
\begin{theorem}
Si $\varphi$ es $\sigma$-aditiva, $\varphi \geq 0$, entonces:
$\varphi$ es no decreciente y subaditiva
\end{theorem}
\begin{proof}
Veamos que es no decreciente $(A \subseteq B \Rightarrow \varphi (A)
\leq \varphi (B))$. Podemos escribir $B = (B \cap A) + (B \cap
\overline{A}) = A + (B \cap \overline{A})$. Entonces $\varphi (A) \leq
\varphi (A) + \varphi (B \cap \overline{A}) = \varphi (B)$.\\
\end{proof}
\section{Continuidad en funciones sobre conjuntos}
Una vez introducido el concepto de límite para una sucesión de
conjuntos, vamos a tratar de definir la continuidad para funciones de
conjunto. Tendremos tres tipos de continuidad, cada uno relacionado
con un tipo de sucesiones de conjuntos de las que hemos definido
anteriormente. En esta sección trabajaremos con una función $\varphi :
\Omega \to \Omega'$\\
Diremos que $\varphi$ es continua por abajo si cumple que, dada una
sucesión creciente de elementos $A_n \uparrow A$, se tiene que
$$ \lim \varphi (A_n) = \varphi (A) $$
Por otra parte, diremos que $\varphi$ es continua por arriba si cumple
que dada una sucesión decreciente de elementos $A_n \downarrow A$, se
tiene que
$$ \lim \varphi (A_n) = \varphi (A)$$
Por último, diremos que una función es continua si lo es por arriba y por abajo.
\begin{theorem}
Teorema de continuidad para funciones sobre conjuntos\\
Sea $\varphi$ una función $\sigma$-aditiva. Entonces, $\varphi$ es
aditiva y continua. Inversamente, si $\varphi$ es aditiva y, o bien
continua por abajo, o finita y continua en $\emptyset$, entonces
$\varphi$ es $\sigma$-aditiva.
\end{theorem}
\begin{proof}
Por un lado, sea $\varphi$ una función $\sigma$-aditiva. Entonces es
trivialmente aditiva. Ahora, veamos que es continua por abajo y por
arriba. Sea $A_n \uparrow A$, entonces:
$$ A = \lim A_n = \bigcup A_n = A_1 + (A_2 - A_1) + (A_3 - A_2) +... $$
Unión de conjuntos disjuntos. Por tanto:
$$ \varphi (A) = \varphi (\lim A_n) = \lim_{n \to \infty } \{ \varphi
(A_1) + \varphi (A_2 - A_1) + ... + \varphi (A_n - A_{n-1}) \} = \lim
\varphi (A_n) $$
Veamos la continuidad por arriba. Sea $A_n \downarrow A$, tomamos
$A_{n_0}$ tal que $\varphi (A_{n_0})$ es finito. Entonces $A_{n_0} -
A_n \uparrow A_{n_0} - A$, y por el apartado anterior tenemos la
convergencia desde abajo, por tanto:
$$ \varphi (A_{n_0}) - \varphi (A) = \varphi (\lim (A_{n_0} - A_n)) =
\lim \varphi (A_{n_0} - A_n) = \varphi (A_{n_0}) - \lim \varphi (A_n)
$$

Asi, se deduce que $ \varphi (A) = \lim \varphi (A_n) $.\\
Inversamente, sea $ \varphi$ una función aditiva. Si $\varphi$ es
continua por abajo, tenemos
$$ \varphi \left( \sum_{n}^{\infty} A_n \right) = \varphi \left( \lim
\sum_{k=1}^n A_k \right) = \lim \varphi \left( \sum_{k=1}^n A_k
\right) = \lim \sum_{k=1}^n \varphi \left( A_k \right) =
\sum_{n}^{\infty} \varphi (A_n) $$
Y por tanto es $\sigma$-aditiva. Si es finita y continua en
$\emptyset$, entonces se obtiene la $\sigma$-aditividad de:
$$ \varphi \left( \sum_{n}^{\infty} A_n \right) = \varphi \left(
\sum_{k=1}^{n} A_k \right) + \varphi \left( \sum_{k=n+1}^{\infty} A_k
\right) = \sum_{k=1}^{n} \varphi (A_k) + \varphi \left(
\sum_{k=n+1}^{\infty} A_k \right) $$
Y tenemos que
$$ \varphi \left( \sum_{k=n+1}^{\infty} A_k \right) \to \varphi
(\emptyset) = 0 $$
\qed
\end{proof}
Una vez demostrado este teorema, vamos a ver un teorema que nos
relaciona las propiedades del supremo e ínfimo de una función
$\sigma$-aditiva con los conjuntos sobre los que está dicha función
definida:
\begin{theorem}
Teorema del supremo e ínfimo\\
Sea $\varphi$ una función $\sigma$-aditiva sobre una $\sigma$-álgebra
$\mathcal{A}$. Entonces, existen $C,D \in \mathcal{A}$ tales que
$\varphi (C) = \sup \varphi$ y $\varphi (D) = \inf \varphi$
\end{theorem}
\begin{proof}
Probaremos la existencia del conjunto $C$. La del conjunto $D$ es
análoga. Si $\varphi(A) = \infty$ para algún $A \in \mathcal{A}$,
entonces podemos establecer $A = C$ y la demostración del teorema es
trivial. Entonces, supongamos que $\varphi < \infty$ y dado que el
valor $-\infty$ está excluido, $\varphi$ es finita.\\
Entonces, existe una sucesión $\{A_n\} \subset \mathcal{A}$ tal que
$\varphi(A_n) \to \sup \varphi$. Sea $A = \cup A_n $ y para cada $n$,
consideramos la partición de $A$ en $2^n$ conjuntos $A_{nm}$ de la
forma $\displaystyle \cap_{k=1}^n A'_k$, donde $A'_k = A_k$ o $A -
A_k$. Para $n < n'$, cada conjunto $A_{nm}$ es una suma finita de
conjuntos $A_{n'm'}$. Sea ahora $B_n$ la suma de los conjuntos
$A_{nm}$ para los cuales $\varphi$ es no negativa. Si no hay ninguno,
entonces $B_n = \emptyset$. Entonces, tenemos por un lado que $A_n$ es
la suma de algunos de los $A_{nm}$, y por otro lado, para $n' > n$,
cada conjunto $A_{n'm'}$ está dentro de $B_n$ o son disjuntos.
Entonces tenemos
$$ \varphi(A_n) \leq \varphi(B_n) \leq \varphi (B_n \cup B_{n+1} \cup
... \cup B_{n'}) $$
Tomando $n' \to +\infty$, se sigue de la continuidad por debajo que
$$ \varphi(A_n) \leq \varphi (B_n) \leq \varphi \left(
\cup_{k=n}^{+\infty} B_k\right) $$
Haciendo tender ahora $n \to +\infty$ y tomando $\displaystyle C =
\lim \cup_{k = n}^{+\infty} B_k$ se sigue, por la continuidad por
arriba, que $\sup \varphi \leq \varphi(C)$. Pero $\varphi(C) \leq \sup
\varphi$, y por tanto se tiene que $\varphi(C) = \sup \varphi$, como
queríamos.
\qed
\end{proof}
\chapter{Medidas y probabilidades}
\section{Concepto de medida, media exterior y probabilidad}
Una función de conjuntos $\mu^\circ$ es una medida si verifica:
\begin{itemize}
\item Es $\sigma$-aditiva, es decir,  $\mu^\circ (\cup A_j) =
\displaystyle \sum \mu^\circ (A_j)$
\item Es no decreciente $A\subset B \, \mu^\circ(A)\leq \mu^\circ(B)$
\item $\mu^\circ(\emptyset)=0$
\end{itemize}
A la tupla ($\Omega$, $\mathcal{A}$, $\mu_{\mathcal{A}}$) se le
denomina espacio de medida.\\
\textbf{Definición de medida exterior:} Una medida exterior es una
función de conjuntos positiva y $\sigma$-subaditiva, es decir, no se
cumple la primera propiedad. La $\sigma$-subaditividad implica que
$\mu(A \cup B) \leq \mu(A) + \mu(B)$.\\
Para que una medida exterior fuera una medida tendría que ser
$\sigma$-aditiva. Es decir, la falla la primera condición. Sí que es
positiva ya que $\mu^\circ(\emptyset)=0$ y es creciente. Esta medida
exterior se aplica a cualquier conjunto. Va a haber unos subconjuntos
en los que la función se comporte como si fuera aditiva.\\
Una vez definido el concepto de medida, vamos a dar ahora el de
probabilidad. Una probabilidad $\mathcal{P}$ sobre un espacio medible
($\Omega$, $\mathcal{A}$) es una medida que además cumple que
$\mathcal{P}(\Omega)=1$. Por tanto, tiene las siguientes
propiedades:\\
$\mathcal{P}(\emptyset)=0$\\
$\forall A \in \mathcal{A}, 0 \leq \mathcal{P}(A) \leq 1$\\
Es una función $\sigma$-aditiva\\
De forma análoga al concepto de espacio de medida, podemos definir
ahora el de espacio probabilístico. Un espacio probabilístico es una
tupla formada por un conjunto $\Omega$, una $\sigma$-álgebra sobre ese
conjunto, $\mathcal{A}$, y una función de probabilidad $\mathcal{P}$.
\begin{theorem}
Teorema de sucesión
\begin{enumerate}
\item Si $A_n \uparrow A \Rightarrow \mathcal{P} (A_n) \uparrow \mathcal{P}(A)$
\item $\mathcal{P}(\lim \inf A_n) \leq \lim \inf \mathcal{P}(A_n)$
\item Si $A_n \downarrow A \Rightarrow \mathcal{P} (A_n) \downarrow
\mathcal{P}(A)$
\item $\mathcal{P}(\lim \sup A_n) \geq \lim \sup \mathcal{P}(A_n)$
\item Si $A_n \rightarrow A \Rightarrow \mathcal{P} (A_n) \rightarrow
\mathcal{P}(A)$
\end{enumerate}
\end{theorem}
\begin{proof}
Falta! 
\end{proof}
\section{Teorema de extensión de Carathéodory}
Una vez vistas las definiciones anteriores de medida y medida
exterior, vamos a ver un teorema fundamental, que nos servirá para
justificar la forma en la que haremos el cálculo de probabilidades a
posteriori. Veamos dos lemas antes que nos serán necesarios para la
demostración del teorema principal.\\
\textbf{Definición:} Un conjunto $A\in S(\Omega)$ es
$\mu^\circ$-medible si se cumple que $\mu^\circ(D) \geq
\mu^\circ(AD)+\mu^\circ(A^cD), \forall D \in S(\Omega)$\\
\textbf{Definición:} Una extensión exterior $\mu^\circ$ de una medida
$\mu$ se define como:
$$\mu^\circ (A) = \inf \sum_j (A_j), \quad A \subset \cup A_j,\quad
recubrimiento $$
\begin{theorem}
La extensión exterior $\mu^\circ$ de una medida $\mu$ sobre un álgebra
es una extensión de $\mu$ a una medida exterior
\end{theorem}
\begin{proof}
Primero, veamos que es una extensión. Esto es trivial, dado que
$\mu^\circ(A) = \inf \displaystyle \sum \mu(A) = \mu(A)$. Ahora,
veamos que es una medida exterior.\\
Veamos que es subaditiva, es decir, $\mu^\circ(\displaystyle \cup_j
A_j) \leq \sum_j \mu^\circ(A_j)$. Sea entonces, para cada $A_j$, un
recubrimiento $ \displaystyle \cup_k A_{kj} \supset A_j$. Entonces:
$$ \sum_k \mu (A_{kj}) \leq \frac{\varepsilon}{2^j} + \mu^\circ (A_j)$$
$$ \mu^\circ (\cup_j A_j) \leq \sum_{j,k} \mu (A_{kj}) \leq \sum_j
\Big( \mu^\circ(A_j) + \frac{\varepsilon}{2^j}\Big) \leq \sum_j
(\mu^\circ(A_j)) + \varepsilon $$
Claramente es no decreciente, ya que si $A \subseteq B$, todo
recubrimiento de $B$ lo será también de $A$, y por tanto,
$\mu^\circ(A) \leq \mu^\circ(B)$\\
Por último, $\mu^\circ(\emptyset) = \mu(\emptyset) = 0$
\end{proof}
\begin{theorem}
Sea $\mu^\circ$ una medida exterior sobre la $\sigma$-álgebra
$\mathcal{A}$, y sea $\mathcal{A}^\circ$ la clase de conjuntos
$\mu^\circ$-medibles:
\begin{itemize}
\item $\mathcal{A}^\circ$ es un $\sigma$-algebra
\item $\mu^\circ$ en $\mathcal{A}^\circ$ es una medida
\end{itemize}
\end{theorem}
\begin{proof}
Primero, veamos que $\mathcal{A}^\circ$ es un álgebra. Sea $A \in
\mathcal{A}^\circ$, entonces $A^c \in \mathcal{A}^\circ$ dado que la
definición de $\mu^\circ$-medibilidad es simétrica. Sean entonces $A,B
\in \mathcal{A}^\circ$. Entonces:
$$ \mu^\circ(D) = \mu^\circ(AD) + \mu^\circ(A^cD) = $$
$$ = \mu^\circ(ABD) + \mu^\circ(AB^cD) + \mu^\circ(A^cBD) +
\mu^\circ(A^cB^cD) \geq$$
$$ \geq \mu^\circ(ABD) + \mu^\circ (AB^cD \cup A^cBD \cup A^cB^cD) =$$
$$ = \mu^\circ(ABD) + \mu^\circ(AB)^cD$$
Dado entonces que $\mathcal{A}^\circ$ es cerrada bajo la operación
complementario e intersección finita, lo es para la unión finita, así
que nos encontramos ante un álgebra. Veamos ahora que $\mu^\circ$ es
aditiva en $\mathcal{A}^\circ$. Sean $A,B \in \mathcal{A}^\circ$
disjuntos. Entonces:
$$\mu^\circ(A+B) = \mu^\circ((A+B)A) + \mu^\circ((A+B)A^c) =
\mu^\circ(A) + \mu^\circ(B)$$
Y teniendo que $\mu^\circ(A) \geq \mu^\circ(\emptyset) = 0$,
$\mu^\circ$ sobre $\mathcal{A}^\circ$ es una función aditiva y
positiva. Para completar la prueba, veamos que $\mu^\circ$ es
$\sigma$-aditiva. Sean $A_n \in \mathcal{A}^\circ$, $A = \displaystyle
\sum A_n$. Tomamos los conjuntos $B_n = \displaystyle \sum_{k=1}^n A_k
\in \mathcal{A}^\circ$. Tenemos que:
$$ \mu^\circ(D) \geq \mu^\circ (B_nD) + \mu^\circ (B_n^cD) \geq
\sum_{k=1}^n\mu^\circ(A_kD) + \mu^\circ(A^cD) $$
Haciendo $n \to +\infty$
$$\mu^\circ(D) \geq \sum_{n=1}^{+\infty} \mu^\circ(A_nD) +
\mu^\circ(A^cD) \geq \mu^\circ(AD) + \mu^\circ(A^cD)$$
Además queda demostrado que $A \in \mathcal{A}^\circ$, así que tenemos
que $\mathcal{A}^\circ$ es un $\sigma$-algebra.
Por último, tomando $D = A$, tenemos que $\mu^\circ(A) \geq
\displaystyle \sum \mu^\circ(A_n) \Rightarrow \mu^\circ(A) = \sum
\mu^\circ(A_n) \Rightarrow \mu^\circ$ es una medida.
\qed
\end{proof}
\begin{theorem}
de extensión de Carathéodory\\
Dada una medida $\mu$ sobre un álgebra $\mathcal{C}$, existe una
extensión $\mu^\circ$ sobre la $\sigma$-álgebra minimal sobre
$\mathcal{C}$ ($\mathcal{A}(\mathcal{C})$). Además, si $\mu$ es
finita, la extensión es única.
\end{theorem}
\begin{proof}
$\forall A \in \mathcal{C}, \forall D \in \mathcal{C}, \forall
\varepsilon>0, \exists \{A_j\} \subset \mathcal{C}$ recubrimiento de
$D$ tal que
$$\mu^\circ(D) + \varepsilon \geq \sum \mu(A_j) \geq \sum \mu (AA_j) +
\sum \mu (A^cA_j) \geq \mu^\circ(AD) + \mu^\circ(A^cD) \Rightarrow$$
$$ \stackrel{\varepsilon \to 0}{\Rightarrow} \mu^\circ(D) \geq
\mu^\circ(AD) + \mu^\circ(A^cD), A \in \mathcal{A}^\circ \Rightarrow
\mathcal{C} \subseteq \mathcal{A}^\circ, \mathcal{A}(\mathcal{C})
\subseteq \mathcal{A}^\circ $$
Por los dos teoremas que hemos demostrado antes, la restricción
$\mu^\circ$ sobre $\mathcal{A}(\mathcal{C})$ es una extensión de $\mu$
a una medida sobre $\mathcal{A}(\mathcal{C})$. Ahora, veamos que es
única. Para ello, sean $\mu_1, \mu_2$ extensiones de $\mu$. Sea
entonces el conjunto $\mathcal{M} = \{A: \mu_1(A) = \mu_2(A)\}
\Rightarrow \mathcal{C} \subset \mathcal{M}$. Tenemos entonces que:
$$ \Omega \in \mathcal{C} \Rightarrow \Omega \in \mathcal{M}
\Rightarrow \mu_1(\Omega) = \mu_2(\Omega) = \mu(\Omega) < \infty
\Rightarrow \mu_1, \mu_2 \: finitos $$
$$ A \in \mathcal{M} \Rightarrow \mu_1(A^c) = \mu(\Omega) - \mu_1(A) =
\mu(\Omega) - \mu_2(A) = \mu_2(A^c) \Rightarrow A^c \in \mathcal{M} $$
$$ A,B \in \mathcal{M} \Rightarrow \mu_1(A+B) = \mu_1(A) + \mu_1(B) =
\mu_2(A) + \mu_2(B) = \mu_2(A+B) \Rightarrow A+B \in \mathcal{M}$$
Entonces, de momento $\mathcal{M}$ es un algebra.\\
Sean ahora $\{A_n\} \subset \mathcal{M}$ monótona, entonces
$\mu_1(\lim A_n) = \lim \mu_1(A_n) = \lim \mu_2(A_n) = \mu_2(\lim A_n)
\Rightarrow \mathcal{M}$ cerrada frente al límite de sucesiones
monótonas $\Rightarrow \mathcal{M} \sigma$-álgebra que contiene a
$\mathcal{C}$, por tanto, contiene a la $\sigma$-álgebra minimal sobre
$\mathcal{C}$
$$ \mathcal{A}(\mathcal{C}) \subseteq \mathcal{M} \Rightarrow \mu_1 =
\mu_2 \: en \: \mathcal{A}(\mathcal{C})$$
\end{proof}
\chapter{Funciones medibles}
Una vez definidos los conceptos sobre espacios de medida y espacios
probabilísticos, vamos a aproximarnos al concepto de función medible.
Para ello, daremos dos definiciones de función medible, para demostrar
más adelante que estas dos definiciones son equivalentes. Empecemos
con la definición constructiva de función medible. Dado que nos
interesa que el codominio sea $\mathbb{R}$, trabajaremos con funciones
definidas entre un espacio medible ($\Omega$, $\mathcal{A}$) y
($\mathbb{R}$, $\mathcal{B}$), donde $\mathcal{B}$ representa la
$\sigma$-álgebra de Borel.\\
Primero, se define la función puntual $X: \Omega \to \mathbb{R}$, que
asigna a cada $\omega \in \Omega$ un número $x = X(\omega)$ único.
Llamaremos a esta función variable aleatoria. Utilizaremos de aquí en
adelante la siguiente notación:
\begin{itemize}
\item $[X]$ = dominio de la variable aleatoria $X$.
\item $[ X \leq Y] = \{\omega: X(\omega) \leq Y(\omega)\}$
\item $[ X = x] = \{\omega: X(\omega)= x\}$
\end{itemize}
Sea entonces la función $X = \displaystyle \sum_j x_jI_{A_j}$, donde
$A_j$ son conjuntos medibles y $I_{A_j}$ denota la función indicadora
de dicho conjunto. Estas funciones se llaman funciones elementales, y
cuando el número de valores distintos que toma la función $X$ es
finito, se conocen como funciones simples. Entonces, la definición
constructiva de función medible es la que sigue:\\
\textbf{Definición constructiva de función medible:} Una función es
medible si es límite de una sucesión de funciones simples $\{X_n\}$
convergentes.\\
Esta definición que hemos dado es constructiva, y por tanto, nos será
muy útil para la definición constructiva de las integrales. No
obstante, para enunciar y demostrar las propiedades de las funciones
medibles, suele ser más útil la definición descriptiva siguiente:\\
\textbf{Definición descriptiva de función medible:} Sea una función
$\varphi : \mathcal{A} \rightarrow \mathcal{B}$. Se dice que $\varphi$
es medible si $\forall B \in \mathcal{B} \Rightarrow \varphi^{-1}(B)
\in \mathcal{A}$. Es decir, una función se dice medible si la imagen
inversa de todo conjunto medible es medible.\\
No obstante, se puede dar, a raíz de esta, otra definición más económica:\\
Para la definición anterior, es suficiente con exigir la medibilidad
de las imágenes inversas de los elementos de una subclase $\alpha$
para la cual la $\sigma$-álgebra minimal sobre $\alpha$ sea
$\mathcal{B}$\\
Veamos ahora que las dos definiciones que hemos dado son equivalentes.
\begin{theorem} Teorema de medibilidad\\
Las definiciones constructiva y descriptiva de una función medible son
equivalentes, y la clase de funciones medibles es cerrada bajo las
operaciones usuales del análisis.
\end{theorem}
\begin{proof}
Sean $X_n$ funciones medibles en el sentido descriptivo. Entonces
todos los conjuntos de la forma
$$[\inf X_n < x] = \cup [X_n < x], [-X_n < x] = [X_n > -x]$$
son medibles, y por tanto, las funciones
$$\sup X_n = - \inf (-X_n), \lim \inf (X_n) = sup (\inf_{k \geq n} X_k)$$
$$ \lim \sup X_n = - \lim \inf (-X_n)$$
son medibles en el sentido descriptivo. Por un lado, las funciones de
este tipo son claramente cerradas bajo las operaciones de supremo,
ínfimo, y límites. Además, toda función simple es medible en el
sentido descriptivo, ya que todos los conjuntos $[X \leq x] =
\displaystyle \sum_{x_j \leq x} A_j$ son medibles. Entonces, el límite
de sucesiones convergentes de funciones simples son medibles, y por
tanto las funciones medibles en sentido constructivo lo son en sentido
descriptivo.\\
Veamos la otra implicación, es decir, que las funciones medibles en
sentido descriptivo lo son en sentido constructivo. Sea una función
$X$ medible en sentido descriptivo. Entonces, las funciones
$$X_n = -nI_{[X < n]} +
\sum_{-n2^n+1}^{n2^n}\frac{k-1}{2^n}I_{\big[\frac{k-1}{2^n} \leq X <
\frac{k}{2^n} \big]} + nI_{X \geq n}, n \in \mathbb{N}$$
son simples. Entonces, dado que
$$\mid X_n(\omega) - X(\omega)\mid < \frac{1}{2^n} \quad para \quad
\mid X(\omega)\mid < n$$
y
$$X_n(\omega) = \pm n \quad para \quad  X(\omega) = \pm \infty$$
se tiene entonces que $X_n \to X$ y esto, con lo anterior, prueba la
equivalencia de las dos definiciones de función medible.\qed
\end{proof}
\begin{lemma}
Sea $X:A\longrightarrow B$\\
$X$ es medible $\Longleftrightarrow$ $X^{-1}(S)\in A,S \in B$
\end{lemma}
\begin{theorem}
Sea $X:\Omega \longrightarrow \mathbb{R}$, y $g: \mathbb{R}
\longrightarrow \mathbb{R}$ continua. Entonces,$ g(X)$ es medible
\end{theorem}
\begin{proof}
Si $X$ es elemental, tenemos que $\displaystyle g(X) =
g\Big(\sum_jx_jI_{A_j}\Big)= \sum_j g(x_j)I_{A_j}$ función elemental,
y por tanto, medible.\\
Si $X$ es el límite de funciones elementales:
$$g(X) = g(\lim X_n) = \lim g(X_n) = \lim \sum_j g(x_j)I_{A_j}$$
\qed
\end{proof}
\begin{theorem}
Sean $X$ función medible y $g$ función boreliana. Entonces, $g(X)$ es medible.
\end{theorem}
\begin{proof}
$$(gX)^{-1}(B)=X^{-1}(g^{-1}(B))\in \mathcal{A}$$
\qed
\end{proof}
\section{Convergencia en probabilidad y convergencia casi segura}
Vamos a establecer ahora criterios que nos permitan comparar variables
aleatorias. Dado un espacio de probabilidad ($\Omega$, $\mathcal{A}$,
$\mathcal{P}$), se dice que dos variables aleatorias son equivalentes
si:
$$ X\mathcal{R}Y \Leftrightarrow \mathcal{P}[X = Y] = 1$$
Análogamente:
$$X(\omega) = Y(\omega) \forall \omega \in \Omega \setminus \Lambda,
\mathcal{P}(\Lambda) = 0$$
\subsection{Definición de convergencia en probabilidad}
Si $P[|X_n- X| \geq \varepsilon]\rightarrow 0$, entonces se dice que
$X_n\stackrel{\mathbb{P}}{\longrightarrow} X$, es decir, $X_n$
converge en probabilidad a $X$\\
\begin{lemma}
$X_n\stackrel{\mathcal{P}}{\longrightarrow} X \wedge
X_n\stackrel{\mathcal{P}}{\longrightarrow} Y \Longrightarrow
X\mathcal{R}Y$\\
\end{lemma}
\begin{proof}
$$|X-Y |=|X - X_n - Y + X_n | \leq |X_n - X|+| X_n-Y |$$
$$P[|X - Y| \geq \varepsilon] \leq P[|X_n - X | \geq
\frac{\varepsilon}{2} ] + P[| X_n - Y | \geq \frac{\varepsilon}{2}]
\rightarrow 0$$
Y por tanto, $X \mathcal{R} Y$
\qed
\end{proof}
\subsection{Definición de convergencia uniforme en u}
Se dice que una variable aleatoria $X$ converge uniformemente en $u$
si se cumple que $\mathcal{P}[\mid X_{n+u} - X_n \mid \geq
\varepsilon] \to 0$
\begin{lemma}
La convergencia en probabilidad implica la convergencia uniforme
\end{lemma}
\begin{proof}
$$ \mid X_{n+u} - X_n \mid \leq \mid X_{n+u} - X \mid + \mid X - X_n
\mid \Rightarrow$$
$$ \Rightarrow \mathcal{P}[\mid X_{n+u} - X_n \mid \geq \varepsilon]
\leq \mathcal{P}\Big[\mid X_{n+u} - X \mid \geq
\frac{\varepsilon}{2}\Big] + \mathcal{P}\Big[\mid X_{n} - X \mid \geq
\frac{\varepsilon}{2}\Big] \to 0$$
\end{proof}
\subsection{Propiedades}
\begin{enumerate}
\item $ X_n \stackrel{\mathcal{P}}{\longrightarrow} X \wedge Y_n
\stackrel{\mathcal{P}}{\longrightarrow} Y \Longrightarrow X_n + Y_n
\stackrel{\mathcal{P}}{\longrightarrow} X + Y$
\item $X_n \stackrel{\mathcal{P}}{\longrightarrow} X \Longrightarrow
KX_n \stackrel{\mathcal{P}}{\longrightarrow} KX$
\item $X_n \stackrel{\mathcal{P}}{\longrightarrow} K$, entonces ${X_n}^2 \stackrel{\mathcal{P}}{\longrightarrow}
K^2$.\\
Para demostrarlo basta notar que: $ {X_n}^2 - K^2 = (X_n + K) (X_n -K)$
\item $X_n \stackrel{\mathcal{P}}{\longrightarrow} a \wedge Y _n
\stackrel{\mathcal{P}}{\longrightarrow} b \Longrightarrow X_nY_n
\stackrel{\mathcal{P}}{\longrightarrow} a \cdot b$\\
Para demostrarlo tenemos que notar que:
$$X_n Y_n = \dfrac{(X_n + Y_n)^2-(X_n -
Y_n)^2}{4}\stackrel{\mathcal{P}}{\longrightarrow}
\dfrac{(a+b)^2-(a-b)^2}{4}=ab$$
\item $X_n \stackrel{\mathcal{P}}{\longrightarrow} 1 \Longrightarrow
\dfrac{1}{X_n} \stackrel{\mathcal{P}}{\longrightarrow} 1$
\item $X_n \stackrel{\mathcal{P}}{\longrightarrow} a \wedge Y_n
\stackrel{\mathcal{P}}{\longrightarrow} b \Longrightarrow
X_nY_n^{-1}\stackrel{\mathcal{P}}{\longrightarrow} ab^{-1}$
\item $X_n \stackrel{\mathcal{P}}{\longrightarrow} X \wedge
Y_n\stackrel{\mathcal{P}}{\longrightarrow} Y \Longrightarrow
X_nY_n\stackrel{\mathcal{P}}{\longrightarrow} XY$\\
Para demostrarlo basta notar que: $(X_n - X)(Y_n -
Y)\stackrel{\mathcal{P}}{\longrightarrow} 0$ y luego
$X_nY_n-XY_n-X_nY+XY\stackrel{\mathcal{P}}{\longrightarrow} 0$ (Por la
propiedad siguiente)
\item $X_n\stackrel{\mathcal{P}}{\longrightarrow} X$, entonces
$YX_n\stackrel{\mathcal{P}}{\longrightarrow} YX$
\end{enumerate}
\begin{theorem}
Si $X_n\stackrel{\mathcal{P}}{\longrightarrow} X$ y $g(\cdot)$ es
continua, entonces se cumple que:
$$g(X_n)\stackrel{\mathcal{P}}{\longrightarrow} g(X)$$
\end{theorem}
\begin{proof}
$\mathcal{P}[|X| \geq k] < \frac{\varepsilon}{2} \forall \varepsilon >
0, \exists k$. Consideramos el compacto $[-k,k], A = [|X| < k], B =
[|X_n - X| < \delta] \: y \: C = [|g(X_n) - g(X)| < \varepsilon]$.
Tenemos que ver si $\mathcal{P}(B)\to 1 \Rightarrow \mathcal{P}(C)\to
1 $:
$$ AB \subset C \Rightarrow C^c \subset A^c \cup B^c \Rightarrow
\mathcal{P}(C^c) \leq \mathcal{P}(A^c) + \mathcal{P}(B^c) \leq $$
$$ \leq \mathcal{P}[|X| \geq k] + \mathcal{P}[|X_n - X| \geq \delta]
\leq \frac{\varepsilon}{2} + \frac{\varepsilon}{2} = \varepsilon$$
\end{proof}
\subsection{Definición de convergencia casi segura}
Una sucesión de variables aleatorias, ${ X_n }$ , converge con
probabilidad 1, o de forma casi segura, a una variable aleatoria $X$ (
que puede degenerar en una constante K) cuando se cumple que:
$$P(\lim_{n\rightarrow\infty}X_n=X)=1$$
De esta forma interpretamos que $X_n\stackrel{c.s}{\longrightarrow}X$
cuando la probabilidad de que en el límite la sucesión de variables
aleatorias y aquella a la que converge sean iguales es uno
\begin{theorem}
$$X_n\stackrel{c.s}{\longrightarrow}X\Longrightarrow
X_n\stackrel{\mathcal{P}}{\longrightarrow}X$$
$$X_n\stackrel{\mathcal{P}}{\longrightarrow}X\Longrightarrow \exists
X_{nk}\,:\, X_{n_k}\stackrel{c.s}{\longrightarrow}_{k\rightarrow\infty}X$$
\end{theorem}
\begin{proof}
$$0=\displaystyle\lim_{n\rightarrow\infty}P\bigcup_{m\geq n}[|X_m -
X|\geq \epsilon ]\geq\displaystyle\lim_{n\rightarrow\infty}P[|X_n -
X|\geq \epsilon ]$$
\qed
\end{proof}
\begin{lemma}
Sea $\mathbb{X}_n$ finita. Entonces se tiene que:
\\\\
$\mathbb{X}_n \stackrel{c.s.}{\longrightarrow}\mathbb{X}\Longleftrightarrow
\mathbb{X}_n$ es de cauchy
\end{lemma}
\begin{proof}
$$\Longrightarrow$$
$\exists n_0\, : \, \forall n\geq n_0$ se tiene que:
$$|\mathbb{X}_n(\omega)-\mathbb{X}(\omega)|<\frac{\epsilon}{2}\,
\omega \in A \, P(A)=1$$
$$|\mathbb{X}_n(\omega)-\mathbb{X}_m(\omega)|\leq|\mathbb{X}_n(\omega)-\mathbb{X}(\omega)|+|\mathbb{X}_m(\omega)-\mathbb{X}(\omega)|<\epsilon$$
$$\Longleftarrow$$
\begin{center}
${\mathbb{X}_n(\omega)}$ de Cauchy
\end{center}
$$\lim\mathbb{X}_n(\omega)=\mathbb{X}(\omega)\, \omega \in A$$
\qed
\end{proof}
\chapter{Esperanza matemática}
\section{Integral de una función de conjunto}
Para el cálculo de probabilidades, nos será muy útil el concepto de
integral sobre funciones de conjunto. Este concepto nos servirá para
calcular lo que se conoce como la esperanza matemática de una variable
aleatoria $X$. En este apartado trabajaremos sobre el espacio de
probabilidad $(\Omega, \mathcal{A}, \mathcal{P})$. Comenzaremos
definiendo la integral para las funciones simples, para dar luego una
definición de integral para funciones no negativas y por último para
funciones cualesquiera.\\
Sea entonces $\{A_k\} \in \mathcal{A}$, tal que $\displaystyle \sum_k
A_k = \Omega$, partición medible del espacio. Sea entonces la función
simple $X = \displaystyle \sum_{j=1}^m x_jI_{A_j}, x_j \geq 0$. La
integral de la función $X$ se define como:
$$\int_{\Omega} X d\mathcal{P} = \sum_{j=1}^m x_j\mathcal{P}_{A_j}$$
Ahora, para cualquier función no negativa $X$, se define la integral
de la función como:
$$\int_{\Omega} X d\mathcal{P} = \lim \int_{\Omega}X_n d \mathcal{P}$$
Donde $\{X_{n}\} \to X$. Finalmente, la integral en $\Omega$ de una
función medible $X$ se define como:
$$\int_{\Omega} X d\mathcal{P} = \int_{\Omega}X^{+} d\mathcal{P} -
\int_{\Omega} X^{-} d\mathcal{P}$$
donde $X^{+} = XI_{[X\geq0]}$ y $X^{-} = -XI_{[X<0]}$. Si
$\displaystyle \int_{\Omega}Xd\mathcal{P}$ es finita, es decir, si los
dos términos de la diferencia anterior son finitos, entonces se dice
que $X$ es integrable en $\Omega$. Ahora, una vez definida la
integral, vamos a ver algunas de sus propiedades. Tenemos primero una
serie de propiedades relacionadas con la aditividad de la integral.
Sean $X,Y$ dos funciones medibles, entonces (no se demostrarán las
propiedades triviales):\\
$\displaystyle \int (X+Y)d\mathcal{P} = \int Xd\mathcal{P} + \int
Yd\mathcal{P}$\\
\begin{proof}
Sean $X = \displaystyle \sum x_jI_{A_j}$ y $y = \displaystyle \sum
y_kI_{B_k}$. Entonces $X+Y = \displaystyle \sum_k \sum_j x_j
I_{A_jB_k} + \sum_k \sum_j y_k I_{A_jB_k} = \sum_k \sum_j (x_k+y_j)
I_{A_jB_k}$\\
Si calculamos ahora las integrales:
$$ \int (X+Y)d\mathcal{P} = \sum_k + \sum_j (x_j + y_k) \mathcal{P}(A_jB_k) =$$
$$ = \sum_j x_j \mathcal{P}(A_j) + \sum_k y_k \mathcal{P}(B_k) = \int
Xd\mathcal{P} + \int Yd\mathcal{P}\\$$
\qed
\end{proof}
$\displaystyle \int_{A+B} X d\mathcal{P} = \int_A X d\mathcal{P} +
\int_B X d \mathcal{P}$\\
$\displaystyle \int cXd\mathcal{P} = c\int Xd\mathcal{P}$\\
Veamos ahora algunas propiedades relacionadas con el orden:\\
$X \geq 0 \rightarrow \displaystyle \int X d\mathcal{P} \geq \int 0 = 0$\\
$X \geq Y \rightarrow \displaystyle \int X d\mathcal{P} \geq \int Y
d\mathcal{P}$\\
$\displaystyle X \stackrel{c.s}{=} Y \rightarrow \int X d\mathcal{P} =
\int Y d\mathcal{P}$\\
\section{Esperanza matemática}
\subsection{Definición general}
Dado un espacio probabilístico $(\Omega, \mathcal{A}, P)$ y una v.a.
$X$, se define la esperanza matemática de $X$ como:
$$E(X)=\int_{\Omega}XdP=\int_{\omega \in \Omega}{X(\omega)dP(\omega)}$$
\\\\
La esperanza matemática se define de forma distinta si estamos
trabajando con una v.a. discreta o continua. En el caso de una v.a.
discreta, sea $p(x_i)$ su función de probabilidad. Definimos la
esperanza matemática como:
$$E(X)=x_1p(X=x_1)+\ldots + x_n p(X=x_n)=\sum_{i=1}^{n}{x_i p(x_i)}$$
En el caso de una v.a. continua, sea $f(x)$ la función de densidad.
Definimos la esperanza matemática como:
$$E(X)=\int_{-\infty}^{+\infty} {xf(x)dx}$$
\subsection{Teorema de la convergencia monótona}
Una vez vista la definición de integral y esperanza matemática y
algunas de sus propiedades, vamos a enunciar y demostrar un teorema de
convergencia que nos será de mucha utilidad para el estudio de
variables aleatorias. Veamos su enunciado y demostración:
\begin{theorem}
Teorema de la convergencia monótona para funciones medibles no negativas\\
Sea $\{X_n\} \geq 0$ tal que $X_n \uparrow X$. Entonces, se tiene que
$\displaystyle \int X_n \uparrow \int X$
\end{theorem}
\begin{proof}
Tomamos las sucesiones $X_{km} \uparrow X_k$. La sucesión $Y_n =
\displaystyle \max_{k \geq n} X_{kn}$ es una sucesión de funciones
simples no negativas y no decreciente, y además
$$X_{kn} \leq Y_n \leq X_n \rightarrow \int X_{kn} \leq \int Y_n \leq \int X_n$$
Ahora, cuando $n \rightarrow \infty$, tenemos que
$$X_k \leq lim Y_n \leq X \rightarrow \int X_k \leq \int lim Y_n \leq \int X$$
Por último, cuando $K \rightarrow \infty$, obtenemos
$$X \leq lim Y_n \leq X \rightarrow lim \int X_n \leq \int lim Y_n
\leq lim \int X_n$$
De donde extraemos que $\lim Y_n = X$ y que $\displaystyle \int X =
lim \int X_n$
\qed
\end{proof}
\subsection{Teorema de Fatou-Lebesgue}
Veamos ahora un resultado que nos da información sobre el límite
superior e inferior de una sucesión de variables aleatorias, en caso
de que estas estén acotadas por variables aleatorias integrables
\begin{theorem}
de Fatou-Lebesgue\\
Sean $Y$, $Z$ dos funciones integrables (pueden no mantener su signo)
y $X_n$ una sucesión de variables aleatorias, entonces:
\begin{enumerate}
\item Si $Y \leq X_n \, \forall n \Longrightarrow$ $E(\lim \inf X_n)
\leq \lim \inf E(X_n)$
\item Si $X_n \leq Z \, \forall n \Longrightarrow E(\lim \sup X_n)\geq
\lim \sup E(X_n)$
\end{enumerate}
\end{theorem}
\begin{proof}
Si $X_n \geq 0$, tenemos que:
$$ X_n \geq Y_n = \inf_{k \geq n} X_n \uparrow \lim \inf X_n
\stackrel{TCM}{=} \lim \inf E(X_n) \geq \lim Y_n = E(\lim \inf X_n)$$
En otro caso:
\begin{enumerate}
\item $X_n - Y \geq 0 \Rightarrow \lim \inf E(X_n) - \lim \inf E(Y)
\geq E(\lim \inf X_n) - E(\lim \inf Y)$
\item $Z - X_n \geq 0 \Rightarrow - \lim \inf E(-X_n) \geq - E(\lim
\inf - X_n) \Rightarrow \lim \sup E(X_n) \leq E(\lim \sup X_n)$
\end{enumerate}
\qed
\end{proof}
\subsection{Teorema de la convergencia dominada}
\begin{theorem}
Sea $X_n$ una sucesión de variables aleatorias t.q.  $X_n
\stackrel{\mathcal{P}}{\rightarrow} X$ o $X_n
\stackrel{c.s.}{\rightarrow} X$  . Si $\exists Y \, t.q. \, |X_n |\leq
Y$. Entonces se tiene que $X$ es integrable y:
$$\lim\int X_n\, dP=\int X\, dP$$
\end{theorem}
\begin{proof}
Por un lado, si tenemos la convergencia casi segura, $|X_n| \leq Y
\Rightarrow -Y \leq X_n \leq Y \stackrel{F-L}{\rightarrow}
\displaystyle \int X_n \to \int X$.
Por otro, si la convergencia es en probabilidad, nos bastaría con
probar que si $Y_n \stackrel{\mathcal{P}}{\rightarrow} 0 \Rightarrow
\displaystyle \int Y_n \stackrel{\mathcal{P}}{\rightarrow} 0$.
Entonces, se considera $Y = |X_n - X|$ y se culmina la demostración.
Entonces:
$$ Y_n \stackrel{\mathcal{P}}{\rightarrow} 0 \Rightarrow \exists
\{Y_n'\} \subset \{Y_n\} \, t.q. \, \int Y_n' \rightarrow \lim \sup
\int Y_n$$
De nuevo, tenemos que $Y_n' \stackrel{\mathcal{P}}{\rightarrow} 0$.
Tomando anora $\{Y_n''\} \subset \{Y_n'\} \, t.q. \, Y_n''
\stackrel{c.s.}{\rightarrow} 0 \rightarrow \displaystyle \int Y_n''
\rightarrow 0 \stackrel{unic.lim.}{\Rightarrow} \lim \sup \int Y_n = 0
\stackrel{Y_n \geq 0}{\Rightarrow} \int Y_n \rightarrow 0$
\qed
\end{proof}


\begin{theorem}
de Fatou-Lebesgue\\

Sean $Y$, $Z$ dos funciones integrables (pueden no mantener su signo)
y $X_n$ una sucesión de variables aleatorias, entonces:
\begin{enumerate}
\item Si $Y \leq X_n \, \forall n \Longrightarrow$ $E(\lim \inf X_n)
\leq \lim \inf E(X_n)$
\item Si $X_n \leq Z \, \forall n \Longrightarrow E(\lim \sup X_n)\geq
\lim \sup E(X_n)$
\end{enumerate}
\end{theorem}

\begin{proof}
Si $X_n \geq 0$, tenemos que:
$$ X_n \geq Y_n = \inf_{k \geq n} X_n \uparrow \lim \inf X_n
\stackrel{TCM}{=} \lim \inf E(X_n) \geq \lim Y_n = E(\lim \inf X_n)$$
En otro caso:
\begin{enumerate}
\item $X_n - Y \geq 0 \Rightarrow \lim \inf E(X_n) - \lim \inf E(Y)
\geq E(\lim \inf X_n) - E(\lim \inf Y)$
\item $Z - X_n \geq 0 \Rightarrow - \lim \inf E(-X_n) \geq - E(\lim
\inf - X_n) \Rightarrow \lim \sup E(X_n) \leq E(\lim \sup X_n)$
\end{enumerate}
\qed
\end{proof}

\subsection{Teorema de la convergencia dominada}
\begin{theorem}
Sea $X_n$ una sucesión de variables aleatorias t.q.  $X_n
\stackrel{\mathcal{P}}{\rightarrow} X$ o $X_n
\stackrel{c.s.}{\rightarrow} X$  . Si $\exists Y \, t.q. \, |X_n |\leq
Y$. Entonces se tiene que $X$ es integrable y:
$$\lim\int X_n\, dP=\int X\, dP$$
\end{theorem}

\begin{proof}
Por un lado, si tenemos la convergencia casi segura, $|X_n| \leq Y
\Rightarrow -Y \leq X_n \leq Y \stackrel{F-L}{\rightarrow}
\displaystyle \int X_n \to \int X$.
Por otro, si la convergencia es en probabilidad, nos bastaría con
probar que si $Y_n \stackrel{\mathcal{P}}{\rightarrow} 0 \Rightarrow
\displaystyle \int Y_n \stackrel{\mathcal{P}}{\rightarrow} 0$.
Entonces, tomaríamos $Y = |X_n - X|$ y tendríamos la demostración.
Entonces:
$$ Y_n \stackrel{\mathcal{P}}{\rightarrow} 0 \Rightarrow \exists
\{Y_n'\} \subset \{Y_n\} \, t.q. \, \int Y_n' \rightarrow \lim \sup
\int Y_n$$
De nuevo, tenemos que $Y_n' \stackrel{\mathcal{P}}{\rightarrow} 0$.
Tomando anora $\{Y_n''\} \subset \{Y_n'\} \, t.q. \, Y_n''
\stackrel{c.s.}{\rightarrow} 0 \rightarrow \displaystyle \int Y_n''
\rightarrow 0 \stackrel{unic.lim.}{\Rightarrow} \lim \sup \int Y_n = 0
\stackrel{Y_n \geq 0}{\Rightarrow} \int Y_n \rightarrow 0$
\qed
\end{proof}

\subsection{Desigualdades}

Vamos a ver algunas desigualdades que nos permitirán
simplificar el cálculo de carácterísticas asociadas a variables
aleatorias.\\

\textbf{Definición: Momento r-ésimo}\\

Dado un espacio probabilístico ($\Omega$, $\mathcal{A}$,
$\mathcal{P}$) y una variable aleatoria $X$, se define el momento
r-ésimo o de orden r de la variable $X$ a:
$$ EX^r = \int X^r \, d \mathcal{P} $$
Dicho momento existe si $E|X|^r < \infty$

\subsubsection{Desigualdad $C_r$}
\begin{lemma}
$|a+b|^r\leq C_r |a|^r + C_r |b|^r$ con $C_r=1$ si $r=1$ y $C_r=2^r$ si $r>1$\\

Entonces se tiene $E|X+Y|^r \leq C_r E|X|^r + C_r E|Y|^r$
\end{lemma}

\subsubsection{Desigualdad de Hölder}
$E|XY| \leq \left(E|X|^r \right)^{\frac{1}{r}}  \left(E|Y|^s
\right)^{\frac{1}{s}}$ con $r>s$ ; $ \dfrac{1}{r}+\dfrac{1}{s}=1$

\subsubsection{Caso particular: Desigualdad de Schwarz}
$E|XY|\leq \left(E|X|^2 \right)^{\frac{1}{2}} \left(E|Y|^2
\right)^{\frac{1}{2}}$

\subsubsection{Desigualdad de Minkowsky}
Si $r \geq 1 \Rightarrow (E|X+X'|^r)^{\frac{1}{r}} \leq \left(E|X|^r
\right)^{\frac{1}{r}} + \left(E|X'|^r \right)^{\frac{1}{r}}$

\subsubsection{Desigualdad básica}
Sea $X$ una v.a. y sea $g$ una función boreliana. Entonces se tiene:

\begin{description}
\item[i)] Si $g$ es par y no decreciente en $[0,\infty) \, \forall
a>0$ , entonces:
$$\dfrac{Eg(X)-g(a)}{sup\, g(X)}\leq P[|X|\geq a]\leq \dfrac{E g(X)}{g(a)}$$
\item[ii)] (Desigualdad de Tchevychev) Si $g$ es no decreciente en $\mathbb{R}$,
$$ P[|X-EX] \geq a] \leq \frac{Var X}{a^2}$$
\item[iii)] (Desigualdad de Markov) Si $g(X) = |X|^r$
$$ \frac{EX^r - a^r}{sup X^r} \leq P[|X| \geq a] \leq \frac{EX^r}{a^r} $$
\end{description}

Vamos a demostrar que en efecto se cumple la desigualdad básica:
\begin{proof}
Definimos $A = [|X| \geq A]$
$$ Eg(A) = \int_A g(X) d\mathcal{P} + \int_{A^c} g(X) d\mathcal{P} $$
$$ g(a)\mathcal{P}(A) \leq \int_A g(X) \leq \sup g(X)\mathcal{P}(A) $$
$$ 0 \leq \int_{A^c} g(X) d\mathcal \leq g(a) $$
$$ g(a)\mathcal{P}(A) \leq Eg(X) \leq \sup g(X)\mathcal{P}(A) + g(a) $$
\qed
\end{proof}

\subsubsection{Aplicaciones}
\begin{enumerate}
\item Usando la desigualdad básica con $g(X) = X^r$ y $E|X_n - X|^r
\to 0 \Rightarrow X_n \stackrel{\mathcal{P}}{\rightarrow} X$
\item ($\Omega$, $\mathcal{A}$, $\mathcal{P}$)
$\stackrel{\mathcal{P}}{\rightarrow}$ ($\mathbb{R}$, $\mathcal{B}$),
definimos ahora $\mathcal{P}^X(\mathcal{B}) =
\mathcal{P}(X^{-1}(\mathcal{B}))$. $\mathcal{P}^X$ es una
probabilidad, ya que $\mathcal{P}^X(\mathbb{R}) = 1,
\mathcal{P}^X(\mathcal{B}) \geq 0, \mathcal{P}^X(\sum B_j) = \sum
\mathcal{P}^X(B_j)$, y $EX = \displaystyle \int_{x \in \mathbb{R}} x d
\mathcal{P}^X(x)$; $Eg(X) = \displaystyle \int_{y \in \mathbb{R}} g d
\mathcal{P}^Y(y) = \displaystyle \int_{x \in \mathbb{R}} g(x) d
\mathcal{P}^X(x)$
\end{enumerate}

\section{Convergencia en r-medida}
Se dice que una sucesión de variables aleatorias $X_n$ converge en
r-medida a $X$ si:
$$ E|X_n - X|^r \to 0$$
Lo notamos como $X_n \stackrel{r}{\rightarrow} X$

\begin{lemma}
Si $X_n \stackrel{r}{\rightarrow} X \Rightarrow E|X_n|^r \rightarrow E|X|^r$
\end{lemma}

\begin{proof}
Tenemos dos casos, para $r \leq 1$ y $r \geq 1$\\

Para $r \leq 1$: $|E|X_n|^r - E|X|^r| \leq E|X_n - X|^r \rightarrow 0$\\

Para $r \geq 1$: $|(E|X_n|^r)^{\frac{1}{r}} - (E|X|^r)^{\frac{1}{r}}|
\leq (E|X_n - X|^r)^{\frac{1}{r}} \rightarrow 0$
\end{proof}

\section{Función de distribución, distribución inducida y función
generatriz de momentos}
\subsection{Función de distribución}
Función puntual que se define sobre la recta real, no negativa, no
decreciente, continua por la izquierda y que cumple que $F(-\infty) =
0, F(+\infty) = 1$\\

\subsection{Distribución inducida}
Se conoce como distribución inducida por la variable aleatoria $X$ a
($\mathbb{R}$, $\mathcal{B}$, $\mathcal{P}^X$), donde la medida de
probabilidad $\mathcal{P}^X$ se define como:
$$ \mathcal{P}^X(B) = \mathcal{P}(X^{-1}(B)), \, \forall B \in \mathcal{B} $$
Tenemos entonces que:
\begin{itemize}
\item $\mathcal{P}^X(B) \geq 0 \forall B \in \mathcal{B}$
\item $\displaystyle \mathcal{P}^X(\sum_j B_j) =
\mathcal{P}(X^{-1}(\sum_jB_j)) = \mathcal{P}(\sum_j X^{-1}(B_j)) =
\sum_j \mathcal{P}(X^{-1}(B_j)) = \sum_j \mathcal{P}^X(B_j)$
\item $\displaystyle EX = \int_{\omega \in \Omega} X(\omega) d
\mathcal{P(\omega)} = \int_{x \in \mathbb{R}} x d\mathcal{P}^X(x)$
\end{itemize}

\subsection{Función generatriz de momentos}
Llamamos función generatriz de momentos de la variable aleatoria $X$ a
la función:
$$ M_X(t) = E(e^{tX}); \, t \in \mathbb{R} $$
\subsection{Función característica}
Dada una variable aleatoria $\mathbb{X}$ continua, definimos su
función característica como:
$$\varphi_X(t)=E(e^{itX})=\int_{-\infty}^{\infty}e^{itx}f_{X}(x)=E(cos(tX))+iE(sen(TX))$$

\chapter{Independencia}
\section{Concepto de independencia}
\textbf{Definición: }Se dice que los eventos $A_t$ son independientes
si para todo subconjunto finito $(t_i,\ldots ,t_n)$ se tiene que:
$$P\bigcap_{k=1}^n A_{tk}=\displaystyle\prod_{k=1}^{n}P\, A_{tk}$$
De hecho, el concepto de independencia es relativo a la familia de
clases. Una clase de eventos se dice independiente si sus eventos son
independientes.

\begin{theorem}
Se tiene que las subclases de una clase independiente son independientes.
\end{theorem}

\section{Suma de variables aleatorias independientes}
\subsubsection{Teorema de Borel}
\begin{theorem}
Las funciones de Borel de funciones aleatorias independientes son
independientes.
\end{theorem}
\subsubsection{Teorema de extensión}
\begin{theorem}
Los $\sigma$ algebras minimales independientes sobre clases
independientes cerradas para la intersección finita son independientes
\end{theorem}
Esto tiene tres aplicaciones fundamentales:
\begin{enumerate}
\item Si los eventos $A_t$ son independientes, también lo son los
$\sigma$ algebras $(A_t , A_t^c , \emptyset , \Omega)$.
\item Si la imagen inversa $\mathcal{C}_t$ de las clases de todos los
intervalos $(-\infty, x_t)$ en los espacios de Borel $R_t$ son
independientes, también lo son las imágenes inversas $\mathcal{B}_t$
de los algebras de Borel en $R_t$. Para todo $\mathcal{C}_t$, éste es
cerrado para la intersección finita y $\mathcal{B}_t$ es el $\sigma$
algebra minimal sobre $\mathcal{C}_t$
\item Sean $\mathcal{B}_t$ algebras de eventos y sea $T_s$ un
subconjunto de $T$. El $\sigma$ algebra $\mathcal{B}_T$ compuesto por
componentes $\mathcal{B}_t$, con $t\in T_s$, es el $\sigma$ algebra
minimal sobre la clase $\mathcal{C}$ de todas las intersecciones
finitas de eventos $A_t$ y contiene a todos sus componentes
\end{enumerate}
\subsubsection{Teorema de composición}
\begin{theorem}
Los $\sigma$ algebras compuestos son independientes si y solo si sus
$\sigma$ subalgebras finitamente compuestos son independientes
\end{theorem}
\subsection{Familia de variables aleatorias}
Una familia de variables aleatorias $X_{T_s}=\{ X_t \, , \, t\in T_s
\}$ induce $\sigma$ algebras $\mathcal{B}(X_{T_s})$ de eventos
\subsubsection{Teorema de las familias}
\begin{theorem}
Las familias de variables aleatorias son independientes si y solo si
sus subfamilias finitas son mutuamente independientes
\end{theorem}
\section{Multiplicación de variables aleatorias independientes}
\textbf{Definición: } Las variables aleatorias $X_t\, , \, t\in T$ son
independientes si para cada clase finita $(S_{t_1},\ldots , S_{t_n})$
de conjuntos de Borel en R:
$P\bigcap_{k=1}^{n}[X_{t_k}\in S{t_k}]=\displaystyle\prod_{k=1}^n
P[X_{t_k}\in S_{t_k}]$
\subsubsection{Lema de la multiplicación}
\begin{lemma}
Si $X_1, \ldots , X_n$ son variables aleatorias independientes no
negativas, entonces
$E\displaystyle\prod_{k=1}^{n}X_k=\displaystyle\prod_{k=1}^{n} E X_k$
\end{lemma}
\begin{proof}
Basta demostrar el resultado para dos variables, dado que el resto se
demuestra por inducción. En primer lugar, veamos que se verifica la
condición para funciones simples.\\

Sean $X = \sum_j x_j I_{A_j}, Y = \sum_k y_k I_{B_k}$ variables
simples no negativas, donde $A_j = [X = x_j], B_k = [Y = y_k]$.\\

Por ser $X,Y$ independientes, $P(A_jB_k) = P(A_j)P(B_k) \Rightarrow
E(XY) = \sum_{k,j} P(A_jB_k) = \sum_{j,k} P(A_j)P(B_k) = E(X)E(Y)$\\

Sean ahora $X,Y$ variables aleatorias no negativas independientes. Su
independencia implica la de
$$ A_{nj}=[\frac{j-1}{2^n} \leq X < \frac{j}{2^n}],
B_{nk}=[\frac{k-1}{2^n} \leq Y < \frac{k}{2^n}]$$
Finalmente, tendremos la independencia de las variables aleatorias simples:
$$ X_n = \sum_{j=1}^{n2^n} \frac {j-1}{2^n}I_{A_{nj}}, Y_n =
\sum_{k=1}^{n2^n} \frac {k-1}{2^n}I_{B_{nk}}$$
Tenemos entonces que:
$$ 0 \leq X_n \uparrow X, 0 \leq Y_n \uparrow Y \Rightarrow X_nY_n \uparrow XY$$
$$ E(X_nY_n) = E(X_n)E(Y_n)$$
De donde se extrae por el teorema de la convergencia dominada que
$E(XY) = E(X)E(Y)$
\qed
\end{proof}


## Variables aleatorias

## Independencia

## Esperanza condicional

## Sucesiones de variables aleatorias independientes

## Martingalas a tiempo discreto

## Procesos estocásticos

## Movimiento browniano

## Integración estocástica

## Aplicación a las finanzas

<!--chapter:end:313-probabilidades.Rmd-->

# Apéndice

<!--chapter:end:399-Apendice.Rmd-->


# (APPENDIX) Apéndice {-}
# Software Tools

Placeholder


## R and R packages
## Pandoc
## LaTeX

<!--chapter:end:400-apendice.Rmd-->

# Referencias {-}




<!--chapter:end:500-references.Rmd-->

