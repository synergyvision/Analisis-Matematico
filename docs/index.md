<script src="https://cdn.datacamp.com/datacamp-light-latest.min.js"></script>

--- 
title: "Análisis, Medida y Probabilidades"
subtitle: "Ciencia de los Datos Financieros"
author: "Synergy Vision"
date: "2019-04-03"
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

<a href="https://synergy.vision/LibrosInteractivos/" target="_blank"><img src="images/cover.png" style="display: block; margin: auto;" /></a>


![Creative Commons License](images/by-nc-sa.png)  
La versión en línea de este libro se comparte bajo la licencia [Creative Commons Attribution-NonCommercial-ShareAlike 4.0 International License](http://creativecommons.org/licenses/by-nc-sa/4.0/).

## ¿Por qué  leer este libro? {-}

Este libro es el resultado de enfocarnos en proveer la mayor cantidad de material sobre Análisis y teoría de la medida con un desarrollo teórico lo más explícito posible, con el valor agregado de incorporar ejemplos de las finanzas y la programación en `R`. Finalmente tenemos un libro interactivo que ofrece una experiencia de aprendizaje distinta e innovadora.

El un mundo abierto, ya no es tanto el acceso a la información, sino el acceso al conocimiento. 

Es mucha la literatura, pero son pocas las opciones donde se pueda navegar el libro de forma amigable y además contar con ejemplos en `R` y ejercicios interactivos, además del contenido multimedia. Esperamos que ésta sea un contribución sobre nuevas prácticas para publicar el contenido y darle vida, crear una experiencia distinta, una experiencia interactiva y visual. El reto es darle vida al contenido asistidos con las herramientas de Internet.

Finalmente este es un intento de ofrecer otra visión sobre la enseñanza y la generación de material más accesible. Estamos en un mundo multidisciplinado, es por ello que ahora hay que generar contenido que conjugue en un mismo lugar las matemáticas, estadística, finanzas y la computación.

Lo dejamos público ya que las herramientas que usamos para ensamblarlo son abiertas y públicas.

## Estructura del libro {-}

TODO: Describir la estructura

## Información sobre los programas y convenciones {-}

Este libro es posible gracias a una gran cantidad de desarrolladores que contribuyen en la construcción de herramientas para generar documentos enriquecidos e interactivos. En particular al autor de los paquetes Yihui Xie xie2015.

## Prácticas interactivas con R {-}

Vamos a utilizar el paquete [Datacamp Tutorial](https://github.com/datacamp/tutorial) que utiliza la librería en JavaScript [Datacamp Light](https://github.com/datacamp/datacamp-light) para crear ejercicios y prácticas con `R`. De esta forma el libro es completamente interactivo y con prácticas incluidas. De esta forma estamos creando una experiencia única de aprendizaje en línea.

<div data-datacamp-exercise data-height="300" data-encoded="true">eyJsYW5ndWFnZSI6InIiLCJwcmVfZXhlcmNpc2VfY29kZSI6ImIgPC0gNSIsInNhbXBsZSI6IiMgQ3JlYSB1bmEgdmFyaWFibGUgYSwgaWd1YWwgYSA1XG5cblxuIyBNdWVzdHJhIGVsIHZhbG9yIGRlIGEiLCJzb2x1dGlvbiI6IiMgQ3JlYSB1bmEgdmFyaWFibGUgYSwgaWd1YWwgYSA1XG5hIDwtIDVcblxuIyBNdWVzdHJhIGVsIHZhbG9yIGRlIGFcbmEiLCJzY3QiOiJ0ZXN0X29iamVjdChcImFcIilcbnRlc3Rfb3V0cHV0X2NvbnRhaW5zKFwiYVwiLCBpbmNvcnJlY3RfbXNnID0gXCJBc2VnJnVhY3V0ZTtyYXRlIGRlIG1vc3RyYXIgZWwgdmFsb3IgZGUgYGFgLlwiKVxuc3VjY2Vzc19tc2coXCJFeGNlbGVudGUhXCIpIn0=</div>







## Agradecimientos {-}

A todo el equipo de Synergy Vision que no deja de soñar. Hay que hacer lo que pocos hacen, insistir, insistir hasta alcanzar. Lo más importante es concretar las ideas. La idea es sólo el inicio y solo vale cuando se concreta.


\BeginKnitrBlock{flushright}<p class="flushright">Synergy Vision, Caracas, Venezuela</p>\EndKnitrBlock{flushright}








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

---
output:
  pdf_document: default
  html_document: default
---
# Conjuntos

Los términos *conjunto*, *colección* y *familia* suelen ser sinónimos, a pesar de que en algunos contextos una de estas palabras tiene prioridad sobre otra. Por ejemplo, se suele decir *colección de conjuntos* y *familia de funciones*. Los conjuntos usualmente se denotan con una letra mayúscula, mientras que para los elementos de un conjunto se utilizan minúsculas. La notación $a \in A$ indica que el elemento $a$ pertenece al conjunto $A$. Por ejemplo, $$2 \in \{a, 3, 2, b\}$$ indica que el elemento $2$ pertenece al conjunto $\{a, 3, 2, b\}$. Nótese que el orden en que se escriben los elementos de un conjunto es indiferente. Así el conjunto anterior es igual a $$\{3,b,a,2\}.$$

Las llaves $\{ \ \}$ siempre se usarán en la definición de conjuntos. En general, para describir a un conjunto exsisten dos formas de hacerlo. Cuando un conjunto se define dando la lista completa de todos sus elementos, decimo por ejemplo 


## Operaciones conjuntistas

Si $A$ es un subconjunto de $B$, escribimos $A \subseteq B$. Si todos los conjuntos con los que se trabaja son subconjuntos de un conjunto $X$, entonces $X$ es llamado el conjunto universal. El conjunto potencia de un conjunto $X$ es la colección $\mathcal{P}(X)$ de todos los subconjuntos de $X$, es decir: $$ \mathcal{P}(X) = \{Y \, : \, Y \subseteq X\}.$$

Si $A, B \subseteq X$, entonces $A \cup B$, $A \cap B$ y $A \setminus B$ denotan la unión, intersección y diferencia relativa de $A$ y $B$, El complemento de $A$, definido como los elementos de $X$ que no están en $A$, se denota por $A^c$. Si $\mathcal{A}$ es un subconjunto de $\mathcal{P}(X)$ y $B \in \mathcal{P}(X)$, se define la traza de $\mathcal{A}$ en $B$ como $$\mathcal{A}\cap B := \{A \cap B \, : \, A \in \mathcal{A}\}.$$

La unión e intersección de una familia indexada $\mathcal{A}=\{A_i \, : \, i \in \mathcal{I}\}$ se denotan, respectivamente, como
$$\cap \mathcal{A}:= \cap_{i \, \in \, \mathcal{I}},$$
y
$$\cup \mathcal{A}:= \cup_{i \, \in \, \mathcal{I}},$$ 

Si el conjunto de índices $\mathcal{I}$ es $\{1,2, \hdots, n\}$ o $\{1,2, \hdots\}$, se escribe
$$\cup_{j=1}^n A_j=A_1 \cup \hdots \cup A_n$$
$$\cap_{j=1}^n A_j=A_1 \cap \hdots \cap A_n$$
$$\cup_{j \geq 1} A_j=A_1 \cup A_2 \cup \cdots$$
$$\cap_{j \geq 1} A_j=A_1 \cap A_2 \cap \cdots$$ 

\begin{prop}
La unión e intersección de conjuntos satisfacen:
\begin{item}
\item
\end{item}
\end{prop}

## Operaciones conjuntistas

Si $A$ es un subconjunto de $B$, escribimos $A \subseteq B$. Si todos los conjuntos con los que se trabaja son subconjuntos de un conjunto $X$, entonces $X$ es llamado el conjunto universal. El conjunto potencia de un conjunto $X$ es la colección $\mathcal{P}(X)$ de todos los subconjuntos de $X$, es decir: $$ \mathcal{P}(X) = \{Y \, : \, Y \subseteq X\}.$$

Si $A, B \subseteq X$, entonces $A \cup B$, $A \cap B$ y $A \setminus B$ denotan la unión, intersección y diferencia relativa de $A$ y $B$, El complemento de $A$, definido como los elementos de $X$ que no están en $A$, se denota por $A^c$. Si $\mathcal{A}$ es un subconjunto de $\mathcal{P}(X)$ y $B \in \mathcal{P}(X)$, se define la traza de $\mathcal{A}$ en $B$ como $$\mathcal{A}\cap B := \{A \cap B \, : \, A \in \mathcal{A}\}.$$

La unión e intersección de una familia indexada $\mathcal{A}=\{A_i \, : \, i \in \mathcal{I}\}$ se denotan, respectivamente, como
$$\cap \mathcal{A}:= \cap_{i \, \in \, \mathcal{I}},$$
y
$$\cup \mathcal{A}:= \cup_{i \, \in \, \mathcal{I}},$$ 

Si el conjunto de índices $\mathcal{I}$ es $\{1,2, \hdots, n\}$ o $\{1,2, \hdots\}$, se escribe
$$\cup_{j=1}^n A_j=A_1 \cup \hdots \cup A_n$$
$$\cap_{j=1}^n A_j=A_1 \cap \hdots \cap A_n$$
$$\cup_{j \geq 1} A_j=A_1 \cup A_2 \cup \cdots$$
$$\cap_{j \geq 1} A_j=A_1 \cap A_2 \cap \cdots$$ 

\begin{prop}
La unión e intersección de conjuntos satisfacen:
\begin{itemize}
\item {\bf Leyes de DeMorgan}
\begin{itemize}
\item[(1)] \left(\bigcap_{i \in \mathcal{I}}A_i \right)^c = \bigcup_{i \in \mathcal{I}}A_i^c;
\item[(2)] \left(A\bigcap_{i \in \mathcal{I}} A_i  \right)^c=\bigcup_{i \in \mathcal{I}}A_i^c;
\end{itemize}
\begin{itemize}
\item {\bf Leyes distributivas}
\item[(3)] A \cup \left(\bigcap_{i \in \matjcal{I}}A_i  \right) = \bigcap_{i \i \mathcal{I} A \cup A_i};
\item[(d)] A \cap \left(\bigcup_{i \in \mathcal{I}} A_i    \right) = \bigcup_{i \in \mathcal{I}}A \cap A_i.
\end{itemize}
\end{prop}
	
Una familia $\{A_i \, : \, i \in \mathcal{I}\}$ de conjuntos se dice {\bf disjunta} si $A_i \cap A_j=\emptyset$, siempre que $i \neq j$. En este caso, la uni\'on $\bigcup_{i \in \mathcal{I}}$ se dice {\bf uni\'on disjunta}. Una {\bf partici\'on} (o {\bf partici\'on conjuntista}) de un conjunto $X$ es una colecci\'on de conuntos disjuntos no vac\'ios , cuya uni\'on disjunta es todo $X$.
	
Una sucesi\'on de conjuntos $\{A_n\}_{n \geq 0}$ se dice {\bf ascendente} si $A_1  \leq subseteq A_2 \subseteq \cdots$, en cuyo caso escribiremos $A_n \uparrow$. Si $A_1 \supseteq A_2 \supseteq \cdots$, se dice que la sucesi\'on es {\bf decreciente}. Denotaremos por $A_n \downarrow$ a una sucesi\'on que es decreciente. Si $\{A_n\}_{n \geq 0}$ es creciente y $A=A_1 \cup A_2 \cup \cdots$ (respectivamente si $\{A_n\}_{n \geq 0}$ es decreciente y $A=A_1 \cap A_2 \cap \cdots$), escribiremos $A_n \uparrow A$ (respectivamente $A_n \downarrow A$).
	
El producto cartesiano de sucesiones finitas o infinitas numerables de conjuntos $A_1, A_2, \hdots$ se denotan, respectivamente, por
$\begin{array}[ccc]
\prod_{n=1}^d A_n = A_1 \times \cdots \times A_d &y& \prod_{n=1}^\infty A_n = A_1 \times A_2 \times \cdots.
\end{array}$
	
Si $A_1 = A_2 = \cdots = A$, escribiremos $A^d$ para el producto finito  y $A^\infty$ para el producto infinito.
	
\begin{prop}
El producto cartesiano satisface las siguiente propiedades:
\begin{itemize}
\item[(1)] $A \times (A_1 \cup A_2 \cup \cdots)=(A \times A_1 \cup A_2 \cup \cdots)=(A \times A_1) \cup (A \times A_2) \cup \cdots$;
\item[(2)] $A \times (A_1 \cap A_2 \cap \cdots)=(A \times A_1 \cap A_2 \cap \cdots)=(A \times A_1) \cap (A \times A_2) \cap \cdots$;
\item[(3)] $(A_1 \cap A_2 \cap \cdots)\times (B_1 \cap B_2 \cap \cdots)=(A_1 \times B_1) \cap (A_2 \times B_2) \cap \cdots$.
\end{itemize}
\end{prop}
	
El producto cartesiano $X:=\prod_{i \in \mathcal{I}}X_i$ de una familia de conjuntos no vacios $X_i$ se define como la colecci\'on de todas las funciones $f:\mathcal{I}\to \bigcup_{i \in \mathcal{I}}X_i$ tales que $f(i)\in X_i$, para cada $i$. N\'otese que el producto cartesiano de conjuntos no vac\'ios es siempre no vac\'io, por el axioma de elecci\'on. El valor $f(i)$ se denomina la {\bf i-\'esima coordenada de $f$}. En el caso particular en que el conjunto de \'indices $\mathcal{I}$ sea el conjunto $\{1,2, \hdots, n\}$, se tiene que toda funci\'on $f: \{1,2, \hdots, n\}\to X$ est\'a completamente determinada por por la $n$-tupla $(f(1), f(2), \dots, f(n))$.
	
## Sistemas numéricos
	
Usaremos la siguiente notaci\'on para el sistema num\'e rico est\'andar:
\begin{itemize}
\item $\mathbb{N}:=\{0,1,2,3, \hdots\}$: el conjunto de los {\bf n\'umeros naturales} o {\bf enteros no negativos};
\item $\mathbb{P}:= \mathbb{N}\setminus \{0\}$: el conjunto de los {\bf n\'umeros enteros positivos};
\item $\mathbb{Z}$: el conjunto de los {\bf n\'umeros enteros};
\item $\mathbb{Q}$: el conjunto de los {\bf n\'umeros racionales};
\item $\mathbb{R}$: el conjunto de los {\bf n\'umeros reales};
\item $\mathbb{C}$: el conjunto de los {\bf n\'umeros complejos}.
\end{itemize}


Los términos conjuntos, colecciones y familias son sinónimos, a pesar de que en algunos contextos se tenga mas preferencia sobre una frase que otra. Por ejemplo, se suele decir coleccion de objetos y familia de funciones. Los conjuntos se denotan usualmente con una letra mayuscula, y elementos de un conjunto con una letra minuscula. Se usa la notacion $$a \in A$$ para indicar que el elemento $a$ pertenece al conjunto $A$. 

Existen dos maneras de representar a un conjunto (comprehensiva y extensiva, ver notas de Manuel.)

\


Dos subconjuntos de $\mathbb{C}$ son de particular importancia:
\begin{itemize}
\item {\bf el disco unitario}:
\[\mathbb{D}:=\{z \in \mathbb{C}: \, |z|<1\};\]
\item {\bf el grupo circular}:
\[\mathbb{T}:=\{z \in \mathbb{C}: \, |z|=1\}.\]
\end{itemize}

En general, el s\'imbolo $\mathbb{K}$ denota a un cuerpo de caracter\'istica $0$, como por ejemplo $\mathbb{Q}$, $\mathbb{R}$ o $\mathbb{C}$. 

Si $A \subseteq \mathbb{R}$, escribiremos $A^+$ para denotar al conjunto $A \cap [0, \infty)$. Asi, por ejemplo, se tiene que $\mathbb{Z}^+=\{n \in \mathbb{Z} \, : \, n \geq 0\}=\mathbb{N}$.

Si $A \subseteq \mathbb{C}$, se denota por $A_*$ al conjunto de elementos no nulos de $A$.

Sea $d$ un entero positivo. Si $A$ es un conjunto, se define
\[A^d:=A \times A \times \cdots \times A.\]

Los {\bf espacios eucl\'ideos $d$-dimensionales reales y complejos} se definen, respectivamente, como $\mathbb{R}^d$ y $\mathbb{C}^d$, con $d \in \mathbb{P}$.

Un {\bf intervalo $d$-dimensional} en $\mathbb{R}^d$ es un producto cartesiano de intervalos en $\mathbb{R}$. Es decir, si ${\bf a}:=(a_1, a_2, \hdots, a_d)$ y ${\bf b}:=(b_1, b_2, \hdots, b_d)$ son elementos de $\mathbb{R}^d$, un intervalo $d$-dimensional es de la forma
\[({\bf a}, {\bf b}]:=(a_1, b_1] \times (a_2, b_2] \times \cdots \times (a_d, b_d].\]

La {\bf norma eucl\'idea} en $\mathbb{K}^d$ se define como 
\[|{\bf z}|:=\sqrt{|z_1|^2+|z_2|^2+ \cdots + |z_d|^2},\]
para cada ${\bf z}=(z_1, z_2, \hdots, z_d) \in \mathbb{C}^d$.

El {\bf sistema num\'erico real extendido} es el conjunto
\[\overline{\mathbb{R}}:=\mathbb{R} \cup \{\pm \infty\}=[-\infty, +\infty].\]

Aqui, $-\infty$ y $+ \infty$ denotan dos s\'imbolos abstractos, que satisfacen los siguientes axiomas:
\begin{itemize}
\item $-\infty, +\infty \notin \mathbb{R}$;
\item $-\infty < x < +\infty$, para todo $x \in \mathbb{R}$;
\item $x+\infty = \infty$, si $-\infty < x \leq +\infty$;
\item $x-\infty = -\infty$, si $-\infty \leq x < \infty$;
\item $x \cdot(+\infty)=\infty$, si $0 < x \leq +\infty$;
\item $x \cdot(+\infty)=-\infty$, si $-\infty < x <0$;
\item $x \cdot (-\infty)=-\infty$, si $0 < x < +\infty$;
\item $x \cdot (-\infty)=+\infty$, si $-\infty \leq x < 0$;
\item $\frac{x}{+\infty}=\frac{x}{-\infty}=0$, si $-\infty < x < +\infty$;
\item $0 \cdot (\pm \infty)=0$.
\end{itemize}

Los elementos de $[0, +\infty]=\overline{\mathbb{R}}^+$ se denominan {\bf n\'umeros reales no negativos extendidos}.



## Relaciones  



Una {\bf relaci\'on} en un conjunto no vac\'io $X$ es un conjunto $R \subseteq X \times X$, no vac\'io. Si $R$ es una relaci\'on de $X$ y $(x,y) \in R$, se escribe $x \sim_R y$, o $x \sim y$. Una relaci\'on de $X$ se dice:
\begin{itemize}
\item {\bf reflexiva} si $x \sim x$, para todo $x \in X$;
\item {\bf sim\'etrica} si $x \sim y$ implica $y \sim x$;
\item {\bf transitiva} si $x \sim y$ y $y \sim z$ implican $x \sim z$;
\item {\bf antisim\'etrica} si $x \sim y$ y $y \sim x$ implican $x=y$.
\end{itemize}

Una relaci\'on en $X$ que es reflexiva, sim\'etrica y transitiva se conoce como {\bf relaci\'on de equivalencia}. La {\bf clase de equivalencia de $x \in X$} es el conjunto
\[[x]:= \{y \in X \, : \, x \sim y\}.\]

La colecci\'on de clases de equivalencias distintas de $X$ se denota como $X/\sim$. As\'i:
\[X/\sim = \{[x] \, : \, x \in X\}.\]
Las relaciones de equivalencia de un conjunto no vac\'io X y las particiones conjuntistas de $X$ son dos nociones equivalentes. En efecto, dado que
\begin{equation}
x \in [y] \Longleftrightarrow y \in [x] \Longleftrightarrow [x]=[y],
\end{equation}
es claro que los elementos de $X/\sim$ son disjuntos dos a dos. Adem\'as,
\begin{equation}
\bigcup_{[x] \, \in \, X/\sim}[x]=\{y \in X \, : \, x \sim y, \text{ para alg\'un } x \in X\}=X.
\end{equation}
As\'i, la colecci\'on $X/\sim$ es una partici\'on de $X$. Rec\'iprocamente, dada una partici\'on de $X$, la relaci\'on definida por
\begin{equation}
x \sim y \Longleftrightarrow x \text{ y } y \text{ pertenecen al mismo bloque de la partici\'on }
\end{equation}
es una relaci\'on de equivalencia para $X$, donde cada clase de equivalencia es precisamente un bloque de la partici\'on.

Un ejemplo de relaci\'on de equivalencia en $\mathbb{R}$ es el siguiente: la relaci\'on $\sim$ est\'a dada por
\begin{equation}
x\sim y \Longleftrightarrow x-y \in \mathbb{Q}.
\end{equation}
En este caso, existe solo una clase $[x] \in \mathbb{R}/\sim$ formada por n\'umeros racionales. De hecho, no es dif\'icil demostrar que $[x]=\mathbb{Q}$. Cualquier otra clase $[y]$ de $\mathbb{R}/\sim$ est\'a formada por n\'umeros irracionales.

Una relaci\'on que es reflexiva, antisim\'etrica y transitiva es llamada un {\bf orden parcial}. En este caso, se escribe $x \leq y$ para denotar que el par $(x,y)$ pertenecen a este tipo de relaci\'on. Un conjunto con un orden parcial se denomina {\bf conjunto parcialmente ordenado}. Una {\bf cota superior} (respectivamente, {\bf cota inferior}) de un subconjunto $Y$ de un conjunto parcialmente ordenado $(X, \leq)$ es un elemento $x \in X$ tal que $y \leq x$ (respectivamente, $x \leq y$), para todo $y \in Y$. Un {\bf supremo} (respectivamente, un {\bf \'infimo})de $Y$ es una cota superior (respectivamente, inferior) $x_0$ de $Y$ tal que $x_0 \leq x$ (respectivamente, $x_0 \geq x$) para toda cota superior (respectivamente, inferior) $x$ de $Y$. Por ejemplo, el par $(\mathcal{P}(X), \subseteq)$ forma un conjunto parcialmente ordenado, para cada conjunto $X$. Si $Y \in \mathcal{P}(X)$, entonces los subconjuntos $\cap_{y \, \in \, Y}y$ y $\cup_{y \, \in \, Y}y$ corresponden al \'infimo y al supremo de $Y$, respectivamente. Un elemento $x$ de $X$ se dice {\bf maximal} si para cada $y \in X$ tal que $x \leq y$, se tiene que $x=y$. Del mismo modo, un elemento $x$ de $X$ se dice {\bf minimal} si para cada $y \in X$ tal que $x \geq y$, se tiene que $x=y$.

Un subconjunto no vac\'io $Y$ de un conjunto parcialmente ordenado $(X, \leq)$ se dice {\bf totalmente ordenado} si, para cada $y_1, y_2 \in Y$ distintos se satisface $y_1 \leq y_2$ o $y_2 \leq y_1$. Un conjunto totalmente ordendao tambi\'en suele llamarse una {\bf cadena}. La noci\'on de cadena aparece en el siguiente resultado importante, que se prueba utilizando directamente el axioma de elecci\'on:

Lema de Zorn: Sea $X$ un conjunto parcialmente ordenado, tal que cada cadena posea una cota superior en $X$. Entonces $X$ posee un elemento maximal.

\

##Funciones

\

Sean $X$ y $Y$ conjuntos. Una {funci\'on} de $X$ en $Y$ es (completar). Una funci\'on $f$ cuyo conjunto de partida es $X$ y conjunto de llegada es $Y$ se denota por $f: X \to Y$. La colecci\'on de todas las funciones de $X$ en $Y$ se denota como $Y^X$.

La {\bf imagen} de $A \subseteq X$ y la {preimagen} de $B \subseteq Y$ bajo la funci\'on $f:X \to Y$ se definen, respectivamente, como
\[f(A):=\{f(x) \in B \, : \, x \in A\},\]
y
\[f^{-1}(A):=\{x \in A \, : \, f(x) \in B\}.\]

Una funci\'on $f:X \to Y$ es {\bf sobreyectiva} si $f(X)=Y$, e {\bf inyectiva} si $x_1 \neq x_2$ implica que $f(x_1)\neq f(x_2)$. Una {\bf sobreyecci\'on} (respectivamente, una {\bf inyecci\'on}) es una funci\'on que es sobreyectiva (respectivamente, inyetiva). Una funci\'on que es a la vez sobreyectiva e inyectiva se dice {\bf biyectiva}. 

Un ejemplo importante de funci\'on sobreyectiva es la {funci\'on cociente} 
$C_\sim: X \to X/\sim$, asociada a una relaci\'on de equivalencia $\sim$ de un conjunto no vac\'io $X$. Por definici\'on, $C_\sim(x):=[x]$. En particular, la preimagen de un subconjunto $B$ de $X/\sim$ bajo $C_\sim$ es la uni\'on de todas las clases de equivalencias $[x]$ in $B$.

Si $X$, $Y$ son conjuntos y $\{X_i \, : \, i \in \mathcal{I}\}$, $\{Y_j \, : \, j \in \mathcal{J}\}$ son subconjuntos de $X$ y $Y$, respectivamente, se tiene que:
\begin{itemize}
\item[(a)] $f^{-1}\left(\bigcup_{j \in \mathcal{J}}Y_j \right)=\bigcup_{j \in \mathcal{J}}f^{-1}(Y_j)$;
\item[(b)] $f^{-1}\left(\bigcap_{j \in \mathcal{J}}Y_j \right)=\bigcap_{j \in \mathcal{J}}f^{-1}(Y_j)$;
\item[(c)] $f\left(\bigcup_{i \in \mathcal{I}}X_i \right)=\bigcup_{i \in \mathcal{I}}f(I_i)$;
\item[(d)] $f\left(\bigcap_{i \in \mathcal{I}}X_i \right)\subseteq\bigcap_{i \in \mathcal{I}}f(I_i)$;
\item[(e)] $f^{-1}(Y_j^c)=(f^{-1}(Y_j))^c$
\item[(f)] $f(X_i^c)=(f(X_i))^c$;
\item[(g)] $f(f^{-1}(Y_j)) \subseteq Y_j$; 
\item[(h)] $X_i \subseteq f^{-1}(f(X_i))$.
\end{itemize}

\

Las igualdades en $(d)$ y $(h)$ se satisfacen si $f$ es inyectiva, mientras que las igualdades de $(f)$ y $(g)$ suceden si $f$ es sobreyectiva.

Para cada $f:X \to Y$, $\mathcal{A} \subseteq \mathcal{P}(X)$ y $\mathcal{B} \subseteq \mathcal{P}(X)$, se definen las colecciones
\[f(\mathcal{A})=\{f(A) \, : \, A \in \mathcal{A}\} \subseteq \mathcal{P}(y)\]

\[f^{-1}(\mathcal{B})=\{f^{-1}(B) \, : \, B \in \mathcal{B}\}\subseteq \mathcal{P}(y)\]
 
Si $f:X \to Y$ y $g: Y \to Z$ son funciones, donde $f(X)\subseteq Y$, la función $g \circ f:X \to Z$ definida por $$(g\circ f)(x)=g(f(x))$$, para todo $x \in X$, se denomina {\bf función composición de $g$ con $f$}. Si $A \subseteq Z$, nótese que se tiene la siguiente relación: $$(g \circ f)^{-1}=f^{-1}(g^{-1}(A))$$.

La {\bf función identidad} $\text{id}_X$ de un conjunto $X$ se define como $\text{id}_X(x)=x$, para cada $x \in X$. Si $A \subseteq X$, la restricción
de $\text{id}_X$ a $A$ se denomina {\función inclusión} o {morfina de inclusión} y se denota como $\iota_A : A \hookuparrow X$.

Si $f:X \to Y$ es biyectiva, la {\bf función inversa} $f^{-1}:Y \to X$ es la función definida como
\[f^{-1}(y)=x \Longleftrigtharrow y=f(x).\]
Se tiene que
\begin{array}[ccc]
f^{-1}\circ f=\text{id}_X &y& f \circ f^{-1}=\text{id}_Y.
\end{array}

Si $X$ es un conjunto universal y $A \subseteq X$, la {\bf función indicatriz de $A$} es la función definida por
\begin{equation}
{\bf 1}_A(x)= \left\{ \begin{array}{lcc}
1 & \text{ si } & x \in A \\
0 & \text{ si } & x \in A^c
\end{array}
\right.
\end{equation}

Toda función indicatriz satisface las siguientes propiedades:
\begin{itemize}
\item {\bf 1}_{A \cap B}={\bf 1}_A{\bf 1}_B;
\item {\bf 1}_{A \cup B}= {\bf 1}_A + {\bf 1}_B - {\bf 1}_{A \cap B};
\item {\bf 1}_{A^c}=1-{\bf 1}_A.
\end{itemize}

Un caso particular de función indicatriz es la función {\bf delta de Kronecker}:
\begin{equation}
\delta_{x,y}= \left\{ \begin{array}{lcc}
1 & \text{ si } & x=y \\
0 & \text{ si } & x \neq y
\end{array}
\right.
\end{equation}

En efecto, si $A=\{(x,x) \, : \, x \in X\}$, entonces $\delta_{x,y}={\bf 1}_A(x,y)$.

Las funciones $x^+$ y $x^-$ en $\mathbb{R}$ se definen como 
\begin{array}{ccc}
x^+:=\max\{x,0\} & \text{ y } & x^-:=\max\{-x,0\}.
\end{array} 

De estas definiciones se desprende fácilmente que 
\begin{array}{ccc}
x=x^+-x^- & \text{ y } & |x|=x^+ + x^-.
\end{array} 

La parte real y la parte imaginaria de un número complejo $z$ se denotan, respectívamente, por $\Re(z)$ y $\Im(z)$. Asimismo, la conjugada de $z$ y el módulo de $z$ se denotan por $\overline{z}$ y $|z|$. Se tiene que
\begin{array}{cccccc}
z=\Re(z) + i\Im(z) &,& \overline{z}=\Re(z)-i\Im(z) & \text{ y } & |z|=\sqrt{(\Re(z))^2+(\Im(z))^2}.
\end{array}

El signo $\sgn(z)$ de una variable compleja $z$ se define como
\begin{equation}
\sgn(z)= \left\{ \begin{array}{lcc}
\frac{|z|}{z} & \text{ si } & z \neq 0 \\
0 & \text{ si } & z = 0.
\end{array}
\right.
\end{equation}


Así, $|z|=z\sgn(z)$ para todo $z \in \mathbb{C}$ y $|\sgn(z)|=1$ siempre que $z\neq 0$. 

Si $F \subseteq Y^X$, el funcional de evaluación en $x$ es la función $\text{ev}_x:F \to Y$ dada por
\begin{equation}
\text{ev}_x(f):=f(x), \qquad f \in F.
\end{equation}

El adjunto o dual de una función $\phi:Z \to X$ (con respecto a $F$) es la función $\phi^*:F \to Y^Z$ definida como
\begin{equation}
\phi^*(f):=f \circ \phi, \qquad f \in F.
\end{equation}

Las siguientes notaciones se utilizarán en los capítulos siguientes, para cada función a valores reales:
\begin{array}{cc}
f^+(x):=\max{f(x),0} & f^-:= (-f)^+\\
(f_1 \vedge \dots \vedge f_n)(x):=\max_{1 \, \leq \, k \,\leq \, n}f_k(x) & (f_1 \wedge \dots \wedge f_n)(x):=\min_{1 \, \leq \, k \,\leq \, n}f_k(x)\\
(\sup_n f_n)(x):=\sup_n f_n(x) & (\inf_n f_n)(x):=\inf_n f_n(x)\\
(\lim_n f_n)(x):=\lim_n f_n(x) & (_n f_n)(x):= _n f_n(x).
\end{array}

## Cardinalidad

Dos conjuntos $A$ y $B$ se dicen tener la misma cardinalidad si existe una biyección de $A$ a $B$.Un conjunto $A$ se dice finito si $A$ tiene la misma cardinalidad que $\{1,2, \hdots, n\}$, para algún $n \in \mathbb{N}$. En este caso, los elementos de $A$ se pueden indexar utilizando el conjunto $\{1,2, \hdots, n\}$, de modo que se puede escribir $A=\{a_1, a_2, \hdots, a_n\}$. Un conjunto $A$ es infinito numerable si tiene la misma cardinalidad que el conjunto $\mathbb{N}$ de los n, en cuyo caso se escribe $A=\{a_0, a_1, a_2, \hdots\}$. Un conjunto es numerable si es finito o infinito numerable; en caso contrario, se dice que el conjunto es no-numerable. Los conjuntos $\mathbb{Z}$ y $\mathbb{Q}$ son numerables. El conjunto $\mathbb{R}$ es no numerable, asi como cualquier intervalo de números reales. La cardinalidad de $\mathbb{R}$ se denota por $\mathfrak{c}$, mientras que la cardinalidad de $\mathbb{N}$ se denota por $\aleph_0$.

\bc{semigrupo}





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

---
output:
  pdf_document: default
  html_document: default
---
# Diferenciación



A lo largo de esta secci\'on vamos a trabajar en $\real^n={(x_1,\dots c, x_n) \  x_j \in \real, j=1,...,N}$
\subsection{Producto escalar, norma y distancia}
Durante todo el año denotaremos al vector $(x_1,x_2,\dots,x_n)$ como $\gx$ por comodidad.

\begin{defn}[Producto\IS escalar euclídeo]

\[ \pesc{\gx,\gy} = \sum_{i=1}^{N} x_iy_i \]


Propiedades:
\begin{itemize}
 \item $\pesc{\lambda \gx, \gy} = \lambda \pesc{\gx, \gy}$
 \item $\pesc{\overline{x} + \overline{y}, \overline{z}}= \pesc{\gx,\gz}+\pesc{\gy,\gz}$
 \item $\pesc{\gx, \gy} = \pesc{\gy,\gx}$
 \item $\pesc{\gx, \gx} ≥ 0$
 \item $\pesc{\gx,\gx} = 0 \implies \gx = \gor{0}$
\end{itemize}

Las tres primeras son la consecuencia de que el producto escalar tiene que ser bilineal.
\end{defn}

En general, un producto escalar es una matriz definida positiva y se opera de la siguiente manera:

\[\pesc{\gx,\gy} = (x_1,x_2,...,x_N) \cdot \begin{pmatrix}
a_11 &\cdots& a_1N\\
\vdots& \ddots & \vdots\\
a_N1 & \cdots& a_NN
\end{pmatrix}
\cdot \begin{pmatrix} y_1\\
\vdots\\ y_N \end{pmatrix}\]


\begin{defn}[Norma\IS euclídea]
\label{defnNorma}
\[ \md{\gx} = \left(\pesc{\gx,\gx}\right)^{\frac{1}{2}} = \dotsb = \left(\sum_{i=1}^{N}x_i^2\right)^{\frac{1}{2}} \]
Propiedades:
\begin{itemize}
 \item  $\md{\gx} = 0 \dimplies \gx = 0$
 \item	Homogeneidad: $\md{\lambda\gx} = \lambda\md{\gx}$
 \item	Desigualdad triangular: $\md{\gx+\gy} \leq \md{\gx}+\md{\gx}$
\end{itemize}
\end{defn}
\begin{lemma}
$\md{\gx} = (\gx \ast \gx) ^ \frac{1}{2}$ para cualquier producto escalar $\ast$.
\end{lemma}
\begin{defn}[Norma]
Cualquier operación que cumpla las 3 propiedades anteriores es una \textbf{norma}.

En general se tiene $\md{\cdot}_p, p \in \mathbb{N}$ y se definen todas de la misma forma:

\[ \md{\gx}_p = \left(\sum_{i=1}^N |x_i|^p \right)^\frac{1}{p} \]

\end{defn}

Hay tres casos particulares, la norma uno \index{Norma!uno}
\[ \md{\gx}_1 = |x_1| + |x_2| + ... + |x_n| \]

La norma 2, que es la norma euclídea

y la norma infinito \index{Norma!infinito}
\[\md{\gx}_{\infty} = \max\left\{|x_1|,|x_2|,\dots,|x_n|\right\} \]

 Vamos a demostrar que la norma $p$ cumple las 3 propiedades de una norma. Para ello, nos apoyaremos en dos teoremas previos:

\begin{theorem}[Desigualdad\IS de Young]
 Sea $p > 1$ y tomamos $p'$ tal que $\frac{1}{p}+\frac{1}{p'} = 1$ (exponente conjugado). Entonces:

\[ |ab| \leq \frac{1}{p} \cdot |a|^p +\frac{1}{p'} |b| ^ {p'} \]
\end{theorem}

\begin{proof}
Se utiliza la idea de la función logaritmo, que es cóncava\footnote{Geométricamente, cóncava significa que si uno 2 puntos de la gráfica, la recta que los une queda debajo de la gráfica.} y creciente.  Tomando 2 puntos $A$ y $B$ tenemos la condición de concavidad

\[ t \log A + (1-t) \log B \leq \log (tA + (1-t) \cdot B)\]

Utilizando la derivada hallamos la ecuación de la recta que pasa por $A$ y por $B$ y tomamos un punto que dista $t$ de $A$ y $(1-t)$ de $B$. Como la función es cóncava sabemos que ese valor será menor que el valor del logaritmo en un punto $t$ entre $A$ y $B$.

Tomando $A=|a| ^ p$, $B = |b| ^ p$ y $t = \frac{1}{p} \rightarrow 1-t = \frac{1}{p'}$ tenemos que

\begin{align*}
\frac{1}{p}\cdot log |a|^p + \frac{1}{p'} \cdot log|b|^{p'} &\leq log\left(\frac{1}{p}|a|^p + \frac{1}{p'} |b|^{p'}\right) \\
\log \abs{a} + \log \abs{b} &\leq log\left(\frac{1}{p}|a|^p + \frac{1}{p'} |b|^{p'}\right) \\
\log \abs{ab} &\leq log\left(\frac{1}{p}|a|^p + \frac{1}{p'} |b|^{p'}\right) \\
\abs{ab} &\leq \frac{1}{p}|a|^p + \frac{1}{p'} |b|^{p'}
\end{align*}
\end{proof}
\begin{theorem}[Desigualdad\IS de Hölder] Se trata de una generalización de la desigualdad de Cauchy-Schwarz, que ocurre en el caso $p=2$
\[ \sum_{i=1} ^ N \abs{x_i y_i} \leq \md{\gx}_p \md{y_i}_p \]
\label{thmHolder}
\end{theorem}

\begin{proof} Tomamos
 \begin{align*}
 a_i &= \frac{\abs{x_i}}{\md{\gx}_p} \\
 b_i &= \frac{\abs{y_i}}{\md{\gy}_{p'}}
 \end{align*}

 Tenemos que \[ a_i b_i \leq \frac{1}{p}a_i ^ p + \frac{1}{p'} b_i^{p'} \]

 Sustituimos:
 \[  frac{\abs{x_i}}{\md{x}_{p}} \cdot \frac{\abs{y_i}}{\md{y}_{p}} \leq \frac{\abs{x_i}^p}{p\cdot \md{x}_{p}^p} + \frac{\abs{y_i}^{p'}}{p'\cdot\md{y}_{p'}^{p}} \]

 Tomamos sumatorios y, teniendo en cuenta que $\md{x}_{p}^p = \sum|x_i|^p$, nos queda

 \[ \frac{1}{\md{x}_{p}\md{y}_{p'}}\cdot \sum_{i=1}^N |x_iy_i| \leq \frac{1}{p\md{x}_{p}^p} \sum |x_i|^p + \frac{1}{p'\md{y}_{p'}^{p'}} \sum |y_i|^{p'} = \frac{1}{p} + \frac{1}{p'} = 1 \]

 \end{proof}

Una vez probadas las dos desigualdades anteriores, pasamos a probar la desigualdad triangular:

\begin{proof} El objetivo es demostrar que \[ \md{\gx+\gy}_p \leq \md{\gx}_p+\md{\gy}_p \] y vamos a hacerlo en varios pasos.

 Para evitarnos las raíces empezamos con $\md{\gx+\gy}_p^p$

 \begin{gather*}
 \md{\gx+\gy}_p ^ p = \sum_1 ^ N |x_i+y_i| ^ p = \sum_ 1 ^ N |x_i+y_i| \cdot |x_i+y_i| ^ {p-1} =\\
 = \sum_1 ^ N |x_i|\cdot|x_i+y_i| ^ {p-1} + \sum_1^N |y_i| \cdot |x_i+y_i|^{p-1}
 \end{gather*}

 Utilizando la desigualdad de Hölder (\ref{thmHolder}) tenemos:

 \begin{multline*} \md{\gx+\gy}_p ^ p \leq \\
 \sum \left(|x_i|^p\right)^{\frac{1}{p}} \cdot \underbrace{\sum \left(\left(|x_i+y_i|^{p-1}\right)^{p'}\right)^{\frac{1}{p'}}}_* +
 \sum \left(|y_i|^p\right)^{\frac{1}{p}} \cdot \underbrace{\sum \left(\left(|X_i+y_i|^{p-1}\right)^{p'}\right)^{\frac{1}{p'}}}_*
 \end{multline*}

 Por ser $p$ y $p'$ exponentes conjugados es fácil comprobar que $1-\frac{1}{p'} = \frac{1}{p}$\\
 Sacamos factor común y pasamos al otro lado obteniendo (PASO INTERMEDIO?)
\[ \left(\sum_1^N |x_i+y_i|^p\right)^{\overbrace{\left(1-\frac{1}{p'}\right)}^p} = \md{\gx+\gy}_p \leq \md{x}_{p} + \md{y}_{p} \]

\textit{Guille: esta demostración es muy, muy rara.}
\end{proof}


EJERCICIO PROPUESTO: Tomamos en el plano el conjunto de los puntos cuya norma es 1. Tomando en la norma p=2 sale la circunferencia. ¿Y en p=3?


\begin{remark} Estos argumentos se pueden utilizar para demostrar
\[ \int \abs{f\cdot g}\, dx \leq \left(\int\abs{f}^p\, dx\right) ^ \frac{1}{p} \cdot \left(\int\abs{g}^{p'}\,dx\right)^\frac{1}{p'} \]
\end{remark}

\begin{defn}[Distancia\IS euclídea]
\[d(\gx,\gy) = \md{\gy - \gx} \]
\end{defn}

Propiedades:
\begin{itemize}
 \item La distancia es siempre positiva: $d(\gx,\gy)\ge 0$
 \item $d(\gx,\gx) = 0$
 \item Simetría: $d(\gx,\gy) = d(\gy, \gx)$
 \item Desigualdad triangular $d(\gx,\gz) \leq d(\gx,\gy) + d(\gy,\gz)$. La distancia entre 2 puntos es menor o igual en línea recta que pasando por un punto intermedio.
\end{itemize}


\begin{defn}[Distancia] Cualquier operacion que cumpla las 3 propiedades anteriores es una distancia. \end{defn}

\paragraph{Recapitulando}
Con un producto escalar puedo definir una norma y con esa norma puedo definir una distancia. Pero... ¿Podemos definir una norma
que no venga de un producto escalar y/o alguna distancia que no provenga de una norma? Sí, por ejemplo

\[ \tilde{d} (\gx,\gy) = \abs{\arctg(y) - \arctg(x)} \]

No cuesta mucho comprobar que cumple las 3 propiedades de una distancia. Además, esta distancia es cuanto menos curiosa porque nunca será mayor de $\pi$.

 Podemos comprobar que si existiera una norma que midiese esta distancia tendríamos \[\tilde{\md{\gx}} = \tilde{d} (\gx,\gor{0}) = \abs{\arctg (x)} \]
 pero esto no cumple la propiedad: $\tilde{\md{\lambda x}} = \abs{\arctg \lambda x} \neq \abs{\lambda}\abs{\arctg x} =
 \abs{\lambda x}\tilde{||x||}$
 ya que ninguna distancia puede ser mayor que $\pi$ y tomando un $\lambda > \pi$ se produciría la contradicción.

\subsubsection{Relación norma - producto escalar}
\label{secNormaprodEsc}
\begin{theorem}
Supongamos que tengo un producto escalar $\ast$ y una norma asociada \[ \md{\gx} = (\gx\ast \gx) ^ {\frac{1}{2}}\]. Entonces \[ \md{\gx + \gy}^ 2 =  \md{\gx} ^ 2 + \md{\gy} ^ 2+2(\gx\ast\gy) \]
\end{theorem}

\begin{proof}
\[ \md{\gx+\gy}^2 = (\gx+\gy)\ast(\gx+\gy) = \gx \ast \gx + \gx \ast \gy + \gy \ast \gx + \gy \ast \gy=\md{\gx} ^ 2 + \md{\gy} ^ 2+2(\gx\ast\gy) \]
\end{proof}

Esa norma asociada al producto escalar tiene dos propiedades importantes:
\begin{itemize}
\item Paralelogramo: $\md{\gx+\gy}^ 2 + \md{\gx-\gy} ^ 2 = 2\left(\md{x}^2+\md{y}^2\right) $
\item Polarización: $\md{\gx+\gy} ^ 2 - \md{\gx-\gy} ^ 2 = 4(\gx*\gy)$
\end{itemize}


\subsubsection{Equivalencia de normas}
Sea $\md{\cdot}$ una norma en $\real^N$. Si intento calcular la norma de un vector $\gx$

\[ \md{\gx} = \md{\sum x_i e_i} \leq \sum_{i=1}^N \md{x_1 e_1} = \sum_{i=1}^N|x_i|\cdot\md{e_i} \]

Tenemos: $\md{\gx} \leq \sum_{i=1}^N c_i |x_i|$ siendo $c_i = \md{e_i}$. Aplicando Cauchy-Schwarz  nos queda
\[ \sum_{i=1}^N \left(c_i^2\right)^\frac{1}{2} \cdot \sum \left(|x_i|^2\right)^\frac{1}{2} \]
Es decir, puedo controlar cualquier norma con una constante y la norma euclídea:
$$|||\gx||| \leq C \md{x}_{2}$$
En particular, $0 \leq |||\gor{x_n} - \gx|||\leq c ||\gor{x_n}-\gx||$.

\begin{remark}
Si aplicamos Holder en vez de Cauchy, sale la igualdad con la norma p y no con la euclídea.
\end{remark}

\paragraph{Aplicación:}
Sea $F(\gx) = |||\gx|||$ y $F:\real^N \rightarrow \real^N$
$$|F(\gx)-F(\gy)| = \left| |||\gx - \gy||| \right| = |||\gx - \gy||| \leq C ||\gx - \gy||$$
Utilizando: $|||\ga-\gb||| \ge |||\ga||| - |||\gb|||$ \footnote{(la desigualdad triangular con restas, que se saca con un simple cambio de variable)}

Es decir, cualquier norma en $\real^n$ es \textbf{continua} respecto de la norma euclídea. \footnote{Continua si la tomas como una función de $\real^N$ en $\real$}

\begin{theorem}[Relación norma $\leftrightarrow$ producto escalar]
$\md{\cdot}$ una norma cualquiera de $\real^N$ proviene de un producto escalar si y sólo si la norma satisface la identidad del paralelogramo.
\end{theorem}

\begin{proof}
En el apartado anterior (\ref{secNormaprodEsc}) demostramos la implicación hacia la derecha. Vamos a demostrar la recíproca:
Suponemos que la norma satisface la identidad del paralelogramo:

\begin{equation}
 \md{\ga+\gb}^2 + \md{\ga-\gb}^2 = 2 \md{\ga}^2 + 2\md{\gb}^2 \label{eqParalelogramo}
\end{equation}
Queremos probar que existe un producto escalar $\ast$ tal que $\md{\gx} = (\gx\ast \gx)^\frac{1}{2}$, así que definimos uno utilizando la identidad de polarización:

\begin{equation}
 \gx\ast\gy = \frac{1}{4} \left( \md{\gx+\gy} ^ 2 - \md{\gx-\gy} ^ 2\right) \label{eqPolarizacion}
 \end{equation}

Queremos probar que, efectivamente, $\ast$ es un producto escalar, así que tenemos que demostrar las siguientes propiedades:
\begin{enumerate}
 \item $\gx\ast\gy = \gy\ast\gx$ .
 \item $\gx\ast\gx \ge 0\quad \forall\; \gx$
 \item $(\gx\ast\gx) = 0 \dimplies \gx=\gor{0}$
 \item $(\lambda \gx) \ast \gy = \lambda\left(\gx\ast\gy\right)$
 \item $(\gx+\gy)\ast\gz =\gx\ast\gz + \gy\ast\gz $
\end{enumerate}

Las propiedades 1, 2 y 3 son triviales. Vamos con 4 y 5

\paragraph{Demostración de la 4ª propiedad}

Demostraremos que se cumple por inducción cuando $\lambda\in\nat$. Primero probamos para $\lambda = 2$.

\begin{align*}
(2\gx)\ast\gy = && \text{usando (\ref{eqPolarizacion})} \\
= \frac{1}{4} \left(|||2\gx+\gy |||^2 - |||2\gx-\gy |||^2\right) = && \\
= \frac{1}{4} \left(|||\underbrace{\gx}_a + \underbrace{\gx+\gy}_b|||^2 - |||\underbrace{\gx}_a+\underbrace{\gx-\gy}_{-b}|||^2\right) = && \text{usando (\ref{eqParalelogramo})} \\
= \frac{1}{4} \left(2|||\gx|||^2 + 2|||\gx + \gy|||^2\right) = && \\
= 2 \frac{1}{4} \left(|||\gx+\gy|||^2 - |||\gx-\gy|||^2\right) = 2 (\gx\ast\gy) &&
\end{align*}

Conclusión: si $\lambda = 2$ vemos que sale fuera y por lo tanto se cumple.

Paso 2 de la inducción: buscamos demostrar la propiedad con $\lambda = n$ con $n \in \mathbb{N}$

\begin{align*}
(n\gx)\ast\gy = && \text{usando (\ref{eqPolarizacion})} \\
= \frac{1}{4} \left(|||n\gx+\gy|||^2 - |||n\gx-\gy|||^2\right) = && \\
= \frac{1}{4} \left(|||\underbrace{(n-1)\gx}_a+\underbrace{\gx+\gy}_b|||^2
		- ||| \underbrace{(n-1)\gx}_a+ \underbrace{\gx-\gy}_b|||^2\right)= && \text{usando (\ref{eqParalelogramo})} \\
=...=2(\gx\ast\gy) + (n-2)(\gx\ast\gy) = && \text{usando hip. de inducción}\\
= n (\gx\ast\gy)
\end{align*}

Queda demostrado por lo tanto para $\lambda \in \nat$. Falta ahora demostrarlo para el resto de conjuntos de números.

\textbf{Para $\lambda \in \ent$} utilizaremos $(-\gx) \ast \gy = - (\gx\ast\gy)$ y podremos usar la demostración de los naturales.

\textbf{Para $\lambda = n \in \rac$} con $n = \frac{p}{q}$, siendo $p$ y $q$ primos entre sí, vemos que

\[ \left(\frac{p}{q}\gx\right)\ast\gy = \frac{q\left(\left(\frac{p}{q}\gx\right)\ast\gy\right)}{q} = \frac{\left(q\cdot\frac{p}{q}\gx\right)\ast\gy}{q} = \frac{\left(p\gx\ast\gy\right)}{q} \] que tal y como habíamos demostrado antes es igual a $ \dfrac{p\left(\gx\ast\gy\right)}{q} $, con lo que queda demostrado también para los racionales.

Por último, queremos demostrarlo cuando $\lambda \in \real$

$\lambda = \liminf{n} r_n$. Utilizaremos el resultado previo de que cualquier norma es continua.

$\gx, \gy$ fijos.

Revisar: Los $|||r_n \gx + \gy|||^2$ y  $|||r_n \gx - \gy|||^2$ son continuos.
$$\alpha \gx*\gy = \frac{1}{4}\left(||r_n \gx + \gy|||^2||| -|||r_n \gx - \gy|||^2||| \right) =$$
$$\lim_{n\to\infty} \left(||r_n \gx + \gy|||^2||| -|||r_n \gx - \gy|||^2||| \right) = \lim_{n\to\infty} (r_n\gx*\gy) = $$
$$\lim_{n\to\infty} r_n(\gx*\gy) = \alpha (\gx*\gy)$$

WTF es esto.

\paragraph{Demostración de la 5 propiedad:}
$$A = (\gx+\gy)*\gz = \frac{1}{4} \left( |||\gx+\gy+\gz|||^2 - |||\gx+\gy-\gz|||^2\right)$$
$$B =\gx*\gz = \frac{1}{4} \left( |||\gx+\gz|||^2 - |||\gx-\gz|||^2\right)$$
$$C =\gy*\gz = \frac{1}{4} \left( |||\gy+\gz|||^2 - |||\gy-\gz|||^2\right)$$
Demostraremos que $A-B-C=0$\\
COMPLETAR la comprobación.
\end{proof}

\begin{remark}
$d(\gx,\gy) = |||\gx-\gy||| \text{ para alguna norma }|||\cdot||| \dimplies (d(\gx+\gz)+d(\gy+\gz) = d(\gx,\gy) \wedge d(\lambda \gx,\lambda \gy = \abs{\lambda} d(\gx,\gy))$
\end{remark}

\subsection{Topología}
\begin{defn}[Bola] Se define la bola de radio $R$ centrada en el punto $\gx_0$ como
\[B_R(\gx_0) =\{\gx \in \real^N \tq \underbrace{d(\gx,\gx_0)}_{=\md{\gx-\gx_0}} < R \} \]
\end{defn}


Para evitar jaleos, al tratar la distancia vamos a tomar la norma euclídea. Como todas las normas son equivalentes, nos da igual tomar una que otra.
\begin{defn}[Conjunto\IS abierto] Un conjunto $A \subset \real^N$ es abierto si y sólo si $\forall\, \ga\in A\; \exists \varepsilon > 0 \tq B_\varepsilon(\ga) \subset A$
\end{defn}

\begin{defn}[Conjunto\IS cerrado] Un conjunto $B \subset \real^N$ es cerrado si y sólo si su complementario $B^c= \real^N-B$ es abierto.
\end{defn}

\begin{theorem}[Caracterización de cerrados en términos de sucesiones][Caracterización!por cerrados]\label{thmCerradoSucesiones} Un conjunto $B \subset \real^N$ es cerrado si y sólo si para cualquier sucesión convergente $\{x_n\} \subset B$ se cumple que  $\lim x_n \in B$.
\end{theorem}

\begin{theorem}[Operaciones con conjuntos abiertos y cerrados][]
Suponemos conjuntos de dimensión finita:
\begin{itemize}
 \item Unión arbitraria de abiertos $\rightarrow$ abierto
 \item Intersección finita de abiertos $\rightarrow$ abierto
 \item Union finita de cerrados $\rightarrow$ cerrado
 \item Intersección arbitraria de cerrados $\rightarrow$ cerrado
\end{itemize}
\end{theorem}

\begin{defn}[Punto\IS de acumulación]\label{defPtoAcc}
La idea intuitiva es aquellos puntos a los que puedo llegar en el límite, es decir, puntos que a su alrededor a una distancia arbitrariamente pequeña existen otros puntos del conjunto.
\[ A\subset \real^N,\; a \in (A) \dimplies  \forall \varepsilon > 0\; (B_{\varepsilon} (a) \setminus \{a\}) \cap A \neq \emptyset \]
Siendo $(A)$ es el conjunto de los puntos de acumulación.
\end{defn}

\begin{defn}[Frontera]
La frontera $∂A$ de un conjunto $A$ son aquellos puntos para los que en su entorno (para cualquier $\varepsilon$) hay puntos tanto del conjunto como puntos de fuera del conjunto.
\[ a \in ∂A \dimplies \forall \varepsilon>0 \tq B_\varepsilon (a) \cap A \neq \emptyset \y B_{\varepsilon} (a) \cap A^C \neq \emptyset \]
\end{defn}

\begin{defn}[Interior] El interior es el conjunto abierto más grande que está contenido en el conjunto $A$.\end{defn}
\begin{defn}[Cierre]\label{dfnCierre} El cierre de un conjunto $A$ es el conjunto cerrado más pequeño en el que está contenido $A$.\end{defn}

\begin{remark}
Cierre e interior no los vamos a definir formalmente porque se dan por supuesto.
\end{remark}

\begin{defn}[Conjunto\IS compacto]
\label{defCompacto}
Un conjunto que cumpla cualquiera de las 3 propiedades siguientes.
\end{defn}

\begin{theorem}[Conjunto\IS cerrado y acotado]\label{thmCerradoAcotado}
Sea $K \subset \real^N$. Son equivalentes:
\begin{enumerate}
 \item \label{propCerrado} K cerrado y acotado.
 \item \label{propSucesion} Para cualquier sucesión $\{x_n\} \subset K$, podemos encontrar una subsucesión convergente $\{x_{n_j}\} \subset\{x_n\}$ con $\lim x_{n_j} \in K$.
 \item \label{propRecubrimiento} Dado cualquier recubrimiento $\{A_i\}$ abierto de modo que $K \subset \cup \{A_i\}$ puedo encontrar un recubrimiento finito $\{A_j\}, j=1,...,M \tq K \subset \bigcup_{i=1}^M A_i$
\end{enumerate}
\end{theorem}

\begin{proof}

\paragraph{2 implica 1}  Supongamos que $K$ no estuviera acotado (negamos la propiedad \ref{propCerrado}). Consideremos una sucesión de vectores $\{x_n\}$ de tal forma que $\md{x_n} = n$, creciente y no acotada, pero con todos los elementos en $K$. Es imposible encontrar una subsucesión convergente, lo que contradice \ref{propSucesion}.

Si, por otra parte, $K$ no fuera cerrado, tendríamos que la frontera está fuera del conjunto, y podemos encontrar una sucesión $\{x_n\}$ con $\lim x_n \in ∂K$, lo que contradice \ref{propSucesion}.

\paragraph{1 implica 2} Empecemos por el caso sencillo, explorando una sucesión cualquiera $\{\gx_n\} \subset K \subset \real$, donde $K$ es, como decíamos en el enunciado, cerrado y acotado. Para encontrar una subsucesión convergente, usaremos el criterio de bisección.

\begin{center}
\begin{tikzpicture}
% a straight line segment
\draw (1,0) -- (10,0);
\foreach \x  in {1,...,10}
  \draw[xshift=\x cm] (0pt,2pt) -- (0pt,-1pt);
% the labels
\node[fill=white,draw=black,circle,inner sep=2pt,label=above:{$x_1$}] at (2.12,0) {};
\node[fill=white,draw=black,circle,inner sep=2pt,label=above:{$x_2$}] at (0.98,0) {};
\node[fill=white,draw=black,circle,inner sep=2pt,label=above:{$x_3$}] at (5.29,0) {};
\node[fill=white,draw=black,circle,inner sep=2pt,label=above:{$x_4$}] at (9,0) {};
\node[fill=white,draw=black,circle,inner sep=2pt,label=above:{$x_5$}] at (3.1,0) {};
\node[fill=white,draw=black,circle,inner sep=2pt,label=above:{$x_6$}] at (7,0) {};
\node[fill=white,draw=black,circle,inner sep=2pt,label=above:{...}] at (7.5,0) {};
\end{tikzpicture}
\end{center}

Escogemos el primer elemento $g_1$ de nuestra subsubcesión, y dividimos por la mitad el segmento.

\begin{center}
\begin{tikzpicture}
\draw (1,0) -- (10,0);
\foreach \x  in {1,...,10}
  \draw[xshift=\x cm] (0pt,2pt) -- (0pt,-1pt);
% the labels
\node[fill=black,draw=black,circle,inner sep=2pt,label=above:{$x_1$},label=below:{$g_1$}] at (2.12,0) {};
\node[fill=white,draw=black,circle,inner sep=2pt,label=above:{$x_2$}] at (0.98,0) {};
\node[fill=white,draw=black,circle,inner sep=2pt,label=above:{$x_3$}] at (5.29,0) {};
\node[fill=white,draw=black,circle,inner sep=2pt,label=above:{$x_4$}] at (9,0) {};
\node[fill=white,draw=black,circle,inner sep=2pt,label=above:{$x_5$}] at (3.1,0) {};
\node[fill=white,draw=black,circle,inner sep=2pt,label=above:{$x_6$}] at (7,0) {};
\node[fill=white,draw=black,circle,inner sep=2pt,label=above:{...}] at (7.5,0) {};

\draw[draw=red,ultra thick] (5.5,-1) -- (5.5,1);
\node[text=red] at (5.5,-1.3) {1};
\end{tikzpicture}
\end{center}

En al menos una de las dos mitades del segmento habrá infinitos términos: cogemos esa mitad y repetimos los mismos pasos. Finalmente, llegaremos a una subsucesión de este estilo:

\begin{center}
\begin{tikzpicture}
\draw (1,0) -- (10,0);
\foreach \x  in {1,...,10}
  \draw[xshift=\x cm] (0pt,2pt) -- (0pt,-1pt);
% the labels
\node[fill=black,draw=black,circle,inner sep=2pt,label=above:{$x_1$},label=below:{$g_1$}] at (2.12,0) {};
\node[fill=white,draw=black,circle,inner sep=2pt,label=above:{$x_2$}] at (0.98,0) {};
\node[fill=white,draw=black,circle,inner sep=2pt,label=above:{$x_3$}] at (5.29,0) {};
\node[fill=white,draw=black,circle,inner sep=2pt,label=above:{$x_4$}] at (9,0) {};
\node[fill=white,draw=black,circle,inner sep=2pt,label=above:{$x_5$}] at (3.1,0) {};
\node[fill=black,draw=black,circle,inner sep=2pt,label=above:{$x_6$},label=below:{$g_2$}] at (7,0) {};
\node[fill=black,draw=black,circle,inner sep=2pt,label=above:{$x_7$},label=below:{$g_3$}] at (7.5,0) {};
\node[fill=black,draw=black,circle,inner sep=2pt,label=above:{$x_9$},label=below:{$g_4$}] at (7.9,0) {};
\draw[draw=red,ultra thick] (5.5,-1) -- (5.5,1);
\node[text=red] at (5.5,-1.3) {$I_1$};

\draw[draw=red,ultra thick] (7.25,-0.75) -- (7.25,0.75);
\node[text=red] at (7.25,-1.15) {$I_2$};

\draw[draw=red,ultra thick] (8.125,-0.5) -- (8.125,0.5);
\node[text=red] at (8.125,-0.95) {$I_3$};

\draw[draw=red,ultra thick] (7.7,-0.25) -- (7.7,0.25);
\node[text=red] at (7.7,-0.8) {$I_4$};
\end{tikzpicture}
\end{center}

Nuestra subsucesión $\{g_x\}$ es igualmente infinita. Tal y como la hemos definido, tenemos que cada $g_i$ está en un intervalo $(I_i, I_{i-1})$ que cada vez se hace más pequeño. Es decir, que la subsucesión $\{g_x\}$ es de Cauchy y, por lo tanto convergente.

Ahora sólo queda ver cómo podríamos obtener esa subsucesión cuando estamos en espacios que no sean $\real^N$. La idea es sencilla: primero, buscamos una subsucesión que converja en la primera coordenada. Dentro de esa subsucesión, buscamos otra subsucesión que converja además en la segunda, y así con las $N$ coordenadas.
\end{proof}

\begin{theorem} \label{thmCompactoMax} Sea $K\subset \real$ un conjunto compacto. Entonces, si $\appl{f}{\real}{\real}$ es continua en $K$ existen  $x_m,x_M \in K \tq F(x_m) \leq F(x) \leq F(x_M)\;\forall x \in K$.

Es decir, si $F$ es continua en $K$ alcanza su máximo y su mínimo en el conjunto.
\end{theorem}

\paragraph{Aplicación:}
$F(\gor{x}) = |||\gor{x}|||$ una norma (que ya sabemos que es continua):

\emph{Conclusión:} $m \md{x} \leq |||\gor{x}||| \leq C||\gor{x}||$

\begin{theorem}
En $\real^N$ TODAS las normas son equivalentes.
\end{theorem}

\subsubsection{Conexión}
\begin{defn}[Conexión\IS por caminos]
Dados $a,b \in C$ podemos encontrar una aplicación continua $\appl{\varphi}{[0,1]}{\real^N}$ tal que $\varphi(0) = a$ y  $\varphi(1) = b$ con $ \varphi(t) \in C\, \forall t \in [0,1]$.

Es decir, $C$ es conexo por caminos si podemos encontrar una "línea", un camino que una dos puntos cualquiera del conjunto y que además no se salga del conjunto.
\end{defn}

\begin{defn}[Conexión\IS por abiertos]
$C$ es conexo por conjuntos si para cualquier par de abiertos $A,B \subset \real^N \tq C\subset A\cup B$ se cumple que, si $A\cap C\neq \emptyset \y B\cap C \neq \emptyset $ entonces $ A\cap B \neq \emptyset$.

Esto es equivalente a decir que $C$ no puede ser expresado como unión de dos conjuntos disjuntos.
\end{defn}


\begin{remark}

\begin{figure}[hbtp]
\label{imgPeine}
\begin{center}
\begin{tikzpicture}

\draw (1,0) -- (10,0);

\foreach \x  in {2,...,20}
  \draw ($10/\x*(1,0) + (0.49,0)$) -- ($(0.49,3) + 10/\x*(1,0)$);

\node[fill=white,draw=black,circle,inner sep=2pt] at (1,0) {};

\end{tikzpicture}
\caption{Conjunto peine}
\end{center}
\end{figure}

Es curioso comprobar que estas 2 definiciones no son equivalentes. Tomemos el conjunto peine (figura \ref{imgPeine})
\[ \left\{(x,0), x\in (0,1]\right\} \cup \{(0,y), y \in (0,1]\} \cup \left\{\bigcup_{n=1}^{\infty}{\left(\frac{1}{n},y\right), y \in [0,1]}\right\} \]

Es un conjunto conexo por abiertos porque no podemos separarlo en dos conjuntos disjuntos. Sin embargo, no es conexo por caminos porque, si queremos ir del punto $(0,1)$ al $(0,0.5)$ no podemos hacerlo ya que el único camino pasaría por el punto $(0,0)$, que no está en el conjunto.
\end{remark}

\subsection{Funciones continuas, abiertos y cerrados}

 Al tener definida una norma de vectores podemos definir convergencia y continuidad:

\begin{defn}[Convergencia] Se dice que $\gx_n$ converge a $\gx$ (notación: $\gx_n \to \gx$) si

\[  \forall \varepsilon > 0\; \exists n_0 \tq n > n_0 \implies \md{\gx-\gor{x}_n}<\varepsilon \]

\end{defn}

\begin{defn}[Función\IS continua] Sea $\appl{F}{\real^N}{\real^M}$. Se dice que $F$ es continua en $a$ si y sólo si

\[  \forall \varepsilon > 0 , \exists \delta > 0 \tq \md{\gx-\ga}_a < \delta \Rightarrow \md{F(\gx)-F(\ga)}_b< \varepsilon \]
\label{dfnContinua}
\end{defn}

\begin{remark} Es interesante ver que se puede hablar de continuidad tomando una norma en $\mathbb{R}^N$ y otra distinta en $\real^M$ sin por ello variar la definición de continuidad, teniendo en cuenta que todas las normas son equivalentes. \end{remark}

A partir de esta definición podemos estudiar qué hacen las funciones continuas con conjuntos abiertos y cerrados. Sea $F$ continua. Contrario a lo que podríamos intuir,

\begin{enumerate}
\item A abierto no implica que  $F(A)$ sea abierto.
\item B cerrado no implica que $F(B)$ sea cerrado.
\end{enumerate}

Empezamos definiendo en qué consiste una función inversa:

\begin{defn}[Función\IS inversa] Dada \[\appl{F}{\real^N}{\real^N}\], definimos su inversa como
\[ \inv{F}(A) = \left\{\gor{x}\in \real^N \tq F(\gor{x})\in A\right\} \]
\end{defn}

A partir de aquí podemos extraer dos conclusiones que sí nos ayudarán a discernir si un conjunto imagen es abierto y cerrado.

\begin{theorem}[Función\IS inversa]\par\noindent\par
\label{thmInversa}
\begin{itemize}
\item F continua y A abierto $\implies A=F^{-1} (B)$ abierto.
\item F continua y B cerrado $\implies A=F^{-1} (B)$ cerrado.
\end{itemize}
\end{theorem}

Este teorema nos sirve para decir fácilmente si un conjunto es abierto o cerrado. Por ejemplo, consideremos
 \[ M=\{(x,y,z) \in \real^3 \tq x^2 + \cos\left(x\abs{y}\right) - e^z < 1 \} \]

Podemos definir ahí la función $F$ como
\[ F(x,y,z) = x^2 + \cos\left(x\abs{y}\right) - e^z\]

que va de $\real^3$ a cierto conjunto $A = \{ a \in \real \tq a < 1 \}$. Podemos reescribir $M$ como
\[M=\{(x,y,z) \in \real^3 \tq  F(x,y,z) \in A\}\]

o, de otra forma, $M = \inv{F}(A)$. Según el teorema (\ref{thmInversa}), como $A$ es abierto entonces $M$ también es abierto.

\begin{proof} Demostramos las dos implicaciones que hemos enunciado.

1) Dado un $\gor{x} \in F^{-1} (A)$ queremos hallar un $R>0$ tal que $B_R(\gor{x})\subset F^{-1} (A)$. Partimos de
\[\gor{x}\in F^{-1} (A) \dimplies F(\gor{x})\in A\]

Como $F$ es continua, $\exists \varepsilon>0 \tq B_{\varepsilon}(F(\gor{x}))\subset A$. Esto es equivalente a decir que, para cualquier $\gz$
\[ ||\gor{z}-F(\gor{x})|| < \varepsilon \implies \gor{z}\in A\]

Por la definición de continuidad (\ref{dfnContinua}), dado un $\gor{s}\in B_R(\gor{x})$

\[ \exists \delta > 0 \tq ||\gor{x}-\gor{s}||<\delta \implies ||F(\gor{x})-F(\gor{s})||< \varepsilon \]


y por lo tanto $F(\gor{s}) \in A$ y $\gor{s} \in F^{-1} (A)$.
Conclusión: Hemos encontrado un $\delta > 0$ tal que $s \in B_R(\gor{x}) \implies s \in F^{-1} (A)$.
\end{proof}

\section{Aplicaciones lineales y matrices}

\subsection{Aplicaciones lineales}

\begin{defn}[Aplicación\IS lineal]

Sea: $\appl{L}{\real^N}{\real^M}$. Entonces, $L$ es lineal si y sólo si

\[ L(\lambda \gor{x}) = \lambda L(\gor{x}) \]
\[ L(\gor{x}+\gor{y}) = L(\gx)+L(\gy)\]

\end{defn}
Además, toda aplicación lineal se puede escribir en forma de matriz.

\[L(\gor{x})=A\gor{x} =
\begin{pmatrix}
a_{11} 	& \cdots & a_{1n}		\\
\vdots	& \ddots &  \vdots 	\\
a_{n1}	& \cdots & a_{nn}
\end{pmatrix}\]

\begin{theorem}
Toda aplicación lineal $L$ es continua.
\end{theorem}
\begin{proof} Partiendo de la definición de continuidad (\ref{dfnContinua}), $L$ es continua si y sólo si

\[ \forall \ga, \gx \; \forall \epsilon > 0 \; \exists \delta > 0 \tq \md{\ga - \gx} < \delta \implies \md{L\ga - L\gx} < \epsilon \]

Sabemos que $\md{A\gx} ≤ C\md{\gx}$ para alguna constante $C$. Podemos reescribir

\[ \md{L\ga - L\gx} = \md{L(\ga-\gx)} ≤ C\md{\ga-\gx} \]

Entonces, la igualdad se cumple si tomamos $\epsilon = C\delta$.
\end{proof}

\subsection{Norma de matrices}
Consideramos una aplicación continua

\begin{align*}
\appl{F}{\real^N&}{\real} \\
\gor{x} &\longrightarrow F(\gx) = \underbrace{||A\gx||}_{L(\gx)}
\end{align*}

Sabemos que existe $C>0$ tal que $||A\gx|| \leq C||\gx||$, es decir,  $||A\gx||\leq C$ si $||\gx||=1$. Queremos saber cuál es la mejor constante que podemos encontrar, la que más se ajuste. Consideramos el conjunto $M$ de todos los vectores de la esfera unidad, es decir

\[ M = \{||A\gx|| \tq ||\gx||=1\}\subset \real \]

Entonces mejor constante $C$ es la cota superior mínima (supremo) que vamos a llamar $\alpha$. Al ser $F$ continua y $M$ compacto, sabemos que el supremo $\alpha \in M$.

\begin{defn}[Norma\IS de una matriz]
$$\norm{A} = \alpha = \max{\norm{A\gx} \tq \norm{\gx} =1}$$
\end{defn}

\begin{proof} Hay que demostrar que esta norma que hemos definido cumple las propiedades de una norma (\ref{defnNorma}). Las dos primeras son triviales, demostremos la desigualdad triangular
\[ \norm{A+B} = \max{\norm{(A+B)\gx}} = \norm{(A+B)\gx_{A,B}} \]

donde $\gx_{A,B}$ es el vector que da el valor máximo para esa multiplicación. Usando la propiedad asociativa

\[  \norm{(A+B)\gx_{A,B}} = \norm{A\gx_{AB} + B\gx_{A,B}} ≤ \norm{A\gx_{A,B}} + \norm{B\gx_{A,B}} \]

Sabemos que existen dos vectores $\gx_A$ y $\gx_B$ que maximizan el resultado $\norm{A\gx_A}$ y $\norm{A\gx_B}$ respectivamente, por lo tanto

\[ \norm{A\gx_{A,B}} + \norm{B\gx_{A,B}} ≤ \norm{A\gx_A} + \norm{B\gx_B} = \norm{A} + \norm{B} \]

\end{proof}

Basándonos en lo que hemos obtenido, calculamos la norma uno de
\[A = \begin{pmatrix}
      1&2\\-3&1\\2&0
     \end{pmatrix}\]

Tenemos que maximizar, sabiendo que $|x|+|y| = 1$:

\[ |x+2y| + |-3x+y| + |2x| \leq |x|+|2y| + |3x| + |y| + 2|x| = 6|x|+3|y| \leq 6 (|x|+|y|) =6 \]
¿Podemos encontrar un vector $\gx = (x_0,y_0)$ tal que $||A(x_0,y_0)^T||_1 = 6$?\\
Tomando $x_0 = 1$ y $y_0 = 0$ lo encontramos. Como $\gx$ está en la esfera unidad y es una cota, es el máximo y por lo tanto la norma que buscamos.

Curiosamente, \textbf{coincide con la suma de los valores absolutos de las columnas} y escoger el más grande.

Si tomamos la norma infinito de
\[A = \begin{pmatrix}
      1&2\\-3&1\\2&0
     \end{pmatrix}\]

Tenemos que \textbf{coincide con el máximo de las posibles sumas de los valores absolutos de las filas}.



Queremos buscar ahora cuánto vale la norma de una matriz cuando usamos la norma euclídea. Usaremos los dos lemas siguientes para apoyarnos.

\begin{lemma}
 Sea A una matriz cualquiera, entonces $\trans{A}A$ es simétrica.
\end{lemma}
\begin{lemma}
 \[ \underbrace{\pesc{\gx,A\gy}}_{\text{Producto en } \real^n} = \underbrace{\pesc{A^T \gx,\gy}}_{\text{Producto en } \real^M} \]
\end{lemma}

Tenemos $A^TA$ diagonalizable, de dimensión $N \times N$. Buscamos cuánto vale $\norm{A\gx}$ con  $\gx \in \real^N$. Empezamos desarrollando el vector en una base ortonormal de  $A^T A$: \[ \gx = \sum \alpha_i \gv_i \] y por lo tanto \[ ||\gx|| = \sum \alpha_i^2 \pesc{\gv_i,\gv_i}\].

 Desarrollamos el producto \[\trans{A}A\gx = \trans{A}A\left(\sum \alpha_i \gv_i\right) = \sum \left(\alpha_i\lambda_i\gor{v}_i\right) \] donde $\lambda_i$ son los autovalores de $\trans{A}A$.

 Ahora queremos hallar el máximo de $||A\gx||$ cuando $||\gx|| = 1$:

 \[ ||A\gx||^2 = \pesc{A\gx,A\gx} = \pesc{\trans{A}A\gx,\gx} = \pesc{\sum \lambda_i \alpha_i \gv_i,\sum\alpha_i \gv_i} \]

 Como la base de $\{\gv_n\}$ es ortonormal, $\pesc{\gv_i, \gv_j} = 0$ si $i≠j$, por lo tanto sólo nos queda
 \[ \pesc{\sum \lambda_i \alpha_i \gv_i,\sum\alpha_i \gv_i} = \sum \lambda_i \alpha_i^2 \leq \lambda_{max} \left(\sum \alpha_i^2\right) = \lambda_{max} \]

 teniendo en cuenta que $\norm{\gx} = 1$ y donde $\lambda_max$ es el autovalor máximo. Es decir, hemos llegado a que
 \[ \max\norm{A\gx} ≤ \sqrt{\lambda_{max}} \]

 Hemos definido una cota para $\norm{A\gx}$. Ahora bien, esa cota se alcanza cuando $\gx$ es el autovector asociado a $\lambda_{max}$, por lo tanto la cota es un máximo y la norma de la matriz.

 \section{Límites}

 \begin{defn}[Límite] Dada una función $\appl{F}{\real^N}{\real^M}$, definimos su límite cuando $\gx\to\ga$ de la siguiente forma:
  \[ \lim_{\gx \rightarrow \ga} F(\gx) = \gor{L} \dimplies \forall \varepsilon > 0,  \exists \delta>0 \tlq 0<||\gx-\ga|| <\delta \implies ||F(\gx) - L||<\varepsilon\]
 \end{defn}

 Importante el detalle de $0 < ||\gx-\ga||$, no es un $\leq$, porque no se necesita que la función esté siquiera definida en el punto $\ga$.

 \begin{theorem}[Convergencia\IS de coordenadas]

  Sean $\gor{x}_n = (x_1,...,x_n) \in \real^N$ y $\gor{L} = (L_1,...,L_n) \in \real^N$. Entonces

  \[ x_n \rightarrow \gor{L} \dimplies (x_1 \rightarrow L_1) \y (x_2 \rightarrow L_2) \y ... \y (x_n \rightarrow L_n) \]
 \end{theorem}

 Idea para el cálculo de límites:
 \begin{itemize}
  \item $\displaystyle\mylim{x}{a}{x} = \lim_{\gy\rightarrow 0} F(\gy+\ga)$.
  \item Límite a lo largo de rectas. $\displaystyle\mylim{x}{a}{\gx} \sim \lim F({t\gor{v}})$

 \end{itemize}

 Si $\displaystyle\lim F({t\gor{v}})$ toma valores distintos dependiendo de $\gor{v}$ entonces $\nexists \displaystyle\mylim{x}{0}{\gx}$

Por otra parte, si $\forall t \in \real, \mylim{x}{a}{t\gor{v}} = L$, entonces $\gor{L}$ es el candidato a ser el límite (no tiene por qué serlo). El siguiente paso sería demostrar con argumentos de comparación (Sandwich) u otros que $\mylim{x}{a}{\gx} = L$.

 El contraejemplo para ver que la existencia del límite por rectas no implica la existencia del límite es estudiar la función \[ f(x,y) = \frac{x y^2}{x^2 + y^4}\] . Veamos por qué.

 Si os acercamos al límite por medio de rectas:

 \[ f(x,y) = f(x,mx) = \frac{x\cdot(mx)^2}{x^2 + (mx)^4} = \frac{m^2x^3}{(1 + x^2m^4)x^2} \]
 \[ \lim{x\to 0} (f(x,mx)) \rightarrow 0, \forall m \in \real \]

 Pero si nos acercamos al límite por medio de $x = y^2$ tenemos:

\[ f(x,y) = f(y^2,y) = \frac{y^2y^2}{y^4+y^4} = \frac{y^4}{2y^4} = \frac{1}{2} ≠ 0\]

Por lo tanto, el límite no existe a pesar de que existe cuando nos acercamos por rectas.


\begin{theorem}
 $F$ es continua si y sólo si para cualquier abierto $A$, $F^{-1}(A)$ es abierto.
\end{theorem}

\begin{proof}
De este teorema ya teníamos demostrada la implicación a la derecha (\ref{thmInversa}), así que sólo falta demostrar hacia la izquierda. Queremos probar que

\[ \forall \varepsilon > 0\; \exists \delta>0 \tlq ||\gx-\ga||<\delta \implies ||F(\gx)-F(\ga)||<\epsilon \]

Tomamos  \[ A = B_{\varepsilon}(F(\ga))\] de tal forma que \[ F(\ga) \in A \implies \ga \in F^{-1}(A) \]

Por hipótesis, $F^{-1}(A)$ abierto y $\ga \in F^{-1}(A)$ . Entonces
\[\exists B_{\delta}(\ga) \subset F^{-1}(A) \].Es decir, \[ \gor{s}\in B_{\delta}(\ga) \subset F^{-1}(A), s\in F^{-1}(A) \implies F(s) \in A = B_{\varepsilon}(F(\ga))\]
\end{proof}

\begin{remark}
Este teorema también se cumple para cerrados.
\end{remark}

--------------------------------------------------


\section{Diferenciación}

\begin{defn}[Función\IS diferenciable]
 $F$ es diferenciable en $\gor{a}$ si existe una aplicación lineal $L$ tal que

\[ \frac{F(\gx)-F(\ga)-L(\gx-\ga)}{||\gx-\ga||} \convs[][\gx][\ga] 0 \]

que se puede expresar como
\[ \lim_{\gor{h} \rightarrow \gor{0}} \frac{\md{F(\ga+\gor{h}) - F(\ga) - L\gor{h}}}{||\gor{h}||} = 0 \]
\end{defn}

\begin{defn}[Diferencial]
A esa matrix $L$ la vamos a llamar la diferencial de $F$ en $\ga$:

\[ L\equiv DF(\ga) \]
\end{defn}

\begin{theorem}
$$F \text{ diferenciable en } \ga \implies F \text{ continua en } \ga$$
\end{theorem}

\begin{proof}
 $$\lim_{\gor{h} \rightarrow \gor{0}} \frac{\md{F(\ga+\gor{h}) - F(\ga) - L\gor{h}}}{\md{\gor{h}}} = 0$$
 Esta es la definición de diferenciable. Para que este límite sea 0, el numerador tiene que tender a 0, por lo que $F(\ga+\gor{h}) - F(\ga) \rightarrow 0$
\end{proof}


\begin{theorem}
Si la diferencial existe, entonces es única.
\end{theorem}

\begin{proof}  Vamos a demostrar que esa aplicación $L$ es única. Supongamos que existen $L_1,L_2$ que cumplen las condiciones.
\[0=\lim_{\gor{h} \rightarrow \gor{0}} \frac{F(\gor{a}+\gor{h}) - F(\ga)-L_1\gor{h}}{||\gor{h}||} = \lim_{\gor{h} \rightarrow \gor{0}} \frac{F(\gor{a}+\gor{h}) - F(\ga)-L_2\gor{h}}{||\gor{h}||}\].

Sumando:

\[ 0 = \lim_{\gor{h} \rightarrow \gor{0}} \frac{||F(\gor{a}+\gor{h}) - F(\ga)-L_1\gor{h}|| + ||F(\gor{a}+\gor{h}) - F(\ga) -L_2\gor{h}||}{||\gor{h}||} \]

Teniendo en cuenta que $||A-B|| = ||A+(-B)|| \leq ||A||+||B||$

\[ 0 \leq \lim_{\gor{h} \rightarrow \gor{0}} \frac{2\cdot\md{F(\ga + \gor{h}) - F(\ga)} + \md{L_1\gor{h}} + \md{L_2\gor{h}}}{\md{\gor{h}}} \]

\textit{Aquí falta completar.}
\end{proof}



\paragraph{Nomenclatura: }
Aproximación lineal $\sim$ Diferencial.

Matriz jacobiana $\sim$ Jacobiana.

\begin{defn}[Matriz\IS diferencial]
 Matriz asociada a $DF(\ga) \equiv $ Matriz de las derivadas parciales de F.

 $$DF(\ga) \equiv \begin{pmatrix}
                \dpa{F_1}{x_1} & \cdot & \dpa{F_1}{x_N}\\
                \vdots& \ddots & \vdots\\
                \dpa{F_N}{x_1} & \cdot & \dpa{F_N}{x_N}
                \end{pmatrix}$$
\end{defn}

\begin{theorem}
 $F$ diferenciable en $\ga \implies \exists \deriv{F_k}{x_i}(\ga), i=1,2,...,N \y k = 1,2,...,M$
\end{theorem}

El contraejemplo para demostrar la implicación a la izquierda es el mismo que en los límites a lo largo de rectas.

$f(x,y) = \left\{ \begin{matrix}
\displaystyle\frac{xy^2}{x+y^2} & (x,y) \neq (0,0) \\
0 & (x,y)=(0,0)
          \end{matrix}\right.
$

Según las aplicaciones que tengamos, la diferencial se suele llamar de una u otra forma. Con $\appl{\delta}{\real}{\real^M}$ utilizamos notación vectorial en vez de matricial porque tendríamos una matriz columna. Por ejemplo: la velocidad (en un instante de tiempo, un punto en el espacio).

\begin{defn}[Gradiente] Sea $\appl{F}{\real^N}{\real}$, entonces definimos el vector gradiente como

\[ \grad F(\gx) = DF(\gx) = \left(\dpa{F}{x_1}, \dpa{F}{x_2},\dotsc, \dpa{F}{x_n}\right) \]
\end{defn}


\subsection{Regla de la cadena}
\index{Regla!de la cadena}
Consideremos la composición de dos funciones de la siguiente forma:

$\appl{F}{\real^N}{\real^M}$.

$\appl{G}{\real^M}{\real^K}$.

$\appl{H=G\circ F}{\real^N}{\real^K}$.

$ \gx \in \real^N, \gy \in \real^M$

\begin{wrapfigure}{r}{0.3\textwidth}
\begin{center}
\begin{tikzpicture}
\draw[->] (-0.1,0.2) -- (-0.1,1.7);
\draw[->] (0.3,1.9) -- (1.6,1.9);
\draw[->] (0.3,0.2) -- (1.7,1.7);

\node at (0,0) {$\real^N$};
\node at (0,2) {$\real^M$};
\node at (2,2) {$\real^K$};

\node[left] at (-0.1,1) {$F$};
\node[above] at (1,2) {$G$};
\node[below right] at (1,1) {$H = G\circ F$};
\end{tikzpicture}
\end{center}
\caption{Composición de funciones}
\end{wrapfigure}

Con $F$ diferenciable en $\ga$ y $G$ diferenciable en $F(\gor{a})$. Entonces $H=G\circ F$ es diferenciable en $\ga $.
Además la expresión matricial es:

\[ \underbrace{DH(\ga)}_{K\times N} = \underbrace{DG(F(\ga))}_{K\times M}\cdot \underbrace{DF(\ga)}_{M\times N} \]

No hace falta calcular toda la matriz si sólo queremos un elemento. Para calcular 1 único elemento de la matriz diferencial (el de la fila $i$, columna $j$), usamos la siguiente fórmula
\[ \dpa{H_i}{x_j}(\ga) = \sum_{k=1}^M \dpa{G_i}{y_k}\cdot\dpa{F_k}{x_j} \]

Siempre teniendo en cuenta que $\displaystyle\dpa{G_i}{y_k}$ está evaluado en $F(\ga)$ y $\displaystyle\dpa{F_k}{x_j}$ está evaluado en $\ga$.

\subsection{Extensiones del Teorema del Valor Medio}

El teorema anterior que vimos del valor medio era para funciones de una variable, y proponía lo siguiente:
\begin{theorem}[Teorema\IS del valor medio (una variable)]
\label{thmTVM1var}
Dada $\appl{f}{\real}{\real}$ diferenciable, se tiene que \[ f(b)-f(a) = f'(c)(b-a)\] para algún $c\in[a,b]$
\end{theorem}

Después el teorema lo extendimos a funciones de $\real^N$ en $\real$: dada $\appl{F}{\real^N}{\real}$ entonces definíamos

 \[ \sigma(t)  = t\gor{b}+(1-t)\gor{a} \]

 y $g = F\circ \sigma$ era una aplicación de los reales a los reales, y entonces aplicando el teorema anterior teníamos que

 \[ F(\gor{b}-\gor{a}) = g(1)-g(0)  = g'(s) \]
 para algún $s\in[0,1]$.

Sin embargo, al tratar de extrapolar este resultado a una función $\appl{F}{\real^N}{\real^2}$ nos queda que

 \[ F(\gor{b})-F(\ga) = \begin{pmatrix}
                         \pesc{\nabla F_1(\gor{c_1}),{\gor{b}-\ga}}\\
                         \pesc{\nabla F_2(\gor{c_2}),\gor{b}-\ga}
                        \end{pmatrix}
 \]
  Tenemos 2 $c$ distintos, uno para cada $f$, por lo que este teorema pierde sentido. Hay que buscar una extensión, otra formulación del teorema que nos permita aplicarlo a las funciones que estamos estudiando.

  \begin{theorem} [Teorema\IS del valor medio (varias variables)]
  \label{thmTVM}
  Sea $f \in C^1$ en un abierto que contenga $[a,b]$. Entonces

  \[ \norm{F(\gor{b})-F(\ga)} \leq \md{DF(\gor{c})} \cdot \md{\gor{b}-\ga} \]

  Siendo $c$ un punto del segmento que une $\ga$ y $\gb$ en el que $\md{DF(tb+(1-t)a)}$ alcanza su máximo.
  \end{theorem}

  \begin{proof}

Primero vamos a demostrar la siguiente desigualdad:

\begin{equation}
\label{eqnTVM1}
 \md{\int_0^1 F(t) \,dt}≤ \int_0^1 \md{F(t)}\,dt
\end{equation}

Si tomamos \[ L = \int_0^1 F(t) \,dt \]  entonces

\[ \md{L}^2 = \md{\int_0^1 F(t) \,dt}^2 = \pesc{L,\int_0^1 F(t) \,dt} \]

Como $L$ es un vector constante, podemos meterlo en la integral y tenemos que

\[ \pesc{L,\int_0^1 F(t) \,dt} = \int_0^1 \pesc{L, F(t)} ≤ \int_0^1 \md{L}\md{F(t)} = \md{L} \int_0^1 \md{F(t)} \]

y por lo tanto

\begin{gather*}
\md{L}^2 ≤ \md{L} \int_0^1 \md{F(t)} \\
\md{L} ≤ \int_0^1 \md{F(t)} \\
\md{\int_0^1 F(t) \,dt } ≤ \int_0^1 \md{F(t)}
\end{gather*}

quedando así demostrada la desigualdad (\ref{eqnTVM1}).

Consideramos ahora

\[ \md{F(\gb) - F(\ga)} \]

Si integramos $DF$ por el camino que va de $\ga$ a $\gb$ nos queda que

\[ \md{F(\gb) - F(\ga)} = \md{\int_0^1 DF\left[\ga(1-t) + t\gb\right](\gb - \ga)\, dt } \]

que por (\ref{eqnTVM1})

\[ \md{F(\gb)-F(\ga)} ≤ \int_0^1 \md{DF\left[\ga(1-t) + t\gb\right](\gb - \ga)}\, dt  \leq  \int_0^1 \md{DF\left[\ga(1-t) + t\gb\right]}\md{\gb - \ga}\, dt \]

Nos fijamos en $\md{DF\left[\ga(1-t) + t\gb\right]}$. Al ser continua y estar definida en un conjunto compacto, entonces alcanza su máximo en algún punto $\gor{c}$ entre $\ga$ y $\gb$, por lo tanto

\[ \md{F(\gb) - F(\ga)} ≤  \int_0^1 \md{DF(\gor{c})}\md{(\gb - \ga)} = \md{DF(\gor{c})}\md{\gb - \ga} \]
  \end{proof}

Este teorema nos sirve, por ejemplo, para ver que si tenemos $\appl{F}{\real^N}{\real^M}, F \in C^1$, definida en un conjunto abierto y conexo y  $DF(\gx) \equiv 0\; \forall\gx$, entonces $F$ es constante.

\subsection{Derivada direccional}

$\appl{F}{\real^N}{\real^M}$ (escalar)

$\ga \sim$ Recta que pasa por $\ga$ con dirección $\gor{v}$.

$r(t) = \ga + t\gor{v}$.

\obs
Como una recta tiene infinitos vectores directores (dependiendo de la longitud), siempre tomaremos vectores directores unitarios, con $\norm{\gor{v}} = 1$.


Vamos a estudiar: $g(t) = F(\ga + t\gor{v}) = F \circ r (t)$.

$t \sim 0 \dimplies \ga + t\gor{v} \sim \ga$
\begin{defn} [Regla de la cadena]
$$g'(0) = \displaystyle\lim_{h \rightarrow 0} \frac{g(h)-g(0)}{h} = \displaystyle\lim_{h \rightarrow 0} \frac{F(\ga+h\gor{v})-F(\ga)}{h} \equiv D_{\gor{v}}F(\ga)$$.
\end{defn}

\obs
La existencia de $D_{\gor{v}}F(\ga), \forall \gor{v}\in \real^N$ NO garantiza que $F$ sea derivable.


Si sabemos que $F$ SÍ es diferenciable podemos usar la regla de la cadena obteniendo:

$D_{\gor{v}}F(\ga) = g'(0) = D(F\circ r)(0) = ... = \pesc{\nabla F(\ga),\gor{v}}$


\paragraph{Aplicación:}
\begin{itemize}
 \item
 Dirección de máximo crecimiento:

$D_{\gor{v}}F(\ga) = \pesc{\nabla F(\ga),\gor{v}}\leq \norm{\nabla F(\ga)}\cdot \underbrace{\norm{\gor{v}}}_{\equiv 1}$

Conclusión:
\begin{align*}
D_{\gor{v}}F(\ga) &\leq \norm{\nabla F(\ga)}\\
&\uparrow\\
\text{El }= \text{se obtien}&\text{e cuando }\gor{v} = \displaystyle \frac{\nabla F(\ga)}{\norm{\nabla F(\ga)}}.
\end{align*}


 \item
 Vector perpendicular a los conjuntos de nivel

 $\appl{F}{\real^N}{\real^M}$

 $S = \{ \gx \in \real^N \tq F(\gx) = 0\}$ (Conjunto de nivel)

 $\ga \in S$

 Entonces: $\nabla F(\ga) \perp S$
\end{itemize}

\begin{theorem}[Derivadas parciales continuas implican función diferenciable]
Si existen todas las derivadas parciales y son continuas $\implies F$ diferenciable en $\ga$.

\end{theorem}

Contraejemplo de la no reciprocidad: $f(x) = x^2 sin\left(\frac{1}{x}\right)$

\begin{proof}
 $\appl{F}{\real^2}{\real}$

 $$¿\frac{\left|F(a+a,b+k) - F(a,b) - \deriv{F}{x}(a,b) h - \deriv{F}{y}(a,b)k\right|}{\norm{(h,k)}}\longrightarrow 0?$$

 Sumamos y restamos al numerador $F(a,b+k)$.

 $$\frac{\left|\left(\underbrace{F(a+h,b+k) - F(a,b+k)}_{\deriv{F}{x}(a+\tilde{h},b+k) \text{ para algún } 0 \leq\tilde{h}\leq h} -  \deriv{F}{x}(a,b) h\right) + \left(\underbrace{F(a,b+k) - F(a,b)}_{\deriv{F}{x}(a+h,b+\tilde{k}) \text{ si } 0 \leq\tilde{k}\leq k}- \deriv{F}{y}(a,b) k\right)\right|}{\sqrt{h^2+k^2}}$$

 $$0\leq\frac{\left|\deriv{F}{x}(a+\tilde{h},b+k)-\deriv{F}{x}(a,b)\right| \cdot |h| + \left| \deriv{F}{y}(a,b+\tilde{k}) - \deriv{F}{y}(a,b)\right| \cdot |k|}{\sqrt{h^2+k^2}} = (*)$$

 Aquí es donde aplicamos que las derivadas parciales son continuas: como $h$ y $k$ son pequeños (por lo tanto $\tilde{h}<h$ también lo será) los puntos $(a,b)$ y $(a+h,b+k)$ también están cerca, por lo que sus imágenes por la derivada estarán también cerca, es decir, $|\deriv{F}{x}(a,b)-\deriv{F}{x}(a+\tilde{h},b+k)| \rightarrow 0$ y lo mismo con la otra.

 Conclusión:

 \begin{align*}
0 \leq (*) \leq \varepsilon \frac{|h|+|k|}{\sqrt{h^2+k^2}} &\leq C\varepsilon \rightarrow 0 \text{ cuando } \gor{h},\gor{k} \rightarrow \gor{0}\\
&\uparrow\\
\text{El numerdador es la} & \text{ norma 1 y el denominador la norma 2.}\\
\text{En } \real^N &\text{ todas las normas son equivalentes.}
 \end{align*}


\end{proof}


\subsection{Derivadas iteradas}

\paragraph{Notación:}

$\deriv{}{y}\left(\deriv{f}{x}\right) \equiv \deriv{^2f}{x \partial y}$

\begin{theorem}[Euler (orden de las derivadas)]
Si las derivadas segundas son continuas, entonces:
$$\deriv{^2f}{x_i\partial x_j} = \deriv{^2 f}{x_j \partial x_i}$$
\end{theorem}

\input{CALII/maximos_minimos_calculo2.tex}

\section{Desarrollo de Taylor}
\index{Polinomio!de Taylor}
Tenemos una función $\appl{F}{\real^N}{\real}$, con $F\in C^k$ ($k$ veces derivable), y queremos el desarrollo de Taylor de $F$ alrededor de $\ga \in \real^N$.

En dimensión 1, el desarrollo era el que sigue

\[ g(x) = g(0) + g'(0)x + \frac{g''(0)}{2!}x^2 + ... + \frac{g^{k)}(0)}{k!}x^k + \underbrace{\frac{g^{k+1)}(s)}{(k+1)!}x^{(k+1)}}_{\text{error}} \]

Tenemos que expandir este desarrollo a más dimensiones. Tomamos \[ g(t) \equiv F(t(\ga + \gor{h}) + (1-t)\ga) \] reduciendo así el cálculo a dimensión 1. Operamos ahora para calcular las derivadas:

\begin{gather*}
g'(t) = \pesc{\nabla F(a+th),h} = \sum_{i=1}^N \deriv{F}{x_i}(a+th)\cdot h_i \\
g''(t) = \sum_{i=1}^N\left(\sum_{j=1}^N \deriv{}{x_j}\deriv{F}{x_i}(\ga+\gor{h})\cdot{h_j}\right)h_i = \sum_{i,j = 1}^N \deriv{^2F}{x_i \partial x_j}(\ga+t\gor{h})h_ih_j \\
\dotsb \\
\frac{g^{s)} (0)}{s!} = \frac{1}{s!}\sum_{i_1,i_2,...,i_s=1}^N \frac{\partial^s F}{\partial x_{i_1},x_{i_2},...,x_{i_s}}
\end{gather*}

De esta forma, el desarrollo de Taylor de orden $k$ de $F$ en $\ga$ en general es

\begin{equation}
T^k_F(x) = \sum_{\alpha = 0}^k
	\left(
		\frac{1}{\alpha !}
		\sum_{i_1,\dotsc,i_\alpha = 0}^N
			(x_{i_1} - a_{i_1}) \dotsb (x_{i_\alpha} - a_{i_\alpha})
			\frac{\partial^\alpha F}{\partial x_{i_1} \dotsb \partial x_{i_\alpha}}
			 (\ga)
	\right)
\end{equation}

Por ejemplo, el desarrollo de Taylor de una función $F(x,y)$ con $\ga = (a,b)$ queda lo siguiente (con $F_{xyz\dotsc} = \dfrac{\partial^nF}{\partial x \partial y \partial z \dotsb}$)

\begin{align*}
T^k_{F}(\gx) &= F(\ga) \\
& +  (x - a) F_x(\ga) + (y - b) F_y(\ga)  \\
& +\frac{1}{2!}\left[(x-a)^2F_{xx}(\ga) + 2(x-a)(y-b)F_{xy}(\ga) + (y-b)^2F_{yy}(\ga)\right] \\
& +\frac{1}{3!}\left[(x-a)^3F_{xxx}(\ga) + 3(x-a)^2(y-b)F_{xxy}(\ga) + 3(x-a)(y-b)^2 F_{xyy} (\ga) + (y-b)^3F_{yyy} (\ga)\right] \\
& +\dotsb
\end{align*}

Existe una forma más compacta para el desarrollo de Taylor de orden dos usando el producto escalar, el vector gradiente y la matriz hessiana ($D^2F$) de derivadas segundas:

\[ F(\gor{a}+\gor{h}) = F(\ga) + \pesc{\grad F(\ga),\gor{h}} + \frac{1}{2} \gor{h}^T D^2F(\ga)\gor{h} \]

\begin{theorem}[Teorema\IS de Taylor]
 $$\frac{|F(\ga)+\gor{h} - P_{s,a}(\gor{h})|}{\norm{\gor{h}}^s} \rightarrow 0, \text{ Cuando } \gor{h} \rightarrow 0$$
 Además $P_{s,a}(\gor{h})$ es el único polinomio de orden S que hace que el límite sea 0.
\end{theorem}

--------------------------

\chapter{Teoremas de la función inversa y sus variantes}

\section{Teorema de la aplicación contractiva}

En el mundo lineal tenemos podemos resolver sistemas de dos formas. Con $\appl{F}{\real^N}{\real^N}$ y $L(\gx) = A\gx$, siendo $A$ una matriz $N\x N$; queremos resolver el sistema $A\gx = \gy$ sabiendo que $A\gor{0} = \gor{0}$.

Este sistema tiene solución si y sólo si  $\det(A) \neq 0$: es la condición para que exista $A^{-1}$.

Existe también la posibilidad de tener una función $\appl{F}{\real^{N+M}}{\real^N}$ con $L(\gx) = A\gx$, $A$ matriz $N\x (N+M)$.

Para resolver el sistema $A\gx = \gy$ parametrizamos $M$ variables.

En el mundo \textbf{no lineal}, consideramos una función $\appl{F}{\real^N}{\real^N}$. Entonces tenemos un sistema de ecuaciones

\[ \left.\begin{matrix}
F(x_1,\dotsc,x_N) = y_1\\
F(x_1,\dotsc,x_N) = y_2\\
\vdots\\
F(x_1,\cdots,x_N) = y_N
        \end{matrix}
\right\} F(\gx)=\gy \]

Vamos a intentar resolver este problema utilizando Taylor para aproximar al orden lineal, pero tenemos que pagar un precio: para que taylor funcione tenemos que trabajar cerca del punto. Esto significa que \textbf{el resultado va a ser local}.


\begin{theorem}[Teorema\IS de la aplicación contractiva] Sea
\begin{itemize}
\item $\appl{F}{\real^N}{\real^N}$ o
\item $\appl{F}{C}{C}, C\in \real^N$, cerrado, o
\item $\appl{F}{K}{K}, K\in \real^N$, compacto.
\end{itemize}

Supongamos que existe $\alpha\in(0,1)$ tal que

\[ \md{F(x)-F(y)}\leq \alpha\md{x-y} \forall x,y \in \left\{\begin{matrix}
                                                           \real^N\\
                                                           C\\
                                                           K
                                                          \end{matrix}\right.
                                              \]

  Entonces

\[  \exists ! x_0 \in\left\{\begin{matrix}         \real^N\\
                                                           C\\
                                                           K
                                                          \end{matrix}\right.
                                                        \tlq F(x_0) = x_0 \text{ (Punto fijo)} \]
\label{thmAC}
\end{theorem}


\begin{proof} Primero llevamos los casos de $C$ y $\real^n$ a un conjunto compacto $K$. Partimos de

\begin{equation}
\md{F(\gx) - F(\ga)} \leq \alpha\md{\gx-\ga} \label{eqAC_hip}
\end{equation}

y veamos qué ocurre para un vector general $\gx$: \[ \md{F(\gx)} = \md{(F(\gx)-F(\ga)+F(\ga)} \leq \md{F(\gx)-F(\ga)} + \md{F(\ga)} \]

Aplicando (\ref{eqAC_hip}) tenemos que
\[\md{F(\gx)} ≤ \alpha \md{\gx-\ga} + \md{F(\ga)} \]

  Si tomamos $\ga=0$ (en el caso  $0 \notin C $ solo haría falta una pequeña traslación), y suponemos $ \md{x} < R$, tenemos entonces que \[ \md{F(\gx)} \leq \alpha R + \md{F(\gor{0})} < R\]
  Es decir, $F$ toma un compacto y lo lleva en sí mismo: $\appl{F}{B_R(0)}{B_R(0)}$. Podemos seguir la demostración ahora suponiendo que estamos trabajando siempre sobre un compacto.

  El siguiente paso es llevar a cabo un \textbf{proceso iterativo}. Tenemos \[ \appl{F}{K}{K} \] con  $K\subset \real^N$ conjunto compacto. Definimos entonces la sucesión de $\{x_n\}_{n \in \nat} \subset K$, construido de forma iterativa con $x_n = F(x_{n-1})$. Vamos a demostrar que esa sucesión es de Cauchy, lo que implicaría que es convergente.

 Para ello, dado $\epsilon > 0$ hay que hallar $n_0$ tal que si $n,m>n_0$ entonces $\md{x_n-x_m}<\epsilon$. Pongamos, para facilitar la demostración, que $n>m$.

 Entonces, sumamos y restamos a ese módulo cada uno de los $x_i$ entre $n$ y $m$:

 \begin{equation}
  \md{x_n - x_m} = \md{x_n \pm x_{n-1} \pm \dotsb \pm x_{m+1} - x_m} \leq \sum_{i=m}^n \md{x_i - x_{i-1}} \label{eqAC_sum}
 \end{equation}

Operamos ahora con cada uno de esos sumandos. Por ejemplo, con $i = n$, vemos que

\begin{gather*}
\md{x_n - x_{n-1}} = \md{F(x_{n-1}) - F(x_{n-2})} \leq \alpha \md{x_{n-1} - x_{n-2}} = \\
= \alpha \md{F(x_{n-2}) - F(x_{n-3})} ≤ \alpha ^2 \md{x_{n-2}-x_{n-3}}
\end{gather*}

Si seguimos operando, llegaremos a que $ \md{x_n - x_{n-1}} \leq \alpha^{n-2} \md{x_2-x_1}$. Generalizando, tenemos que

\[ \md{x_i - x_{i-1}} ≤ \alpha^{i-2} \md{x_2-x_1} \]

Aplicando esta fórmula en (\ref{eqAC_sum})

\[ \md{x_n-x_m} \leq \left(\alpha^{n-2} + \alpha^{n-3} + \dots + \alpha^{m-1}\right) \md{x_2 - x_1}\]

Esa suma de $\alpha$'s es la suma de una sucesión geométrica de razón $\alpha$. Por lo tanto, la podemos simplificar como \[\sum_{k=m-1}^{n-2} \alpha^k = \alpha^{m-1}\frac{1-\alpha^{n-m}}{1-\alpha} ≤ \frac{\alpha^{m-1}}{1-\alpha} \], y la ecuación nos queda de la forma \[ \frac{\alpha^{m-1}}{1-\alpha}  \md{x_2-x_1} \]. Dado que $\dfrac{\alpha^{m-1}}{1-\alpha}  \convs[][n_0] 0$, tendremos que tomando un $n_0$ suficientemente grande se cumple que

\[ \frac{\alpha^{m-1}}{1-\alpha}  \md{x_2-x_1} < \varepsilon \]

para un $\epsilon$ arbitrariamente pequeño. Con esto \textbf{demostramos que la sucesión de $x_n$ es de Cauchy} y por lo tanto es convergente a un cierto límite $x_0$.

Tal y como habíamos construido la sucesión, tenemos que

\begin{equation} \label{eqAC_suc}x_n= F(x_{n-1}) \end{equation}

$x_n$ converge a $x_0$ cuando $n\to\infty$. De la misma forma, como $x_{n-1}$ también converge a $x_0$, está claro que $F(x_{n-1})$ convergerá a $F(x_0)$. Sustituyendo estos dos resultados en (\ref{eqAC_suc}), tenemos que

\[ x_0 = F(x_0) \]

Hemos demostrado por lo tanto que el límite de esa sucesión que hemos construido \textbf{es un punto fijo} de la función.

Nos queda \textbf{demostrar ahora que ese punto es único}, y lo haremos por reducción al absurdo:

 Supongamos que existen dos puntos fijos:

 \begin{gather*}
 a = F(a)\\
 b= F(b)
\end{gather*}

 Entonces tendríamos que \[ \md{a-b} = \md{F(a)-F(b)}\leq \alpha \md{a-b} \] pero como $\alpha$ es menor estricto que 1, entonces tendríamos que \[ \md{a-b} < \md{a-b} \], lo que es una contradicción.
\end{proof}

El teorema de la aplicación contractiva nos sirve, por ejemplo, para comprobar si hay una solución de una ecuación diferencial ordinaria (EDO).

$$\left.\begin{matrix}y'(x) = f(x,y(x))\\
        y(x_0) = y_0
       \end{matrix}\right\} \leftrightarrow y(x) = y_0 + \int_{x_0}^x f(s,y(s)) ds$$

Podemos definir:

\begin{align*}
y_1(x) &= y_0 + \int_{x_0}^{x} f(s,y_0)ds\\
y_2(x) &= y_0 + \int_{x_0}^x f(s,y_1(s))ds \equiv T(y_1)\\
&\dots\\
y_n &= T(y_{n-1}) =  y_0 + \int_{x_0}^x f(s,y_{n-1}(s))ds\\
¿T(y) &= y?
\end{align*}
Aquí es donde entraría la diferencia entre trabajar en $\real^N$ y un espacio de funciones.

Ejercicio propuesto: Aplicar este argumento a iterativo

$\left. \begin{matrix} y' = y\\
         y(0) = 1 \equiv y_0
        \end{matrix}\right\}$


\section{Teorema de la función inversa}
En Cálculo I teníamos el siguiente teorema:
\begin{theorem} Sea $\appl{f}{\real}{\real}\; f\in C^1$ y $f'(a) \neq 0$. Entonces $f$ es invertible en un entorno de $f(a)$.

La inversa es diferenciable en ese entorno, y además $(f^{-1})'(f(a)) = \frac{1}{f'(a)}$
\end{theorem}

El teorema nos daba un resultado \textbf{local} que asegura que existe la inversa, que es diferenciable y además nos daba su fórmula.

Buscamos ahora lo que ocurre en dimensión $N$. Tomamos $\appl{f}{\real^N}{\real^N}$ y supongamos que en algún abierto $\exists F^{-1}$ y $F,F^{-1} \in  C^1$.

Entonces está claro que

\[ (F\circ \F)(y) = y \implies DF(\F(y))D\F(y) = Id \]
\[ (\F\circ F)(y) = y \implies D\F(F(y))DF(y) = Id \]

Con $\appl{F}{\Omega\subset \real^N}{\real^N}$ queremos probar que existe una aplicación $\appl{G}{V}{U}$ que verifique las siguientes condiciones

\begin{gather*}
G\circ F(\gx) = \gx, \forall\gx\in U \subset \Omega \\
F\circ G(\gy) = \gy, \forall \gy \in V \\
G \text{ diferenciable}
\end{gather*}

\begin{theorem} [Teorema\IS de la función inversa]
\label{thmInv}
Sea $\appl{F}{\Omega\subset\real^N}{\real^N} \text{ con } F\in C^1(\Omega)$.

Supongamos $DF(\ga)$ invertible, $\ga \in \Omega$.

Entonces existe un abierto $V \tlq F(\ga)\in V$, un abierto $U \tlq \ga \in U$ y una inversa local $\appl{G}{V}{U}$.\\
Además, $G$ es diferenciable en $U$ y $DG(y) = \left[DF(\F(y))\right]^{-1}, \forall y \in U$.
\end{theorem}

\begin{proof} Haremos la demostración en varios pasos.

 \paragraph{1: Simplificar la notación}  Queremos invertir $F(x) = y, \gor{y} \sim F(\ga), \gx \sim \gor{a}$.

 Llamamos:
 \begin{itemize}
  \item $y = F(\ga) + \gor{z}; \gor{z} \sim \gor{0}$
  \item $y = \ga + \gor{s}; \gor{s} \sim \gor{0}$
\item  $F(\ga+\gor{s}) = F(\ga)+\gor{z}$.
  \end{itemize}
 Definimos además \[ \tilde{F}(\gor{s}) \equiv F(\ga + \gor{s}) - F(\ga) = \gor{z} \] de tal forma que  \[ \tilde{F}(\gor{0}) = \gor{0} \]

 Es decir, hacemos una traslación para suponer que $F(\gor{0}) = \gor{0}$.

 Por las hipótesis del teorema, sabemos que $\det DF(\gor{0}) \neq 0$

 Es claro que resolver para $F$ es exactamente lo mismo que resolver para $CF(\gx) = \gor{y}$, donde C es una matriz invertible.

 Tomamos $\tilde{F} = [DF(\gor{0})]^{-1}F$, de tal forma que ganamos la siguiente igualdad

 \[ D\tilde{F}(\gor{0}) = Id \]

 \paragraph{2: Formulación como punto fijo.}

 Partimos de $F(\gor{0})=\gor{0}$ y $ DF(\gor{0}) = Id$.

 Definimos $f(\gx) = \gx - F(\gx)+\gy$

 Entonces resolver $F(\gx) = \gor{y}$ es lo mismo que encontrar un punto fijo $f(\gx) = \gx$. Por lo tanto, ahora nuestro objetivo es probar que $f$ es contractiva para así poder aplicar el teorema de la aplicación contractiva (\ref{thmAC}).

 \paragraph{3: Estimar $f$} Empezamos con

 \[ Df(\gx) = Id - DF(\gx) \rightarrow Df(\gor{0}) = Id - DF(0) = Id - Id = \begin{pmatrix}  \bigzero \end{pmatrix}  \]

 La primera estimación que podemos hacer es sobre el determinante. Si $DF(\gor{0}) = Id$, entonces $\det(DF(\gor{0})) = 1$. Como $F$ es continua, entonces

 \[ \exists \varepsilon_0 >0 \tlq \md{\gx} \leq \varepsilon_0 \implies  \det(DF(\gor{0}))>0 \]

  Es decir, en un entorno del $\gor{0}$, el determinante sigue siendo positivo.


 Ahora estimamos información sobre el diferencial de $f$. Como $F\in C^1$, entonces también se cumple que $f \in C^1$. Como $\appl{f}{\real^N}{\real^N}$, entonces

  \[ Df(\gor{0}) = \begin{pmatrix}
                  Df_1(\gor{0}) \rightarrow\\
                  \vdots\\
                  Df_N(\gor{0}) \rightarrow
                 \end{pmatrix} = \begin{pmatrix}  \bigzero \end{pmatrix} \]

 Por tanto $\md{Df_i(\gor{0})} = 0$.

 Por continuidad $\exists \varepsilon_i > 0 \tlq \md{x} \leq \varepsilon_i, \implies \md{Df_i(\gx)} <\frac{1}{2N}$. Fijamos un $\varepsilon = \min \{\varepsilon_0,\varepsilon_1,\dotsc, \varepsilon_N\} ,\, i=0,\dotsc,N$.

 Entonces, si $\md{x} \leq \varepsilon$ tenemos  que
\begin{gather}
\det(DF(\gx))>0 \label{eqFinv_DetF} \\
\md{Df_i(\gx)}  = \md{\nabla f_i(\gx)} < \dfrac{1}{2N}, i=1,2,...,N \label{eqFinv_Detfi}
\end{gather}

 \begin{remark} $\varepsilon$ NO depende de $\gy$. \end{remark}


  Tomaremos así $\gx\in \gor{B_\varepsilon(\gor{0})}$, donde $\gor{A}$ es el cierre de $A$ (\ref{dfnCierre}).

  \paragraph{4: Demostrar que $f$ lleva un cerrado en sí mismo}

Es decir, hay que demostrar que \[ \appl{f}{ \gor{B_\varepsilon(\gor{0})}}{ \gor{B_\varepsilon(\gor{0})}} \].

  Teniendo $\md{\gor{s}}\leq \varepsilon$ queremos probar $\md{f(\gor{s})}\leq \varepsilon$. Operamos:

  \begin{equation}
  f(\gor{s}) = \md{f(\gor{s}) - f(0) + f(0)} \leq \md{f(\gor{s})-f(0)} + \underbrace{\md{f(0)}}_{f(0) = \gor{0} + F(\gor{0}) + \gor{y} = y}
  \label{eqFinv_Des1}
  \end{equation}
Por otra parte

  \[ \md{f(s)-f(0)}^2 = \sum_{i=1}^N (f_i(\gor{s})-f_i(0))^2 \]

  Aplicando el teorema del valor medio (\ref{thmTVM}) con un punto $0<\tilde{s}<s$, tenemos que

  \[ f_i(s) - f_i(0) = Df_i(\tilde{s}) \cdot (\gor{s} - \gor{0}) \]

  Entonces

 \[ \sum_{i=1}^N (f_i(\gor{s})-f_i(0))^2 =\sum_{i=1}^N \left(Df_i(\tilde{s})\cdot\gor{s}\right)^2 =
 	\sum_{i=1}^N(\pesc{\nabla f_i(\tilde{s}),\gor{s}})^2
 	\leq \sum_{i=1}^N \md{\nabla f_i(\tilde{s})}^2\md{\gor{s}}^2 \]

 	y usando (\ref{eqFinv_Detfi}) nos queda que

 	\[ \sum_{i=1}^N (f_i(\gor{s})-f_i(0))^2 ≤ N \frac{1}{4N^2} \md{\gor{s}} \]
  y por lo tanto
  \[ \md{f(\gor{s}) - f(\gor{0})}^2 \leq \frac{1}{4N} \md{\gor{s}}^2 \]

  Usando este resultado recuperamos (\ref{eqFinv_Des1})
 \begin{align*}
  \md{f(s)} &\leq \frac{1}{2\sqrt{N}} \md{\gor{s}} + \md{\gy} \\
  &\leq \frac{1}{2\sqrt{N}}\varepsilon + \md{\gy} \\
  & \leq \frac{\varepsilon}{2} + \md{y} \\
  &< \varepsilon \dimplies \md{y} < \frac{\varepsilon}{2}
  \end{align*}

y por lo tanto hemos demostrado que $f$ lleva un cerrado en sí mismo.

  Esta última acotación (forzar que $\md{y}< \frac{\epsilon}{2}$) es por la que es un teorema local.

  \paragraph{5: $f$ es contractiva en $B_\varepsilon(\gor{0})$}

  Tomamos $\gor{r},\gor{s} \in B_\varepsilon(\gor{0})$

  $$\md{f(\gor{r}) - f(\gor{s})} = \left(\sum \left( f_i(\gor{r}) - f_i(\gor{s})\right) ^2 \right)^{\frac{1}{2}}$$
  Aplicando el teorema del valor medio
  $$\left(\sum_{i=1}^N \pesc{Df_i(z_i), (\gor{r}-\gor{s})^2}\right)^{\frac{1}{2}}, z_i\in B_\varepsilon(0) $$
  La misma cuenta de antes:
  $$\md{f(\gor{r}) - f(\gor{s})} \leq \frac{1}{2\sqrt{N}}\md{\gor{r}-\gor{s}}$$

  Acabamos de encontrar el $\alpha \in (0, 1)$ que aparecía en el teorema de la aplicación contractiva: \[ \alpha = \frac{1}{2\sqrt{N}} \]

  Ahora ya podemos aplicar el teorema de la aplicación contractiva y ya tenemos el punto fijo. Por lo tanto, existen dos vectores $\gx, \gy$ tal que $F(\gx) = \gy$ y por lo tanto existirá también una aplicación $G$ con $x= G(y)$. Vamos a demostrar que

  \[ \appl{G}{B_{\frac{\varepsilon}{2}}(0)}{\overline{{B_{\frac{\varepsilon}{2}}(0)}}} \]

  Sea $y \in B_{\frac{\varepsilon}{2}}$. Entonces

\[ \md{G(y)} = \md{\gx} = \md{f(\gx)} = \md{f(\gx) \pm f(\gor{0})} \leq \md{f(\gx) - f(\gor{0})} + \md{f(\gor{0})} \]

Como $f$ es contractiva

\[ \md{f(\gx) - f(\gor{0})} + \md{f(\gor{0})} \leq \frac{1}{2\sqrt{N}} \md{\gx} + \md{\gy} \]

y por lo tanto
\[ \md{G(y)} \leq \frac{1}{2\sqrt{N}}\varepsilon + \frac{\varepsilon}{2} < \varepsilon \]

  Si $\md{G(y)} < \varepsilon$ entonces  $G(y)\in B_{\varepsilon} \implies \appl{G}{B_\varepsilon}{B_\varepsilon}$.

  Por lo tanto, podemos concluir que $G(y) = x \dimplies F(x) = y$ con $y\in B_{\frac{\varepsilon}{2}}(\gor{0})\;, x \in B_{\varepsilon}(\gor{0})$

  \paragraph{6: Continuidad de $G$}


  Vamos a ver que pasa con diferencias del tipo $\md{s -G(s)}$. Sea $G(s) = t$ y $s = F(t)$.
  \begin{gather*}
  f(t) = t - F(t) + y\\
  s - G(s) = -G(s) + F(G(s)) = F(t)-t = y-f(t) = y - f(G(s))
  \end{gather*}

Consideramos ahora \[ \md{G(u)-G(v)} = \md{G(u)-G(v) -u +u-v+v} \leq \md{u-v} + \md{G(u)-u + v-G(v)} \]

Aplicando el resultado anterior

  \begin{gather*}
\md{u-v} + f(G(u)) - y - [y -f(G(v))] =\\
= \md{u-v} + \md{f(G(u)) - f(G(v))} \leq \\
\leq \frac{1}{2\sqrt{N}} \md{G(u)-G(v)} \leq \frac{1}{2}  \md{G(u)-G(v)}\\
\md{G(u)-G(v)}\leq \md{u-v} + \frac{1}{2}\md{G(u)-G(v)}\\
\md{G(u)-G(v)} \leq 2 \md{u-v}
  \end{gather*}

  Por lo tanto $G$ es una función continua uniforme.

  \begin{remark}
  En este caso tenemos $\md{G(u)-G(v)} < C\md{u-v} \leftarrow $ \textbf{Espacio de funciones Lipschitz}

  Si en cambio $\md{G(u)-G(v)} < C\md{u-v}^\alpha \leftarrow $ \textbf{Espacio de funciones Hölder} ($\alpha<1$).
  \end{remark}

  \paragraph{Paso 7: G diferenciable}  Sea $\gy \in B_{\frac{\varepsilon}{2}}(0)$

  Aplicamos la definición de diferenciabilidad

  \[ \lim_{h \rightarrow \gor{0}}\frac{\md{G(y+h) - G(y) \left[DF(G(y))\right]^{-1} \gor{h}}}{\md{\gor{h}}} = 0 \]

  Vamos a intentar trabajar con las $\gx's$ que es donde sabemos todo y no con $\gy's$ que no tenemos ni idea de nada.

  \emph{Notación:}
  \begin{align*}
G(\gy) &= \gx & \gor{y} &= F(\gx)\\
G(\gy + \gor{h}) &- G(\gy) = \xi & \gy + \gor{h} &= G(\gx + \gor{\xi})\\
&\downarrow&\ &\downarrow\\
G(\gy + \gor{h}&) = \gx + \xi & \gor{h} &= F(\gx + \gor{\xi}) - F(\gx)
\end{align*}
$$\gor{h} \rightarrow 0 \dimplies \gor{\xi} \rightarrow \gor{0}$$
  Sustituimos con esta notación en la definición:


  $$\lim_{h \rightarrow \gor{0}}\frac{\md{G(y+h) - G(y) \left[DF(G(y))\right]^{-1} \gor{h}}}{\md{\gor{h}}} = \\$$
  $$...\\$$
  $$\lim_{\xi\rightarrow \gor{0}} \underbrace{\frac{\md{\xi}}{\md{F(\gx + \gor{\xi} - F(\gx)}}}_{A} %&
  \cdot \underbrace{\frac{\gor{\xi} - \left[DF(G(y))\right]^{-1} (F(\gx +\gor{\xi}) - F(\gx)}{\md{\gor{\xi}}}}_{B}\\   $$

  Vamos a acotar B aplicando:
  $$\xi = \underbrace{\left[DF(G(y))\right]^{-1}DF(x)}_{=Id} \cdot \xi$$

  $$B = \frac{\md{\left[DF(G(y))\right]^{-1} \left[ -\{F(x+\xi)-F(x) - DF(x)\xi\}\right]}}{\md{\xi}}$$

  $$B\leq C \frac{\md{F(x+\xi) - F(x) - DF(x)\xi}}{\md{\xi}} \convs[\text{F dif.}][\xi][0] C\cdot 0 \rightarrow 0$$

  Donde $C$ es la norma de la matriz.


  Ahora vamos a probar que $A$ está acotado, probando que $A>0$, lo que acota el inverso:

  $$\frac{1}{A} = \frac{\md{F(x+\xi)-F(x)}}{\md{\xi}} = \frac{\md{F(x+\xi) - F(x) - DF(x)\xi + DF(x)\xi}}{\md{\xi}}$$
  $$\geq \frac{\md{DF(x)\xi}}{\md{\xi}} - \underbrace{\frac{\md{F(x+\xi) - F(x) - DF(x)\xi}}{\md{\xi}}}_{\rightarrow 0}$$


  $$\md{\frac{DF(\gx)\xi}{\md{\xi}}} = \md{DF(\gx)\times\gor{v}}, \md{\gor{v}} = 1$$
  $$\text{Definimos } M(\gor{v}) = \md{DF(\gx)\times\gor{v}}, \text{ para } \gor{v} \in S^1$$

  $S^1$ es la esfera de radio 1, un conjunto compacto.


  Aplicamos: $M$ continua, definida en un conjunto compacto $\implies$ $M$ alcanza su máximo y su mínimo (\ref{thmCompactoMax}). En concreto, si su mínimo es $\delta$ tenemos:

  $$ M(v)\geq \delta > 0 \implies \frac{1}{A}\geq \delta > 0 \implies A\leq C $$


  $$\left.\begin{matrix}A \leq C\\B \rightarrow \gor{0}\end{matrix}\right\} \implies \lim_{h \rightarrow \gor{0}}\frac{\md{G(y+h) - G(y) \left[DF(G(y))\right]^{-1} \gor{h}}}{\md{\gor{h}}} = 0$$

  y por lo tanto $G$ es diferenciable, y la expresión de su diferencial es \[ DG(y) = \left[DF(\F(y))\right]^{-1} \]
\end{proof}

\paragraph{Ejemplo del teorema de la función inversa.}
Sea $F(x,y) = (x^2-5y^2,4xy)$.

Tomamos $(x_0,y_0)$.

¿$F$ invertible en un entorno de $F(x_0,y_0)$?

Calculamos Df:

$$Df = \begin{pmatrix}
        2x&-10y\\
        4y & 4x
       \end{pmatrix}$$

$$\det(DF) = 8x^2 + 40y^2 \neq 0 \text{ si } (x,y) \neq (0,0)$$

Cuando el determinante sea 0, significa que no puedo aplicar el teorema, por tanto, no sé si la función es invertible o no. Aplicamos los fundamentos. ¿Es inyectiva la función?

No es inyectiva en ningún entorno del (0,0).

El hecho de que el teorema sea local nos puede llevar a confusiones. Por ejemplo, sea \[ F (r,\sigma) = (rcos(\sigma),r\sen(\sigma)), r \in [0,1], \sigma \in [0,4\pi]\]

Entonces hay dos soluciones para la inversa:

\[ F^{-1} (0,\frac{1}{2}) = \left\{\begin{matrix}2\pi+\frac{\pi}{2}\\\frac{pi}{2}\end{matrix}\right. \]

Lo que hay que hacer es partir de un punto del conjunto de salida. El teorema dice que escogido un punto del conjunto de salida, existe un entorno en el conjunto de llegada en el que se puede definir la función inversa. \textbf{Hay que acotar también el conjunto de llegada.}

Otro ejemplo es considerar  $g(x) = f(x) + \varepsilon x$ siendo $f(s) =\left\{\begin{matrix}x^2sin\left(\frac{1}{x}\right)& \text{ si } x\neq0\\0 &\text{si } x=0\end{matrix}\right.$
Esta función $g \notin C^1$. $g$ es derivable ($g'(0) = \varepsilon>0$) pero la derivada no es continua. Se deja como ejercicio para el lector la comprobación.

\section{Teorema de la función implícita}

Tomemos el caso particular de una superficie en $\real^3$. Puede venir dada de dos formas:
\begin{itemize}
 \item Conjunto de nivel: $F(x,y,z) = 0$
 \item Gráfica: $z=f(x,y) \rightarrow F(x,y,z) = f(x,y)-z$
\end{itemize}

¿Existe alguna forma de expresar $F(x,y,z)$ de la forma $z=f(x,y)$? Pensando en el ejemplo de la esfera: $F(x,y,z) = x^2+y^2+z^2+1$, se puede expresar de dos formas:

\[ z = \pm \sqrt{1 - x^2 - y^2} \]

¿Cuál es la condición que necesitamos para poder despejar $z$? Supongamos que sabemos despejar $z=f(x,y)$, entonces tenemos: $F(x,y,f(x,y)) = 0$. Derivando implíctamente

\[ \underbrace{\frac{\partial}{\partial x} [F(x,y,f(x,y)]}_{\dpa{F}{x} + \dpa{F}{z}\cdot\dpa{f}{x}}= \underbrace{\frac{\partial}{\partial y} [F(x,y,f(x,y)]}_{\dpa{F}{y} + \dpa{F}{z}\cdot\dpa{f}{y}} = 0 \]

Si $f$ es diferenciable tenemos:
$$\dpa{f}{x}(x,y) = - \frac{\dpa{F}{x}(x,y,f(x,y))}{\dpa{F}{z}(x,y,f(x,y))}$$
$$\dpa{f}{y}(x,y) = - \frac{\dpa{F}{y}(x,y,f(x,y))}{\dpa{F}{z}(x,y,f(x,y))}$$
Necesitamos entonces que $\displaystyle\dpa{F}{z}\left(x,y,f(x,y)\right) \neq 0$. Veamos cómo extrapolar esto de forma general con tres variables.

\begin{theorem}[Teorema\IS de la función implícita (en $\real^3$)]

\label{TFImp}

Sea $\appl{F}{\Omega\subset\real^3}{\real}, F\in C^1$, con

\[ F(a,b,c) = 0 \] y \[ \dpa{F}{z}(a,b,c)\neq 0 \]

Entonces existe una función $\appl{f}{\omega}{\real}$ con $(a,b)\in \omega \implies  f(a,b) = c$ de tal forma que

$F(x,y,f(x,y)) = 0, \forall(x,y)\in \omega$

\end{theorem}

\begin{proof} Vamos a realizar el siguiente proceso:

Definimos $H(x,y,z) = (x,y,F(x,y,z))$. Esta función aplana la superficie del conjunto de nivel, porque $(x,y,z) \in S \implies F(x,y,z)=0 \implies H(x,y,z) = (x,y,0)$

Esta función nos aplana la superficie del conjunto de nivel, pero lo que estamos buscando es desde un espacio bidimensional (conjunto de partida de $f$) llegar a la superficie de nivel, que es una superficie de $\real^3$, el espacio de partida de $F$. Entonces vamos a buscar $H^{-1}$.

El problema de esta función es que $\appl{H}{\real^3}{\real^3}$, pero toda la información que necesitamos es la tercera componente de $H^{-1}$.

Según el teorema de la función inversa, existen abiertos $U, V$ con $(a,b,c) \in U$ y  $V\in (a,b,0)$; y una única inversa local

\[ \appl{\inv{H}}{V}{U} \]

De tal forma que

\[ \inv{H}(u,v,w) = (x,y,z) \dimplies (u,v,w) = H(x,y,z) = (x,y,F(x,y,z)) \]

Es decir \[ \inv{H} (u,v,w) = (u,v,g(u,v,w)) \]

donde $g$ es la función única que depende de $(u,v,	w)$, y no es más que la tercera componente de la inversa que hemos construido. Demostremos que existe:
 \begin{gather*}
 H\circ H^{-1} = Id \\
 H(H^{-1}(u,v,w)) = H(u,v,g(u,v,w)) = (u,v,w)
 \end{gather*}

 En particular si $w=0$:
 $$(u,v,0) = H(u,v,g(u,v,0)) = (u,v,F(u,v,(g(u,v,0)))$$
 Conclusión: Hemos encontrado una única $g$, tal que $F(u,v,g(u,v,0)) = 0$.

  Notación: $g(u,v,0) = f(u,v)$

  $F(u,v,f(u,v)) = 0, (u,v) \in \text{Proyección sobre el plano horizontal de la superficie}$

\end{proof}

\begin{theorem}[Teorema\IS de la función implícita (caso general)]\label{thmFImp}

Dadas $n$ ecuaciones, $n+m$ incógnitas, consideramos

$$\appl{F}{\Omega\subset\underbrace{\real^M}_{x} \times \underbrace{\real^N}_{y}}{\real^N}$$

Con la notación $F = (F_1,...,F_N)$

Los elementos de $\real^M\times\real^N$ los llamamos $(x_1,x_2,...,x_m,y_1,y_2,...,y_n) = (\gor{x},\gy)$.

Supongamos $F\in C^1$. Sea $\ga \in \real^M, \gor{b} \in \real^N \tlq (\gor{a},\gor{b})\in \Omega , F(\gor{a},\gor{b})=0$

Supongamos $D_yF(\ga,\gb)$ no singular, es decir $\det(D_yF(\ga,\gb))\neq 0$, siendo:
$$D_yF = \begin{pmatrix}
          \dpa{F_1}{y_1}&...&\dpa{F_n}{y_n}\\
          \vdots&\ddots&\vdots\\
          \dpa{F_n}{y_1}&\cdots&\dpa{F_n}{y_n}
         \end{pmatrix}$$

\paragraph{Entonces:} Existen abiertos $\omega \subset \real^M, \Theta \in\real^N$, con $\ga \in \omega, \gb \in \Theta$ y una única función: \[ \appl{g}{\omega\subset\real^M}{\Theta \subset\real^N}, g\in C^1(\omega) \]

Tal que:
\begin{itemize}
 \item $g(\ga) = \gb$
 \item $F(\gx,g(\gx)) = \gor{0}, \forall \gx \in \omega$
 \item $\displaystyle Dg(\gx) = - \left[D_yF(\gx,g(\gx))\right]^{-1} \cdot D_xF(\gx,g(\gx))$
\end{itemize}
\end{theorem}

\begin{proof}

 Definimos: $H(\gx,\gy) = (\gx,F(\gx,\gy))$. Esta función $\appl{H}{\real^{m+n}}{\real^{n+m}}, H\in C^1$. Además $H(\ga,\gb) = (\ga,F(\ga,\gb)) = (\ga,\gor{0})$

 $$DH_{(a,b)} = \left(
                 %\underbrace{1&0&0&...&0}_{m}&\underbrace{0&...&0}_{n}\\
                 %\underbrace{0&1&0&...&0}_{}&\underbrace{0&...&0}_{}\\
                 \begin{array}{c|c}
                 I_{m\times m} &  0_{m\times n}\\
                 \hline
                 D_x F_{n\times m} &  D_y F_{n\times n}
                 \end{array}
                 \right)$$

$\det(DH(\ga,\gb)) = \det(D_y(\ga,\gb)) \neq 0$. Aplicando el teorema de la función inversa podemos invertir $H$ en un entorno de $H(\ga,\gb)$. Además, por el teorema también sabemos la unicidad y que $H \in C^1$.

Problema: identificar $g$ dentro de $H^{-1}$.

$$\underbrace{H(\gx,\gy)}_{\equiv (u,v)} = (\gx,F(\gx,\gy))$$
$$\implies H^{-1}(u,v) = (x,y) = (u,?)$$
Notación: $H^{-1}(u,v) = (u,\tilde{g}(u,v))$

Estamos interesados en la restricción $H^{-1} (u,0) = (u,\tilde{g}(u,0))$. Podemos comprobar que $\tilde{g}(u)\in\real^N, u\in \real^m$.

Tenemos
\[H^{-1} (u,0) = (u,g(u)) \dimplies (u,0) = H(u,g(u)) = ( u,F(u,g(u)))\]


Ya tenemos los 2 primeros apartados, vamos a por la fórmula:

\[F(\gx,g(\gx)) = \gor{0}\]
\[D_x[F(\gx,g(\gx))] = (\gor{0})\]
\[D_x[F(\gx,g(\gx))] = \begin{pmatrix}
                        \dpa{F_1(\gx,g(\gx))}{x_1}&\cdots&\dpa{F_1(\gx,g(\gx))}{x_n}\\
                        \vdots&\ddots&\vdots\\
                        \dpa{F_n(\gx,g(\gx))}{x_1}&\cdots &\dpa{F_n(\gx,g(\gx))}{x_n}
                       \end{pmatrix}
\]
Donde: $$\dpa{F_1(\gx,g(\gx))}{x_1} = \dpa{F_1}{x_1} + \sum_{k=1}^{n} \dpa{F_1}{y_k}\cdot \dpa{y_k}{x_1} \sim (D_y F_1 \rightarrow) \cdot \begin{pmatrix}
\dpa{g}{x_1}\\
\vdots\\
\dpa{g}{x_n}
\end{pmatrix}$$

Aplicando esto obtenemos:

\[ 0 = D_x[F(\gx,g(\gx))] = (D_xF) + (D_yF)(Dg) = D_xF(\gx,g(\gx)) + D_yF(\gx,g(\gx))\cdot Dg(\gx)\]

Despejando obtenemos la fórmula que nos decía el teorema.


\end{proof}

\subsection{Ejemplos}
\begin{example}

$$z^3lg(xy) + 2x^2 + 2y^2 +z^2 + 8xz - z + 8 =0$$

Demostrar que la ecuación anterior define DOS funciones $z = f_1(x,y), z = f_2(x,y)$ en un entorno de $(x,y)=(1,1)$.

\paragraph{Solución: }

Esto no contradice al teorema (que tiene unicidad) porque tenemos que anclar los puntos con los que vamos a trabajar en los que $F(x,y,z) = 0$. Asíque vamso a ver $F(1,1,z) = \underbrace{z^3lg(xy)}_{0} + 2 + 2 + z^2 + 8z -z +8 = 0 \implies z^2+7z+12 = 0 \implies $ 2 soluciones.

Tenemos que ver qué pasa con $\displaystyle \dpa{F}{z}(1,1,z_i)$.

\[\dpa{F}{z} = 3z^2lg(xy) + 2z -1\]
\[\dpa{F}{z}(1,1,z_i) = 2z_i + 7 \neq 0\]

Ahora estamos en condiciones de aplicar el teorema.

También nos pide hallar el desarrollo de Taylor de orden 1 para $f_1$.

\[f_1(x,y) = f_1(1,1) + \underbrace{\dpa{f_1}{x}(1,1)(x-1) + \dpa{f_1}{y}(1,1) (y-1)}_{\pesc{\nabla f_1(1,1),(x-1,y-1)}} + err\]
¿Cómo calcular las derivadas? Recurrimos al teorema y sustituyendo $z=f_1(x,y)$
\[(f_1(x,y))^3 lg(xy) + 2x^2 + 2y^2 + (f_1(x,y))^2 + 8x(f_1(x,y))-(f_1(x,y))+8 = 0\]
Derivada con respecto a $x$:
\begin{gather*}
 0 = (f_1(x,y))^2\dpa{f_1}{x}(x,y)\cdot lg(xy) + (f_1(x,y))^3 \frac{1}{x}+4x + \\ 2(f_1(x,y))\dpa{f_1}{x}(x,y) + 8x\dpa{f_1}{x}(x,y) - \dpa{f_1}{x}(x,y) \\
 \dotsb
 \end{gather*}
Vamos a evaluar en $(1,1)$ lo que tenemos donde $f_1(x,y) = z_1$ y $f_2(x,y) = z_2$ y despejamos $\dpa{f_1}{x}$.
\end{example}

\begin{example}[Hoja 3, ejercicio 14]

Demostrar que existe una 'unica f... con $f(0,0) = 0$.
$$e^{f(x,y)} = (1+xe^{f(x,y)})(1+ye^{f(x,y)})$$
¿Podemos despejar $z = f(x,y)$?. (Es lo mismo que demostrar que existe una función $$e^{z} = (1+xe^z)(1+ye^z)$$

Definimos $F(x,y,z) = e^z - (1+xe^z)(1+ye^z) = 0$

Comprobamos que $F(0,0,0) = 1-1 = 0$.

Hipótesis del teorema: $\appl{F}{\real^3}{\real}$ con $F(0,0,0) = 0, F \in C^{\infty}$
Nos falta comprobar \[\dpa{F}{z}(0,0,0) \neq 0\]. (Este paso en el caso general es el determinante de $D_zF(0)$)

Entonces podemos aplicar el teorema
\[\implies \exists ! f \tlq F(x,y,f(x,y)) = 0\]
\end{example}

\paragraph{Ejemplo}

Estudiar si es posible despejar $u(x,y,z), v(x,y,z)$ en las ecuaciones:

\[\left\{\begin{matrix} xy^2+xzu+yv^2 &= 3\\ xyu^3+2xv-u^2v^2 &= 2\end{matrix}\right.\]
En un entorno de $(x,y,z) = (1,1,1)$

Vamos a tener que definir una
\[\appl{F}{\real^5}{\real^2}\]
\[(x,y,z,u,v) \rightarrow F(x,y,z,u,v)= (xy^2+xzu+yv^2-3,xyu^3+2xv-u^2v^2-2)\]
Podemos comprobar fácilmente que $F\in C^{\infty}$ y $F(1,1,1,1,1) = ... = (0,0)$.

Para poder despejar u,v tenemos que evaluar $D_{(u,v)}F$ en $(1,1,1,1,1)$.

\[D_{(u,v)} = \begin{pmatrix} \dpa{F_1}{u}&\dpa{F_1}{v}\\ \dpa{F_2}{u} &\dpa{F_2}{v}\end{pmatrix}
= \begin{pmatrix} xz & 2yv\\3xyu^2-2uv^2 & 2x-2u^2v \end{pmatrix} = ... = \begin{pmatrix} 1&2\\ 3&0 \end{pmatrix}\]

Tenemos $\det D_{(u,v)} = -6 \neq 0$. Entonces estamos en las hipótesis para utilizar el teorema y garantizar que en un entorno del punto $(1,1,1)$ blablabla.
COMPLETAR

Vamos a calcular (porque lo pide el enunciado) \[\dpa{u}{x},\dpa{v}{x},\dpa{v}{z}\].

Como el teorema garantiza que existe, derivamos implícitamente:

Vamos a derivar implícitamente respecto a $x$ el sistema:
\[\left\{\begin{matrix} y^2+zu+xzu_x + y 2v v_x = 0 \\ yu^3+xy3u^3u_x  + 2v + 2xv_x - 2uu_xv^2-2u^2vv_x = 0 \end{matrix}\right.\]
Donde $u_x = \dpa{u}{x}$.

\emph{Sabemos:} si $(x,y,z) = (1,1,1) \implies (u,v) = (1,1)$

Sustiuyendo:
\[\left\{\begin{matrix}1+1+u_x+2v_x &= 0 \\ 1+3u_x+2+2v_x-2u_x-2v_x &= 0\end{matrix}\right.\]
\[\left\{\begin{matrix}u_x(1,1,1) + 2v_x(1,1,1) &= -2\\ u_x(1,1,1) &= -3 \end{matrix}\right.\]

Faltaría  calcular $\dpa{v}{z}$

\paragraph{Ejercicio propuesto: Calcular $\dpa{u}{x^2}$}

\paragraph{Ejercicio} Demostrar T.F.Inversa a partir del T.F Implícita
Tenemos:
\begin{gather}
 \appl{F}{\real^N}{\real^N}\\
 F\in C^1\\
 F(\ga) = \gb\\
 \det DF(\ga) \neq 0
\end{gather}
¿Podemos despejar $F(\gx) = \gy$ para $\gx$ en un entorno de $\ga$ $\gy$ en un entorno de $\gb$?

$F(\gx) = \gy$ es lo mismo que $H(\gx,\gy) = 0$ con $H(\gx,\gy) = F(\gx)-\gy$.

$\appl{H}{\real^N\times \real^N}{\real^N}. H\in C^1$ y $H(\ga,\gb) = 0$. Tenemos el punto de partida en el que anclar el teorema. Queremos hallar $\gx$ como función de $\gy$ en la ecuación $H(\gx,\gy) = 0$.

Necesitamos para aplicar el teorema: $\det D_x H(\gx,\gb) \neq 0$.

\obs $D_x H  = D_x F \neq 0$ (por (4))

\paragraph{Conclusión:} $\exists f(\gy) \tlq H(f(\gy),\gy) = \gor{0} \equiv F(f(\gy)) - \gy = \gor{0} \equiv F(f(\gy)) = \gy$.

Ahora tenemos que ver que la composición en el otro sentido también nos da la identidad.

\[f(F(\underbrace{f(\gy)}_{v}) = f(\gy) \implies f(F(v)) = v\]

----------------------


\section{Teoremas del Rango}
\label{secRango}
¿Dónde está escondida la indentidad en un sistema de ecuaciones (lineales o no)?

\begin{theorem}[Teorema\IS del Rango (1)]
Sea \[\appl{F}{\Omega\subset \real^M\times\real^N}{\real^N}\]
\[F\in C^1, (\ga,\gb) \in \Omega \text{ con } \ga \in \real^M, \gb \in \real^N\]
Supongamos que $DF(\ga,\gb)$ tiene rango $n$ (máximo posible).

Entonces: $\exists$ un abierto $\omega$ con $(\ga,\gb) \in \omega$ y una función \[ \appl{G}{\omega\subset\real^M\times\real^N}{\real^M\times\real^N}, G\in C^1 (\omega)\] con inversa local diferenciable, tal que \[F\circ G(\gor{u},\gor{v}) = \gor{v}, \forall(\gor{u},\gor{v})\in \omega\]

\end{theorem}

\begin{proof}
 Reordenamos las variables de manera que \[DF(\ga,\gb) = \begin{array}{c|c} A &B \end{array}\]
 \[A \in M_{m\times m}, B = D_yF(\ga,\gb), \det B \neq 0\]

 Definimos \[H(\gx,\gy) = (\gx,F(\gx,\gy))\]
 Calculamos:
 \[DH = \left(\begin{array}{c|c}
         I & \\
         \underbrace{D_xF}_{m\times n} & \underbrace{D_yF}_{n\times n}
        \end{array}\right)\]


  Estudiamos el determinante: $\det DH = \det D_yF \neq 0$ debido a la reordenación de las variables que hemos hecho al principio. Además, $F\in C^1 \implies H \in C^1$. Estamos en condiciones de aplicar el teorema de la función inversa. $\exists$ una inversa LOCAL $H^{-1}$

  \[H(x,y) = (u,v) \dimplies (x,y) = H^{-1}(u,v) \equiv (\underbrace{G_1(u,v)}_{\real^M},\underbrace{G_2(u,v)}_{\real^N})\]

  \begin{gather*}
H(H^{-1}(u,v)) = (u,v)\\
H(G_1(u,v),G_2(u,v))\\
= (G_1(u,v),F(G_1(u,v),G_2(u,v)))
  \end{gather*}
 Tomando $G(u,v) = (G_1(u,v),G_2(u,v))$ obtenemos que $F\circ G(u,v) = v$, para $(u,v)$ en un entorno del punto $(\ga,\gb)$

\end{proof}

\begin{theorem}[Teorema\IS del Rango (2)] \label{TR2}
 \[\appl{F}{\real^N}{\real^N\times\real^M}\]
 \[F \in C^1, \ga \in \Omega\]

 Rango de $DF(\ga) = n$ (máximo).

 Entonces, $\exists \omega $ abierto en $\real^N\times\real^M$, con $F(\ga) \in \omega$.

 Y una función $ G\in C^1(\omega), \appl{G}{\real^M\times\real^N}{\real^M\times\real^N}$

  $G$ tiene inversa local diferenciable tal que $(G\circ F) (\underbrace{\gx}_{\real^N}) = (\underbrace{\gx}_{\real^N},\underbrace{\gor{0}}_{\real^M})$.
\end{theorem}

\begin{proof}
 \[DF(\ga) = \begin{pmatrix}
              \dpa{F_1}{x_1} &\dots &\dpa{F_1}{x_n}\\
              \vdots&\ddots&\vdots\\
              \dpa{F_n+m}{x_1} &\dots & \dpa{F_n+m}{x_n}
             \end{pmatrix}
\]
Reordemamos las $F_j$ de la siguiente manera:
\[DF(\ga) = \overbrace{\left(\begin{array}{c}
		  \det\neq 0\\
		  \hline
                  \text{Resto}
                  \end{array}\right)}^{n \text{ columnas }}\begin{array}{c} \} \text{ n filas}\\ \} \text{ m filas}\end{array}\]

Definimos:
\begin{align*}
H: \real^N\times\real^M &\longrightarrow \real^N\times\real^M\\
(\gx,\gy) &\longrightarrow \underbrace{F(\gx)}_{\real^N} + (\underbrace{\gor{0}}_{\real^N}, \underbrace{\gy}_{\real^M}) = (F(\gx),\gy)
\end{align*}

\[F(\gx) = H(\gx,\gy) = (F_1(\gx),F_2(\gx),...,F_n(\gx), F_{n+1}(\gx)+\gy_1,...,F_{n+m}(\gx)+\gy_m)\]
\[DH = \left(\overbrace{D_xF}^{\text{ N columnas}} \; \begin{array}{|c}0  \\ \hline Id \end{array}  \right) \begin{array}{c} \}\text{ n filas} \\  \}\text{ m filas} \end{array} \implies \det DH \neq 0
\]

Estamos en condiciones de aplicar el teorema de la función inversa $ \implies \exists$ una inversa local $\invers{H}$ tal que
\[\invers{H} \circ H(u,v) = (u,v), u\in \real^N,v\in\real^M\]
En particular:
\[\left. \begin{array}{c} \invers{H} \circ H (\gor{u},\gor{0}) = (\gor{u},\gor{0})\\
H(\gor{u},\gor{0}) = (F(\gor{u}) + (\gor{0}, \gor{0})) \end{array} \right\} \implies \invers{H} \circ H(\gor{u}+(\gor{0},\gor{0})) = \invers{H}(F(\gor{u})) = (\gor{u},\gor{0})\]
REVISAR: A partir del $\implies$ soy yo, no azorero.
\end{proof}

\begin{theorem}[Teorema\IS del rango (resultado general)]
\[\appl{F}{\real^N}{\real^K}, F\in C^1\]
Con rango $DF = p < \min\{n,k\}$

Existe $\Gamma (u_1(\gx),...,u_n(\gx)) = (\underbrace{u_1,...,u_p,0,...,0}_{k})$, siendo $\Gamma = \Phi \circ F \circ \invers{\Phi}$.


 Siendo $U$ un cambio de variable.
\end{theorem}

\paragraph{Ejercicio}

\[\left\{\begin{array}{cc}
   F_1\equiv x^2+z^2+2xz-2x-2z+1&=0\\
   F_2\equiv x^2+4y^2+4z^2+4xy+4xz+8xy&=0
  \end{array}\right.\]
  ¿Es depejable en función de z en un entorno de $(x,y) = (0,-1), z=1$?

Solución:

1) Ver que el punto safisface las ecuaciones.

2) Ese sistema es como definir:
\[\appl{F}{\real^3}{\real^2}, F\in C^1, F(0,-1,1) = (0,0)\]

3) Calculamos el determinante de $DF(0,-1,1)$ y vemos que da $0$.

Conclusión: no podemos aplicar el teorema, pero pensando un poco vemos que

\[F_1 = (x+z)^2 -2(x+z) + 1 = (x+z-1)^2\]
\[F_1 = 0 \dimplies x=1-z\]
\[F_2(x,y,z) = F_2(1-z,y,z) = (1-z)^2 + 4y^2 + 4z^2 + 4(1-z)y + 4(1-z)z+8yz\]
\[ =... = a(z)y^2+b(z)y+c(z) \implies y=\frac{-b\pm \sqrt{...}}{2a}\]
¿Cual de las 2 soluciones escoger? Sabemos (por el enunciado) que si $z=1$ entonces $y=-1$. Escogeremos la solución a la que dandole el valor $z=1$ nos de $-1$.

\paragraph{Hoja 3: Problema 22}

\[\begin{array}{cc}
   x^3+z^3y^3+z &= 0\\
   cos(xyz)+sen(z)-1 = 0
  \end{array}\]
 ¿Es despejable en función de $z$ en un entorno de $(x,y) = (0,0), z=0$.

 Solución:

 1) El punto es solución del sistema.

 2) Definimos \[\appl{F}{\real^3}{\real^2}, F\in C^1, F(0,0,0)=(0,0)\]

 3) Calculamos el determinante de $DF(0,0,0)$ y vemos que da $0$.

 Conclusión: no podemos aplicar el teorema\\
 Supongamos que si se puede despejar. Entonces tendríamos algo de la forma:

 \begin{gather*}
 \left\{\begin{array}{cc}
   [x(z)]^3+z^3[y(z)]^3+z &= 0\\
   cos(x(z)y(z)z)+sen(z)-1 &= 0
  \end{array}\right\}\rightarrow\\
  \,\\
   \left\{ \begin{array}{cc}
               3[x(z)]^3x'(z) + 3z^2[y(z)]^2 + z^32y(z)y'(z) + 1 &=0\\
               -sen(x(z)y(z)z) \cdot\{...\} + cos(z) &= 0
              \end{array}\right\}
              \equiv\\\,\\
              \left\{
              \begin{array}{cc}
               0+1&=0\\
               0+1&=0
              \end{array}\right.
 \end{gather*}
  Esto demuestra que no pueden existir las derivadas.

----------------------




## Definición y ejemplos

##  El teorema del valor medio

## Funciones convexas

## Funciones inversas

## Regla de L'Hospital

## Teorema de Taylor en $\mathbb{R}$

## Método de Newton


<!--chapter:end:104-diferenciacionR.Rmd-->

# Integración de Riemann


En dimensión 1, la teoría de integración la basábamos en la integral de Riemann. Tomábamos una partición de $[a,b]$: $\mathcal{P} = a = t_0 < t_1<...<t_k = b$ y a cada subintervalo de esa partición $I_i =[t_i,t_{i+1}]$ asignábamos dos pares de valores, $M_i$ y $m_i$:

\begin{gather*}
M_i = \sup \{f(x)\tq x\in I_i\}\\
m_i = \inf \{f(x)\tq x\in I_i\}
\end{gather*}

Definíamos las sumas superiores ($\mathbb{U}$) e inferiores ($\mathbb{L}$):

\begin{gather*}
\mathbb{U}(f,\mathcal{P}) = \sum_{i=0}^{k-1} M_i(t_{i+1}-t_i) \\
\mathbb{L}(f,\mathcal{P}) = \sum_{i=0}^{k-1} m_i(t_{i+1}-t_i)
\end{gather*}

Esto nos da una aproximación al área debajo de la función como una suma de rectángulos. Tal y como los hemos definido, está claro que

\[ \mathbb{L}(f,\mathcal{P}) ≤ \int_a^b f ≤ \mathbb{U}(f,\mathcal{P}) \]

También parece obvio que, cuanto más pequeña sea la anchura de los intervalos, más se aproximarán las sumas superiores e inferiores al valor real. Definimos entonces

\begin{gather*}
\alpha = \lim_{\abs{\mathcal{P}}\to 0} \mathbb{U}(f,\mathcal{P}) \\
β = \lim_{\abs{\mathcal{P}}\to 0} \mathbb{L}(f,\mathcal{P})
\end{gather*}

, donde $\abs{\mathcal{P}} = \max t_{i+1} - t-i$, es decir, la anchura máxima de los intervalos que formarn $\mathcal{P}$. A partir de aquí podemos llegar a la definición de función integrable:

\begin{defn}[Función\IS integrable] Se dice que $f$ es integrable en $[a,b]$ si y sólo si

\[ \alpha = \lim_{\abs{\mathcal{P}}\to 0} \mathbb{U}(f,\mathcal{P}) =
\lim_{\abs{\mathcal{P}}\to 0} \mathbb{L}(f,\mathcal{P}) = β \]

La notación es \[ \int_a^b f(x)dx = \alpha = \beta \]
\end{defn}

\begin{theorem}
Si $f$ continua en $[a,b]$ entonces  $f$ es integrable en $[a,b]$.
\end{theorem}

El recíproco es \textbf{falso}. Se ve fácilmente si $f$ es una función escalonada, por ejemplo: podemos calcular el área debajo de ella sin problemas pero no es continua.

\begin{theorem} Sea $f$ integrable en $[a,b]$.

Tomamos $\mathcal{P}_h$ una partición de $[a,b] \tlq \max_{i} \abs{t_{i+1}-t_i} = h$ , es decir, $h$ mide el trozo más grande de la partición.

\[ \lim_{h\rightarrow 0} \sum_{i=1}^{k-1} f(s_i)(t_{i+1}-t_i) = \int_a^bf(x)dx \] para \textbf{cualquier} elección $s_i\in[t_i,t_{i+1}]$

\end{theorem}

\begin{theorem}[Cambio\IS de variable (dimensión 1)]
Sea $g$ un difeomorfismo, y suponemos que es creciente (la cuenta es análoga si fuese decreciente); de tal forma que transforma el intervalo $[a,b]$ en el intervalo $[g(a),g(b)] = [A,B]$. Entonces

\[ \int_A^B f(x)\,dx = \int_{\inv{g}(A)}^{\inv{g}{B}} f(g(t)) g'(t)\,dt \]

Es decir, tenemos cambio de los límites, de las variables y también de la medida.
\end{theorem}

\subsection{Integración en dimensión $1 < N ≤ 3$}

En dimensión mayor que uno teníamos una serie de generalizaciones, y empezábamos con el teorema de Fubini que nos permite el cambio en el orden de integración:

\begin{theorem}[Teorema\IS de Fubini] Sean $A$ y $B$ dos conjuntos compactos. Entonces

\[ \int_A \int_B f(x,y)\,dx\,dy = \int_B \int_A f(x,y)\,dy\,dx \]

En la práctica, tendremos que cambiar los límites de integración para que la integral exprese el mismo área.
\end{theorem}

\begin{wrapfigure}{r}{0.4\textwidth}
\begin{center}
\includegraphics[width=0.4\textwidth]{imgs/AreaInt1.png}
\caption{Integral $I_1$}
\label{imgInt1}
\end{center}
\end{wrapfigure}

Por ejemplo, si tenemos la siguiente integral (ver figura \ref{imgInt1}) \[ I_1 = \int_0^2\int_{y^2}^{2y} f(x,y)\,dx\,dy \] y queremos invertirla cambiamos los límites de integración: \[ I_1 = \int_0^4 \int_{\frac{x}{2}}^{\sqrt{x}} f(x,y)\, dy\,dx \]

Otro ejemplo: estudiemos \[ I_2 = \int_a^bf(x)\,dx = \int_a^b\int_0^{f(x)}dx\,dy \]. Si probamos a cambiar el orden de integración, tenemos que

\[ I_2 = \int_0^M\int_{A(y)}dx\,dy \]

Donde $M$ es el máximo de $f$ y $A(y) = \{ x\in [a,b] \tq f(x) ≥ y \}$. La longitud de ese conjunto $A$ se denomina la medida, y entonces podemos expresar

\[ I_2 = \int_0^\infty \abs{\{x \tq f(x) > y\}}\,dy \] ya que la medida del conjunto será $0$ cuando $y > M$.

Curiosamente, hemos pasado de una integral de Riemann a otra con una expresión distinta, la llamada \textbf{integral de Lebesgue}\index{Integral! de Lebesgue}. Esto pertence al campo de la \textbf{teoría de la medida}, y permite estudiar conjuntos extraños y más monstruos y engendros varios. \label{IntLebesgue}

En general, podemos expresar nuestro cambio de variable de forma más general para cualquier cambio de variable:

\begin{theorem}[Cambio\IS de variable (dimensiones superiores)]
Dados unos conjuntos $D,\,D^\ast$ con $\appl{\Phi}{D}{D^\ast}$ un difeomorfismo, y $\gx \in D;\; \gy \in D^\ast$. Entonces

\[ \int_{D^\ast} f(\gy)\,d\gy = \int_D f(\Phi(\gx)) \abs{\det \dpa{\gy}{\gx}}\,d\gx \]
\end{theorem}

\subsubsection{Integración en curvas}

\begin{defn}[Curva\IS $C^1$]  Se denomina curva en $\real^n$ a una aplicación \begin{align*}
\appl{\gamma}{[a,b]\subset \real&}{\real^n} \\
t&\to \gamma(t) = (x_1(t),\dotsc,x_n(t))
\end{align*}

y con $\gamma\in C^1$.

También exigiremos que la curva sea un \textbf{camino regular}\index{Camino!regular}, es decir que

\[ \gamma'(t) \neq \gor{0} \;\forall t \]

de tal forma que obligamos a que tenga tangente en todo punto.
\end{defn}

Para calcular la longitud aplicamos las ideas básicas del cálculo integral: \textit{troceamos} el intervalo $[a,b]$, y aproximamos cada uno de esos trozos por un segmento. Calculamos la suma de la longitud de esos segmentos, hacemos tender la anchura de los \textit{trozos} y si converge, la longitud se puede medir.

\begin{theorem}[Longitud\IS de una curva] Dada una partición $\mathcal{P} = \{ a= t_0 < t_1 < \dotsb < t_k = b\}$ definimos \[ \abs{\mathcal{P}} = \max_i \abs{t_{i+1} - t_i} \] y la longitud $L$ de la curva.

\[ L(\sigma) = \lim_{\abs{\mathcal{P}}\to 0} \underbrace{\sum_{i=0}^{k-1} \md{\sigma(t_{i+1}) - \sigma(t_i)}}_{=S(\sigma,\mathcal{P})} \]

SI $\sigma\in C^1$, entonces $L(\sigma)$ existe y además

\[ L(\sigma) = \int_a^b \md{\sigma'(t)}\,dt \]

\end{theorem}

Este teorema responde a una idea con respecto al cambio de variable: si tomamos $\Gamma$ como la curva que queremos integrar, entonces se puede expresar

\[ L(\sigma) = \int_\Gamma 1\,d\sigma = \int_a^b \md{\sigma'(t)}\,dt  \]

donde $\md{\sigma'(t)}$ es el cambio en la medida correspondiente.

\begin{proof} Por pura pereza y no escribir más \footnote{A mí también me parece bien} suponemos \[ \sigma(t) = (x(t),y(t)) \]. Tenemos que

\begin{gather*}
 S(\sigma,\mathcal{P}) = \sum_{i=0}^{k-1} \md{\sigma(t_{i+1}) - \sigma(t_i)} = \\
 = \sum_{i=0}^{k-1}\sqrt{\left(x(t_{i+1}-x(t_i)\right)^2 + \left(y(t_{i+1}-y(t_i)\right)^2}
 \end{gather*}

 Por el Teorema del valor medio (\ref{thmTVM1var}) tenemos que

 \begin{gather*}
 \left(x(t_{i+1}-x(t_i)\right)^2  = x'(s_i^1)^2(t_{i+1}-t_i)^2 \\
 \left(y(t_{i+1}-y(t_i)\right)^2  = y'(s_i^2)^2(t_{i+1}-t_i)^2
 \end{gather*}

 Entonces

 \[  S(\sigma,\mathcal{P})  = \sum_{i=0}^{k-1}  (t_{i+1}-t_i) \sqrt{x'(s_i^1)^2 + y'(s_i^2)^2} \]

 No podemos simplificar porque no es seguro que $s_i^1 = s_i^2$. Si fueran el mismo punto, serían sumas de Riemann y habríamos terminado.

 Como tenemos una función continua ($\sigma'$) y estamos trabajando en un intervalo cerrado y acotado ($[a,b]$) podremos reducir la expresión a $\sqrt{x'(t_i)^2 + y'(t_i)^2}$ y que gracias a la continuidad uniforme la diferencia con $\sqrt{x'(s_i^1)^2 + y'(s_i^2)^2}$ se puede hacer todo lo pequeña que queramos, llegando a hacer coincidir en el límite $s_i = t_i$, por lo que podríamos escribir:

\[  S(\sigma,\mathcal{P})  = \sum_{i=0}^{k-1} \sqrt{x'(t_i)^2 + y'(t_i)^2} (t_{i+1}-t_i) \]
  o también:
\[  S(\sigma,\mathcal{P})  = \sum_{i=0}^{k-1} \sqrt{x'(t_{i+1})^2 + y'(t_{i+1})^2} (t_{i+1}-t_i) \]


La forma matemática de escribir este argumento:

Notación: $G(s,t) = \sqrt{(x'(s))^2 + (y'(s))^2}$

Llamamos:
\[(1) = \sum G(s_i^1,s_i^2)(t_{i+1}-t_i)\]
\[(1) = \sum G(t_i^1,t_i^2)(t_{i+1}-t_i)\]

Vamos a estudiar $\abs{(1)-(2)}$

\[0\leq \abs{(1)-(2)} \leq ... \leq \sum_i \abs{G(s_i^1,s_i^2)- G(t_i^1,t_i^2)}(t_{i+1}-t_i)\]

$(s_1^1, s_1^2 \in [t_i,t_{i+1}]$ por tanto:
\[\md{s_i^1,s_i^2) - (t_i,t_i)} = ... \leq \sqrt{2}\md{\mathcal{P}}\]

Aplicamos $G$ continua en $[a,b]\times [a,b]$ (compacto) $\implies G$ uniformemente continua.

\end{proof}

\obs \textbf{Falso} en general si la curva es sólo continua

\paragraph{Ejemplo:}

\[\appl{\sigma}{[0,1]}{\real^2}\]

\todo{A dibujar!}

Descripción gráfica: entre $\frac{1}{2^k}$ y $\frac{1}{2^{k+1}}$ y formo un triángulo isósceles con esos 2 puntos y de altura hasta la bisectriz.

Sea el triangulo K:

\todo{Dibujo}

\[Longitud =L_k = ... ??? ... = \frac{1}{2k+1} \{\sqrt{\frac{1}{4k^2}+1} + \sqrt{\frac{1}{4k^2+4} +1} \} \ge \frac{1}{2k+1}\]
\[\text{Longitud total } = \sum L_k \ge \sum_k \frac{1}{2k+1} = \infty\]

Este mostruito no tiene longitud. ¿Y si en vez de rectas tomamos sinusoides? Esa función si debería ser $C^1$ pero la longitud es $\infty$. Entonces la curva no puede ser $C^1$ (sería un contrajemplo del teorema)

\begin{defn}[Curva\IS rectificable]\label{defCurvaRectf}
Si el límite \[ \lim_{\abs{\mathcal{P}}\rightarrow 0} S(\sigma,\mathcal{P})\] existe entonces $\sigma$ es \textbf{rectificable}.

Además, con comprobar que la curva es $C^1$ es suficiente.

Para que $\sigma$ sea rectificable, basta con que sea continua de Lipschitz, es decir que \[\lim_{x\to x_0} \frac{d(f(x),f(x_0)}{d(x,x_0)}\leq C,\forall x\]

\end{defn}


\subsubsection{Parametrización por longitud de arco}

\[ \appl{\sigma}{[a,b]}{\real^n} \]

con $\sigma$ curva $C^1$ y regular. Entonces

\[ L(s) = \int_a^s \md{\sigma'(t)}\,dt \]

y por el Teorema Fundamental del Cálculo

\[ L'(s) = \md{\sigma'(s)} \]

Al imponer que la curva sea regular, entonces $\sigma'(s)\neq 0$ y por lo tanto existe la inversa $\inv{L}$. Si tenemos entonces un $\tau ∈ [0,L(b)]$, entonces $S=\inv{L}(\tau) ∈ [a,b]$.\wtf

Definimos

\begin{gather*}
\sigma^\ast = \sigma \circ \inv{L} \\
\sigma^\ast = \sigma(\inv{L}(\tau)) \\
(\sigma^\ast)'(\tau) = \sigma'(\inv{L}(tau)) (\inv{L}(\tau))' = \sigma'(\inv{L}(\tau)) \frac{1}{L'(\inv{L}(\tau))} = \sigma'(s) \frac{1}{L'(s)} = \frac{\sigma'(s)}{\md{\sigma'(s)}}
\end{gather*}

Es decir, hemos conseguido una parametrización con velocidad constante $\md{(\sigma^\ast)'} = 1$ y por lo tanto

\[ L(\tau) = \int_0^\tau \md{(\sigma^\ast)'}\,ds = \int_0^s 1\,ds = s \]

\section{Integración en dimensiones superiores}

\subsection{Elemento de área}

Supongamos que estamos en $\real^3$. Podemos hablar de la longitud de una variedad de dimensión 1, del área de una de dimensión 2 o del volumen de una de dimensión 3. Ahora bien, ¿qué ocurre cuando pasamos a dimensiones superiores? La denominación será la siguiente

\begin{itemize}
\item \textbf{1-variedad} Longitud
\item \textbf{k-variedad} $1<k<N$ Área
\item \textbf{N-variedad} Volumen
\end{itemize}

Para calcular esas \textit{cosas} empezaremos partiendo del área de un parelelepípedo.

Definiremos el paralelepípedo como, dados $k$ vectores independientes $\{\gv_i\} \subset \real^N$,

\[ P_k = \sum_{i=1}^k \lambda_i\gv_i\;\lambda_i \in [0,1] \]


Elemento de área: $P_k \equiv \{ \sum_{i=1}^k \lambda_i\gor{v}_i, \lambda_i \in [0,1]\}\subset \real^N$

Definimos una \begin{gather*}
\appl{\Psi}{\real^N}{\real^N}\\
\gx \longrightarrow (\Psi_1(\gx),...,\Psi_n(\gx))
\end{gather*}

\begin{itemize}
\item si $\gx \in P_k \implies \Psi(\gx) = (\Psi_1(\gx),\Psi_2(\gx),...,\Psi_k(\gx),0,...,0)$
\item $\Psi$ mantiene longitudes y ángulos, es decir $\pesc{\Psi(u),\Psi(v)}=\pesc{u,v}, \forall u,v\in\real^N$

Esto implica: $\pesc{\Psi(u),\Psi(v)}=\pesc{u,v} \implies \md{\Psi(\gu)} = \md{\gu}$. Si se conservan los módulos, se conservan también los ángulos.
\end{itemize}

\obs Si $\gx,\gy\in P_k \implies \pesc{\gx,\gy} = \underbrace{\pesc{\Psi(\gx),\Psi(\gy)}}_{\text{Prod } \real^N} = \underbrace{{\tilde{\Psi}(\gx),\tilde{\Psi}(\gy)}}_{\text{Prod } \real^K}$


\textbf{Idea:} Área $(P_k)$ = Área $(\tilde{\Psi}(P_k)) \equiv \displaystyle \int_{\tilde{\Psi}(P_k)}d\gor{s}$, una integral en $\real^K, K<N$



El paso que vamos a dar ahora es: Construir una aplicación $L$ tal que $L(\gor{e}_i) = \tilde{\Psi}(\gor{v}_i)$

Y aplicamos el cambio de variables:
\[\int_{\tlps(P_k)} d\gor{s} = \int_{[0,1]^K} \abs{\det\left( \dpa{s}{t} \right)} d\gor{t}\]

Tenemos:
\begin{itemize}
\item $L$ lineal, $\appl{L}{\real^K}{\real^K}$
\item $L(\gor{e}_j) = \tlps(\gv_j)$.
\end{itemize}
Con la segunda propiedad podemos construir la aplicación $L$.

\begin{gather*}
L = \begin{pmatrix} \tlps(\gv_1) & \tlps(\gv_2) & ... & \tlps(\gv_k)\\
\downarrow & \downarrow & \ddots & \downarrow
\end{pmatrix} = \frac{d\gor{s}}{d\gor{t}}\end{gather*}

\textbf{Conclusión:} \[Area(P_k) = \abs{\det L} = \left|\det \begin{pmatrix}
\tlps(\gv_1) & \tlps(\gv_2) & ... & \tlps(\gv_k)\\
\downarrow & \downarrow & \ddots & \downarrow
\end{pmatrix}\right|\]

\begin{itemize}
\item Necesitamos una manera cómoda con la que construir $\tlps$.
\item ¿Utilizando otra parametrización llegamos al mismo resultado?
\end{itemize}


\[ Area(P_k) = \left( \det \begin{pmatrix}
\tlps(\gv_1) & \tlps(\gv_2) & ... & \tlps(\gv_k)\\
\downarrow & \downarrow & \ddots & \downarrow
\end{pmatrix}
\begin{pmatrix}
\tlps(\gv_1) & \tlps(\gv_2) & ... & \tlps(\gv_k)\\
\downarrow & \downarrow & \ddots & \downarrow
\end{pmatrix} ^T \right)^{\frac{1}{2}}\]
¿Qué ganamos?
\[\begin{pmatrix}
\pesc{\tlps(\gv_1),\tlps(\gv_1)} & \pesc{\tlps(\gv_1),\tlps(\gv_2)} & ... & \pesc{\tlps(\gv_1),\tlps(\gv_k)}\\
\pesc{\tlps(\gv_2),\tlps(\gv_1)} & \pesc{\tlps(\gv_2),\tlps(\gv_2)} & ... & \pesc{\tlps(\gv_2),\tlps(\gv_k)}\\
\vdots & \vdots & \ddots & \vdots\\
\pesc{\tlps(\gv_k),\tlps(\gv_1)} & \pesc{\tlps(\gv_k),\tlps(\gv_2)} & ... & \pesc{\tlps(\gv_k),\tlps(\gv_k)}
\end{pmatrix} = (\ast) = \left(\det(\pesc{v_i,v_j})\right)^{\frac{1}{2}}\]
($\ast$) Hemos construido las cosas de tal manera que se mantiene el producto escalar.

\paragraph{Ejemplo: } $P_2 \subset \real^3$ generado por $\gu,\gv\in\real^2$

$Area(P_2) = \left(\det \begin{pmatrix}
\pesc{\gu,\gu} & \pesc{\gu,\gv}\\
\pesc{\gv,\gu} & \pesc{\gv,\gv}
\end{pmatrix} \right)^{\frac{1}{2}} = \left(\pesc{\gu,\gu}\pesc{\gv,\gv} - \pesc{\gu,\gv}^2\right)^{\frac{1}{2}} =\left(\md{\gu}\md{\gv} - \md{\gu}\md{\gv}(cos(\theta)^2)\right)^2 = \md{u}\md{v} \sqrt{1-cos^2(\theta)}  =  \md{u}\md{v} sen(\theta) = ||u\times v||$

Esto cumple lo que la sabíamos de selectividad. El área de un paralelogramo 2 dimensional en $\real^3$ es la raiz cuadrada del módulo del producto vectorial.

\textbf{Aplicación:} Vamos a aplicar esto para hallar el área de una $k-variedad$ en $\real^N$.

\todo{Dibujo}
\begin{itemize}
\item $\Phi(\gs_0) = \gx_0 \in M$
\item $\Phi(\gs_0 + h_j\gor{e}_j) = \Phi(\gs_0) + \dpa{\Phi}{s_j}(\gs_0)\cdot h_j + err(h)$
Aplicando taylor, en el que cada alargamiento $h$ depende de la dirección.
\end{itemize}

\textbf{Idea:} $Area(\Phi(Q_k)) = Area(P_k) + err(h)$ donde $Area(P_k) = \left(\det (\pesc{v_i,v_j})\right)^{\frac{1}{2}}, \{v_j\}$ genera $P_k$.

\[\left(\det\left(\pesc{\dpa{\Phi}{s_i},\dpa{\Phi}{s_j}}h_ih_j\right)\right)^{\frac{1}{2}}\]

Tomamos $h_i = h, \forall i$

\[\underbrace{\underbrace{h^k}_{Area(Q_k)} \left(\det\left(\pesc{\dpa{\Phi}{s_i},\dpa{\Phi}{s_j}}\right)\right)^{\frac{1}{2}}}_{Area(P_k)}\]

Conclusión: \[Area(M) = \sum_n Area(Q_k^n) \left(\det\left(\pesc{\dpa{\Phi}{s_i}(\gs_0^n),\dpa{\Phi}{s_j}(\gs_0^n)}\right)\right)^{\frac{1}{2}} + err(h)\]

Si llamamos $F(s_0^n) = \left(\det\left(\pesc{\dpa{\Phi}{s_i}(\gs_0^n),\dpa{\Phi}{s_j}(\gs_0^n)}\right)\right)^{\frac{1}{2}}$

Tenemos: \[\sum_n Area(Q_k) F(s_0^n) \convs[Riemann] \int_D F(\gs)d\gs\]

\textbf{Por tanto:} $Area(M) = \int_D \left(\det\left(\pesc{\dpa{\Phi}{s_i},\dpa{\Phi}{s_j}}\right)\right)^{\frac{1}{2}}$

Lo que en Cálculo 2 llamábamos $\md{T_u\times T_v}$.


Dada una $\appl{f}{\real^N}{\real}$ podemos definir: \[\int_{\Phi(D)}f dA = \int_{D}f(\Phi(s)) \left(\det(\pesc{\Phi_{s_i},\Phi_{s_j}})\right)^{\frac{1}{2}} ds\]

\paragraph{Ejemplos}

\subparagraph{Ejemplo 1)}

\[\appl{\sigma}{[a,b]}{\real^N}\]

Sea $\Gamma = \{\sigma(t)\in\real^N\tq t\in[a,b]\}$

El elemento de área sería:

\[\int_{\Gamma} fdA = \int_a^bf(\sigma(t)) (\pesc{\sigma',\sigma'})^{\frac{1}{2}}\]


\subparagraph{Ejemplo 2)}

\[
\Phi : D\subset\real^2\rightarrow \real^3\]
\[(s_1,s_2)\rightarrow (x(s_1,s_2),y(s_1,s_2),z(s_1,s_2))\]

Tenemos en este caso:
\[\int_{\Phi(D)}fdA = \int_D f(\Phi(s_1,s_2)) (\det(\pesc{\Phi_{s_i},\Phi_{s_j}}))^{\frac{1}{2}})ds\]
\[(\det(\pesc{\Phi_{s_i},\Phi_{s_j}}))^{\frac{1}{2}}) = (*) = \md{\Phi_1 \times \Phi_2}\]
$(*)$ visto anteriormente.

Integrales de \textbf{campos} sobre \textbf{curvas} y \textbf{superficies} en $\real^3$.

\begin{itemize}
\item[1] $\Gamma$ curva, $\overrightarrow{F}$ campo. Nos interesa la componente que sigue la tangente de la recta (ya que en la dirección perpendicular no se realiza trabajo). Para ello multiplicamos escalarmente por el vector director normalizado.
\[\int_{\Gamma} \overrightarrow{F}d\sigma \equiv \text{ Trabajo } \equiv \int_{\Gamma} F_T = \int_{\Gamma} \pesc{\overrightarrow{F},\frac{\sigma'}{\md{\sigma'}}}\]
\[ = \int_a^b \pesc{\overrightarrow{F}(\sigma(t)),\frac{\sigma'(t)}{\md{\sigma'(t)}}} \md{\sigma'(t)}dt = \int_a^b \pesc{\overrightarrow{F}(\sigma(t)),\sigma'(t)} dt\]

\item[2] Flujo a través de una superficie.

En este caso, la componente que nos interesa es la perpendicular a la superficie.

$\overrightarrow{n} = T_u\times T_v$

\[\int_{\Phi(D)} \overrightarrow{F} = ... = \int_{D} \pesc{\overrightarrow{F}(\Phi(u,v)),T_u\times T_v}dudv\]
\end{itemize}

Volvemos a plantearnos el problema: ¿Distintas parametrizaciones nos da el mismo trabajo/flujo? Depende de la \textit{orientación} de la parametrización. No es lo mismo el trabajo para ir desde abajo de la curva hasta arriba que para bajarla. ¿Este problema traducido a $\real^K$, flipas o k ase?


Recordamos algunos teoremas y definiciones vistos en Calculo 2:

\subsection{Campos vectoriales}
Los campos vectoriales son funciones $\appl{F}{\real^N}{\real^N}$, en el que a cada punto se le asigna un vector.
\index{Campo!vectorial}

\begin{defn}[Campo\IS conservativo]
Diremos que $F$ es un campo gradiente o conservativo si $\exists \appl{V}{\real^N}{\real}$ tal que $F=\nabla V$.
\end{defn}

\begin{defn}[Divergencia]
En un campo vectorial, la divergencia mide el cambio de volumen y existencia de fuentes o sumideros. Si la divergencia es 0, tenemos un "fluido" incompresible.

\[ \textrm{div}\;F = \frac{∂F_1}{∂x_1} + \cdots + \frac{∂F_n}{∂x_n} \]
\end{defn}

\begin{defn}[Rotacional]
El rotacional mide el giro interno de las partículas en un campo, que se puede expresar como \footnote{En realidad, $\nabla$ no es un vector y esto es sólo una regla mnemotécnica}

\[ \textrm{rot}\;F = \nabla \x \vf \]

Si el rotacional es distinto de cero, significa que ha habido choques internos de las partículas y por lo tanto ha habido pérdida de energía.
\end{defn}

\begin{theorem}
Supongamos que $F\in C^1$ es un campo gradiente. Entonces, $\rot F = \vec{0}$. El recíproco también es cierto.
\end{theorem}


\begin{theorem}[Teorema\IS de Green]
Sea $\Gamma$ una curva simple en $\real^2$. Llamamos $D$ al interior de $\Gamma$. Sea $(P,Q)$ el campo con $P,Q\in C^1(D)$. Entonces

\[ \int_{\Gamma^+} (P,Q)\dif \sigma = \iint_D \frac{\partial Q}{\partial x}-\frac{\partial P}{\partial y}\id{x,y} \]
\end{theorem}

\begin{theorem}[Teorema\IS de Stokes]
Dada $\Gamma$ una curva cerrada simple en $\real^3$ que es el borde de una superficie $S$, tenemos que

\[ \int_{\Gamma^+}\vec{F}\dif \sigma =\iint_{S^+}\rot \vec{F}\dif S \]

Esto indica que el flujo por una superficie depende sólo de la forma de su boca.
\end{theorem}

\begin{theorem}[Teorema\IS de Gauss]
Sea $S$ una superficie cerrada que encierra una región $\Omega$, y $\vec{F}\in C^1(\Omega)$.

\[ \iint_{S^+} \vf \dif S = \iiint_\Omega \dv \vec{F}\, \id{x,y,z} \]
\end{theorem}


Todos estos teoremas son parecidos en cuanto a que a la izquierda se tiene el campo evaluado en la frontera y a la derecha tenemos una integral en el interior de una expresión más o menos compleja en la que aparecen las derivadas. Cabe esperar que sean casos particulares de un teorema superior, cosa que es cierta. Este teorema se le llama de \textbf{Stokes} en general.

De aquí al final de curso nos dedicaremos a llegar a ese teorema y ver que estos 3 teoremas son casos particulares.

Para ello nos adentraremos en el espinoso jardín de la orientación.

\subsection{Orientación}
El tema de la orientación tiene que ver con tener cuidado con el orden. Vamos a ver los ejemplos de pocas dimensiones:

\paragraph{Ejemplos:}

\subparagraph{Ejemplo 1) Bases en $\real^2$}

\[\mathcal{B}_1 = \{(0,1),(1,0)\}\]
\[\mathcal{B}_2 = \{(1,0),(0,1)\}\]

Sea $\gv = (v_1,v_2)_{\mathcal{B}_1} = (v_2,v_1)_{\mathcal{B}_2} \neq \gv$

Lo que haremos en este caso será un cambio de base, $\mathcal{B}_1,\mathcal{B}_2$ bases en $\real^N$. Sea $\mathcal{C}_{\mathcal{B}_1\to\mathcal{B}_2}$ matriz del cambio de base de $\mathcal{B}_1$ a $\mathcal{B}_2$.

\begin{defn}[Orientación]
Diremos que $\mathcal{B}_1,\mathcal{B}_2$ tiene la misma orientación $\dimplies \det \mathcal{C}_{\mathcal{B}_1\to\mathcal{B}_2} > 0$
\end{defn}

¿Que pasaría si el determinante de esa matriz de cambio de base sea 0? No puede ser (por definición de cambio de base, que tiene que ser reversible).

\subparagraph{Ejemplo 2)} $\real^3$.
Sean
\[\mathcal{B}_1 = (\gu,\gv,\gw),\mathcal{B}_2 = (\gv,\gu,\gw),\mathcal{B}_3 = (\gw,\gu,\gv)\]

Si tomamos $\gu = \begin{pmatrix} 1\\0\\0\end{pmatrix}_{\mathcal{B}_1} = \begin{pmatrix}0\\1\\0\end{pmatrix}_{\mathcal{B}_2} = \begin{pmatrix}0\\1\\0\end{pmatrix}_{\mathcal{B}_3} $

Siguiendo este razonamiento llegamos a la matriz de cambio de base:

\[\mathcal{C}_{\mathcal{B}_1\to\mathcal{B}_2} = \begin{pmatrix} 0 & 1 & 0 \\ 1 & 0 & 0 \\ 0 & 0 & 1 \end{pmatrix}\]
Cuyo determinante es negativo.

Lo mismo con

\[\mathcal{C}_{\mathcal{B}_1\to\mathcal{B}_1} = \begin{pmatrix} 0 & 0 & 1 \\ 1 & 0 & 0 \\ 0 & 1 & 0 \end{pmatrix}\]
Cuyo determinante es positivo.

¿Porqué al cambiar el orden se cambia la orientación?

\obs Aceptamos como orientación positiva la de la base canónica ordenada como Dios manda: $\{(1,0,0,...,0), (0,1,0,0,...,0), (0,0,1,0,0,...,0),...,(0,0,...,0,1)\}$

Vamos con algún ejemplo más:

\subparagraph{Ejemplo 3)} (Importante)

En $\real^3$, sean $\gu,\gv$ independientes.

Construimos $\mathcal{B} = \{\gu,\gv,\gu\times\gv\}$. Queremos saber si esta base es de orientación positiva u orientación negativa.

\[\gu\times\gv = \left|
\begin{array}{ccc}
 \overrightarrow{i} & \overrightarrow{j} & \overrightarrow{k}\\
u_1 & u_2 & u_3 \\
v_1 & v_2 & v_3
 \end{array}\right| = ... = \left(\left|\begin{array}{cc}u_2&v_2\\u_3&v_3\end{array}\right|,\left|\begin{array}{cc}u_1&v_1\\u_3&v_3\end{array}\right|,-\left|\begin{array}{cc}u_1&v_1\\u_2&v_2\end{array}\right|\right)\]

 \[\mathcal{B}_{\mathcal{B}\to\mathcal{C}} = \begin{pmatrix}
u_1&v_1& \left|\begin{array}{cc} u_2&v_2\\u_3&v_3 \end{array}\right|\\

u_2&v_2& -\left|\begin{array}{cc} u_1&v_1\\u_3&v_3 \end{array}\right|\\

u_3&v_3& \left|\begin{array}{cc} u_1&v_1\\u_2&v_2\end{array}\right|
 \end{pmatrix}\]

 Cuyo determinante es \[\left|\begin{array}{cc}u_2&v_2\\u_3&v_3\end{array}\right|^2+\left|\begin{array}{cc}u_1&v_1\\u_3&v_3\end{array}\right|^2+\left|\begin{array}{cc}u_1&v_1\\u_2&v_2\end{array}\right|^2>0\]


\subparagraph{Ejemplo 4)} $\real^2$

Sean \[\mathcal{C} = \{(1,0),(0,1)\}\]
\[\mathcal{B} = \{(u_1,u_2),(v_1,v_2)\}\]

La matriz fácil de calcular es \[C_{\mathcal{B}\to \mathcal{C}} = \begin{pmatrix} u_1&v_1\\u_2&v_2\end{pmatrix}\]
\[0<\det \begin{pmatrix} u_1&v_1\\u_2&v_2\end{pmatrix}  = \pesc{(u_1,u_2),(v_1,v_2)} = \pesc{(\lambda,0),(\beta,-\alpha)} = \lambda\beta\]

Aplicando un giro (de aquí salen $\lambda$...) podemos ver que el si el ángulo entre $\gu,\gv \in (0,\pi) \leadsto +$ pero si el ángulo entre $\gu,\gv \in (\pi,2\pi) \leadsto -$. ¿Y en $\pi$? Entonces los vectores no serían independientes.

\textbf{Idea:} Vamos a manipular con los vectores de la base aplicandoles una deformación continua para ver que pasa con la discontinuidad de la orientación en $\pi$ a ver que encontramos.

Sea la deformación $(\alpha(t),\beta(t)), t\in(0,1)$ continua, donde $(\alpha(0),\beta(0)) = (e_1,e_2)$ y $(\alpha(1),\beta(1)) = (e_1,e_2)$

\begin{itemize}
\item
Si la orientación de la base que tengo al final es positiva, entonces podemos encontrar una transformación continua que mantenga positivo el determinante, $\forall t$.
\item
Si la orientación es negativa, entonces \textbf{siempre} det=0 para algún $t$.
\end{itemize}

\paragraph{Vamos a extender la idea anterior} en $\real^3$.

Idea geométrica: Yo tengo 2 bases y quiero pasar de una a otra, si puedo encontrar un camino en el que los 3 vectores nunca pertenezcan al mismo plano entonces la orientación es la misma. \textbf{El orden es fundamental}.

Sea
\[\mathcal{B} = \{e_1,e_2,e_3\} \hspace*{150pt} \mathcal{C} = \{\gu,\gv,\gw\}\]


\hspace*{50pt}
\begin{tikzpicture}[baseline=(X.base)]
\def\R{2.5} % sphere radius
\def\angEl{15} % elevation angle
\def\angAz{-105} % azimuth angle
\def\angPhi{-40} % longitude of point P
\def\angBeta{19} % latitude of point P


%Ecuador
\pgfmathsetmacro\H{\R*cos(\angEl)} % distance to north pole

\tikzset{xyplane/.estyle={cm={cos(\angAz),sin(\angAz)*sin(\angEl),-sin(\angAz),
                              cos(\angAz)*sin(\angEl),(0,0)}}}
\draw[xyplane,<->] (3,0) node[below] {$e_1$} -- (0,0) -- (0,3)
    node[right] {$e_2$};
\draw[->] (0,0) -- (0,3) node[above] {$e_3$};

\end{tikzpicture}
\hspace*{100pt}
\begin{tikzpicture}[baseline=(X.base)]

\def\R{2.5} % sphere radius
\def\angEl{15} % elevation angle
\def\angAz{-105} % azimuth angle

\tikzset{xyplane/.estyle={cm={cos(\angAz),sin(\angAz)*sin(\angEl),-sin(\angAz),
                              cos(\angAz)*sin(\angEl),(0,0)}}}
 \draw[xyplane,<->] (3,0) node[below] {$\gu$} -- (0,0) -- (0,3)
    node[right] {$\gv$};
\draw[->] (0,0) -- (0,-3) node[right] {$\gw$};
\end{tikzpicture}

No hay ninguna manera de llevar $e_3$ a $\gw$ sin formar un único plano con los tres vectores.

Aunque podríamos llevar $e_3 \to \gu$ y $e_1 \to \gw$.

Si no se mantiene el orden, tendríamos la base $\mathcal{C}* = \{\gw,\gv,\gu\}\neq\mathcal{C}$.


\paragraph{Caracterización práctica}
\begin{lemma}
\label{thmProdVect} Si $\gu,\gv$ son vectores independientes, entonces $\{ \gu,\gv,\gu\times\gv \}$ es una base.
\end{lemma}

\begin{lemma} La base $\{\gu,\gv,\gw\}$ tiene orientación positiva si y sólo si $\gw$ y $\gu\times\gv$ están en el mismo lado del espacio respecto del plano generado por $\gu,\gv$ (o, lo que es lo mismo, $\pesc{\gw,\gu\x\gv} > 0$).
\end{lemma}

Ahora que ya tenemos vista la orientación de bases en $\real^N$ vamos a ver la orientación en $T_a M$ (espacio tangente de una variedad en un punto)

\todo{Tipico dibujo de un conjunto en el plano $\real^K$ que la parametrización $\Phi$ lo lleva al espacio.}

Sea $\{e_1,e_2,\dotsc,e_k\}$ la base canónica en $\real^k$, y $\Phi(u_0)=\ga$

Como la variedad viene dada por una parametrización, tomamos $\img D\Phi$, es decir: \[T_{\ga}M = \img D\Phi(u_0)  = \{D\Phi(u_0)\gv,\gv\in\real^K\}\]
Tomando la base euclídea:
\[D\Phi(u_0) \{\sum^k v_i\gor{e}_i\}\equiv \sum^k v_i\underbrace{[D\Phi(u_0)\gor{e}_i]}{\in\real^N} \]

\subparagraph{1)}Es decir, la $\img D\Phi$ está generada por los k vectores \begin{equation}\label{baseTaM}
\{ D\Phi(u_0)\gor{e}_1,\dotsc ,D\Phi(u_0)\gor{e}_k \}
\end{equation}

\subparagraph{2)}
La condición de rango máximo nos asegura que los $k$ vectores son linealmente independientes.

\paragraph{Conclusión:} El conjunto (\ref{baseTaM}) es una base de $T_{\ga}M$

\textit{Problema} Si tenemos 2 parametrizaciones distintas $\Phi,\Psi$ entonces tendremos 2 bases diferentes. Cabe plantearse bajo qué condiciones se mantiene la orientación. (aunque todavía no tengamos muy claro que es la orientación de una variedad)

\paragraph{Ejemplos:}
\subparagraph{1)} Las orientaciones de una curva en $\real^N$ es fácil, basta comprobar los sentidos de los vectores tangentes.

Vamos a hacer las cuentas:

Sean $\sigma,\beta$ parametrizacones del mismo trozo de la curva, que parten de orígenes distintos.

\[\appl{\sigma}{U}{\Gamma},s\to \sigma(s)\]
\[\appl{\beta}{V}{\Gamma},t\to \beta(t)\]

Tenemos un teorema que nos garantiza que existe un \textbf{difeomorfismo} (\ref{TeoremaDifeomorfismo})g, tal que \[\sigma(s) = \beta(g(s)) \y \sigma'(s) = \beta'(g(s))\cdot g'(s)\]

En este caso, para que las dos parametrizaciones den la misma orientación, $g'>0$.

\subparagraph{2)} Las orientaciones de una superficie también, basta comprobar los sentidos de los vectores normales.

\[\appl{\Phi}{U}{\real^3}, (u,v) \to \Phi(u,v)\]
\[\appl{\Psi}{V}{\real^3}, (r,s) \to \Psi(r,s)\]

Tenemos un teorema que nos garantiza... tal que \[g(u,v) = (g_1(u,v),g_2(u,v))\]

En este caso, calculamos \[\left.\begin{array}{c}
\Phi_u\times\Phi_v \\
\Psi_r\times\Psi_s
\end{array}\right\}\]

Tenemos que $\Phi(u,v) = \Psi(g_1(u,v),g_2(u,v))$

\begin{gather*}
\Phi_1(u,v) = \Psi_1(g_1(u,v),g_2(u,v))\\
(\Phi_1)_{u} = (\Psi_1)_r r_u + (\Psi_1)_s s_u = ((\Psi)_r\,(\Psi_1)_s)\begin{pmatrix}
(g_1)_u\\(g_2)_v
\end{pmatrix}
\end{gather*}
Se calculan las 6 derivadas $(\Phi_1,\Phi_2,\Phi_3)$ respecto de $u$ y de $v$ \emph{Teniendo cuidado de en donde evaluamos que derivadas} y acabamos llegando a

\[\begin{pmatrix}
(\Phi_1)_u\\(\Phi_2)_u\\(\Phi_3)_u
\end{pmatrix} = \begin{pmatrix}
(\Psi_1)_r & (\Psi_1)_s\\
(\Psi_2)_r & (\Psi_2)_s\\
(\Psi_3)_r & (\Psi_3)_s
\end{pmatrix}\begin{pmatrix}
(g_1)_u\\
(g_2)_u
\end{pmatrix}
\]
Análogamente:
\[\begin{pmatrix}
(\Phi_1)_v\\(\Phi_2)_v\\(\Phi_3)_v
\end{pmatrix} = \begin{pmatrix}
(\Psi_1)_r & (\Psi_1)_s\\
(\Psi_2)_r & (\Psi_2)_s\\
(\Psi_3)_r & (\Psi_3)_s
\end{pmatrix}\begin{pmatrix}
(g_1)_v\\
(g_2)_v
\end{pmatrix}
\]

Ahora procedemos a calcular
\[\Phi_u\x\Phi_v = \dotsc = \left(
\left|\begin{array}{cc}
(\Phi_2)_u & (\Phi_2)_v\\
(\Phi_3)_u & (\Phi_3)_v
\end{array}
\right|,-
\left|\begin{array}{cc}
(\Phi_1)_u & (\Phi_1)_v\\
(\Phi_3)_u & (\Phi_3)_v
\end{array}
\right|,
\left|\begin{array}{cc}
(\Phi_1)_u & (\Phi_1)_v\\
(\Phi_2)_u & (\Phi_2)_v
\end{array}
\right|
\right)\]

Tomando el primer elemento calculamos:

\[
\det\left(
\begin{array}{cc}
(\Psi_2)_r & (\Psi_2)_s\\
(\Psi_3)_r & (\Psi_3)_s
\end{array}
\right)\begin{pmatrix}
(g_1)_u &(g_1)_v \\
(g_2)_u & (g_2)_v
\end{pmatrix} =
\left| \begin{array}{cc}
(\Psi_2)_r & (\Psi_2)_s\\
(\Psi_3)_r & (\Psi_3)_s
\end{array}\right| \det Dg
\]

Repitiendo la cuenta con el resto de los elementos, llegamos a

\[\Phi_u\x\Phi_v = \Psi_r\x\Psi_s\cdot (\det Dg)\]

\paragraph{Conclusión} Para mantener la orientación necesitamos $\det Dg > 0$

\begin{defn}[Orientación \IS en $\real^N$]
Sean $\Phi,\Psi$ parametrizaciones de una subvariedad k-dimensional en $\real^N$, con $g \equiv$ cambio de variables tal que $\Phi=\Psi \circ g$.
Entonces $\Phi,\Psi$ inducen la misma orientación $\dimplies \det Dg>0$
\end{defn}

\obs Este teorema solo afecta a la zona de la subvariedad $M$ parametrizada por $\Phi$ y $\Psi$ al mismo tiempo.

\paragraph{Ejemplo de superficies no orientables}

\subparagraph{Banda de Moebius}
\begin{center}
\includegraphics[width=0.5\textwidth]{imgs/Moebius.jpg}
\end{center}
\index{Banda de Moebius}


La parametrización es
\[
\Phi(t,\theta) = \left((R+t\cdot sen\frac{\theta}{2})cos\theta, (R+t\cdot sen\frac{\theta}{2})sen\theta, t cos\frac{\theta}{2} \right) \, t\in(-1,1),\theta\in(0,2\pi)
\]

¿Estamos seguros de que es una parametrización?
\begin{itemize}
\item Regular ($C^1$)
\item $D\Phi$ rango máximo (Fácil)
\item Homeomorfismo
\end{itemize}

Vamos a comprobar el homeomorfismo,

Tenemos 2 posibles caminos:

\subparagraph{1)} Despejamos  en función de $x,y,z$

$\frac{y}{x} = tg \theta$.

Definimos \footnote{Utilizando: (\ref{ImgCirc2})}: \[
\begin{array}{ccc}
\theta &= arctg\frac{y}{x} & (1)\\
\theta &= arctg\frac{y}{x} + \pi & (2)\\
\theta &= arctg\frac{y}{x} + 2\pi & (3)
\end{array}
\]
Y comprobar que es continua


\subparagraph{2)} Escribimos este conjunto como un conjunto de nivel y ver que es una variedad, por lo tanto no hace falta comprobar el homeomorfismo sobre la imagen.

\begin{gather*}
\sqrt{x^2+y^2} = (R + t\cdot cos\frac{\theta}{2})\\
\sqrt{x^2+y^2} - R = \frac{z}{tg\frac{"arctg\frac{y}{x}"}{?}}
\end{gather*}


\subparagraph{Orientación}

Una clave importante es que cuando $\theta\rightarrow 0^+ \implies \Phi(t,\theta)$ pero si $\theta\rightarrow 2\pi^{-} \implies \Phi(-t,\theta)$

$\overrightarrow{n} = T_t\x T_{\theta} = ... = \overrightarrow{n}(t,\theta)$

\begin{gather*}
\overrightarrow{n}(t,\theta) \convs[][\theta\rightarrow 0^+] (-R,\frac{t}{2})\\
\overrightarrow{n}(t,\theta) \convs[][\theta\rightarrow 2\pi^-] (R,-\frac{t}{2})
\end{gather*}

Nota: esta parametrización que no cubre el segmento con el que se empieza. Esta parametrización tiene una propiedad curiosa, al empezar, el vector normal apunta hacia dentro y al final, apunta hacia fuera. Es imposible cubrirla del todo con una parametrización.

\paragraph{El otro ejemplo} típico de superficie no orientable es la botella de Klein

\begin{center}
\includegraphics[width=0.5\textwidth]{imgs/botella-de-klein.png}
\end{center}


\paragraph{Variedades con borde}

Conjuntos con frontera en $\real^2$.

Utilizamos la tercera caracterización de subvariedad, que dice que existe un \textbf{difeomorfismo} que vamos a llamar $\Phi$, (que por ser difeomorfismo, existe $\Psi = \Phi^{-1})$.

Podemos suponer que estamos trabajano con un cuadrado en el plano y su imagen para facilitar las cuentas.

Partimos de \begin{itemize}
\item $\Psi(s_0,0) = (x_0,y_0)\in dM$ (la frontera de $M$)
\item $\Psi(s_0,0) \in dM$
\item $\Psi(s,t) \in M, t>0 (s,t)\in U$
\end{itemize}

En U es fácil orientar un cuadrado. ¿Cómo nos "llevamos" la orientación? Con la diferencial, que si queremos que sea la misma orientación $\implies \det D\Phi > 0$.

Sea $\mathcal{C} = \{e_1=(1,0),e_2=(0,1)\}$ base canónica en $\real^2$ (variables (s,t)).

Sea $\mathcal{B} = \{D\Psi(s_0,0)e_1,D\Psi(s_0,0)e_2\}$ base en $\real^2$ (variables $(x,y)$)

Tenemos también $\sigma(s) = \Psi(s,0)$ parametrización de un trozo de $dM$ que contiene a $x_0$.

\[D\Psi = \begin{pmatrix}
\displaystyle\dpa{\Psi_1}{s} &\displaystyle\dpa{\Psi_1}{t}\\
\displaystyle\dpa{\Psi_2}{s} &\displaystyle\dpa{\Psi_2}{t}
\end{pmatrix}\]
En la primera columna lo que tenemos es el vector tangente a la curva. Cuando $t=0$ tenemos la parametrización de la frontera.

\[
D\Psi|_(s_0,0) = \begin{pmatrix}
\sigma'(s_0) & \overrightarrow{v}\\
\downarrow & \downarrow
\end{pmatrix}
\]

Haciendo un desarrollo de Taylor tenemos:

\[
\Psi(s_0,t) = \begin{pmatrix}
\Psi_1(s_0,0)\\
\Psi_2(s_0,0)
\end{pmatrix} + t \underbrace{\begin{pmatrix}
\dpa{\Psi_1}{t} (s_0,0)\\
\dpa{\Psi_2}{t} (s_0,0)
\end{pmatrix}}_{\gor{v}} + err
\]

\[\underbrace{\begin{pmatrix}\Psi_1(s_0,t)\\
\Psi_2(s_0,t)
\end{pmatrix} }_{\in M\, t>0}= \gor{x}_0 + t\gv + err
\]
Conclusión: $\gv$ "apunta hacia el interior de $M$".

\subparagraph{Orientación}
\[\mathcal{C} = \{e_1,e_2\}\]
\[\mathcal{B} = \{D\Psi(s_0,0)e_1,D\Psi(s_0,0)e_2\} = \{\sigma'(s_0),\gv\}\]

\[\mathcal{B} \text{ orientación positiva } \dimplies \det D\Psi(s_0,0) > 0 \dimplies \text{ Ángulo entre } \sigma'(s_0) \text{ y } \gv \in (0,\pi)\]

Con un dibujo se llegaría a entender perfectamente  la siguiente conclusión (basada en la interpretación geométrica de que el ángulo $\in (0,\pi)$)

\index{Orientación\IS de una subvariedad}
\textbf{Conclusión} si recorremos la frontera de la subvariedad	 con la mano izquierda hacia dentro es la orientación positiva si nuestra subvariedad queda en el interior de esa frontera/curva, si nuestra subvariedad es el exterior de la curva pues será la orientación negativa.

\paragraph{Ejemplo}

\[\appl{\Phi}{\real^2}{\real^3}\]

Tenemos $\sigma(s) = \Phi(s,0) $, parametrización de un trozo de $dM$ que contiene a $x_0$.

Siendo \[D\Phi(s_0,0) = \begin{pmatrix}
...
\end{pmatrix} = \begin{pmatrix}
\sigma'(s_0) & \overrightarrow{v}\\
\downarrow & \downarrow
\end{pmatrix}\]

\textbf{Orientación:}

\[\mathcal{C}  = \{e_1,e_2,e_3\}\]

\[\mathcal{B} = \{D\Phi(s_0,0)e_1,D\Phi(s_0,0)e_2\} = \{\sigma'(s_0),\gv\}\]

Solo se tienen 2 vectores. Anteriormente hemos visto que es el producto vectorial (\ref{thmProdVect})

Es decir

\[\mathcal{B} = \{\sigma'(s_0),\gv,\sigma'(s_0)\x\gv\}\]

Con las cuentas vistas antes del ejemplo comprobamos que $\gv$ apunta hacia el interior de $M$.

Hola mundo



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

---
output:
  html_document: default
  pdf_document: default
---
# Integración de formas diferenciales

Una forma diferencial es una  funcion escalar definida en un abierto de $\real^n$
\[\appl{f}{\Omega\subset\real^N}{\real}\]
Operaciones habituales:
\begin{itemize}
\item Suma: sí
\item Producto: sí
\item Composiciones: no (porque no cuadran las dimensiones)
\end{itemize}
\paragraph{1-formas}
\index{Formas!1}
Sea $\mathcal{C} = \{e_1,e_2,...,e_n\}$ la base canónica en $\real^N$.
Sea $L$ una aplicación lineal
\[\appl{L}{\real^N}{\real}\]
Que recordamos que cumplen:
\[ L(\gx+\gy) = L(\gx)+L(\gy); L(\lambda\gx) = \lambda L(\gx)\]
Definimos $\gy\in\real^N \leadsto \gy = \displaystyle\sum_1^n y_i e_i$, con lo que \[L(\gy) = \sum y_i L(e_i)\]
Entonces \[\left.\begin{array}{cc}
v_i = L(e_i)\\
y_i = P_i(\gy)
\end{array}\right\} \rightarrow L(\gy) = \sum_i v_iP_i(y)\]
Siendo $P_i$ las proyecciones, una base del espacio dual.
\textbf{Notación:}
$P_i \equiv dx_i$.
$dx_i[\gy] \equiv P_i(\gy) = y_i$
Entonces, dado un $\gv$ podemos construir
\[L \equiv \sum_i^N v_idx_i\]
\[L[\gy] = \sum_i^N v_idx_i[\gy] = \sum_i^N v_iy_i\]
\begin{defn}[1-forma]
\[\omega(\gx)= \sum_1^N F_i(\gx) dx_i\]
\begin{itemize}
\item Se evalúa en $\gx\in\real$
\item Actúa sobre $\gy\in\real^N$
\end{itemize}
Es decir, \[\omega(\gx)[\gy] = \left(\sum F_i(\gx)dx_i\right)[\gy] = \sum F_i(\gx)dx_i[\gy] = \sum F_i(\gx)y_i\]
\end{defn}
Indicaremos con paréntesis el punto en el que estamos evaluando, y con corchetes el punto en el que estamso actuando.
\textbf{Operaciones:}
\begin{itemize}
\item Sumar: sí (lo razonable)
\item Multiplicar: por una función escalar sí está definida.
\end{itemize}
\paragraph{Ejemplo:}
Supongamos $f$ una función escalar (una 0-forma).
\[\grad f(\gx) = \left( \dpa{f}{x_i}(\gx)\right)\, i=1,...,N\]
Nos podemos construir una 1-forma desde el gradiente
\[\dpa{f}{x_i}(\gx)dx_i \]
A esta 1-forma en particular la llamaremos $df(\gx)$.
¿Utilidad? Ya la veremos, pero es una forma de escribir el producto escalar.
\[\pesc{\grad f(\gx),\gy} = df(\gx)[\gy]\]
\paragraph{2-formas}
\index{Formas!2}
Punto de partida: Aplicaciones \textbf{bilineales alternadas}
\[\appl{\Phi}{\real^N\x\real^N}{\real}\]
Que cumplen \begin{itemize}
\item $\Phi([\gu,\gv]) = - \Phi([\gv,\gu]) \implies \Phi(\gu,\gu)=0$
\item $ \Phi([\gu+\gv,\gw]) = \Phi ([\gu,\gw]) + \Phi([u,w])$
\item$\Phi([\lambda \gu,\gv]) = \lambda \Phi([\gu,\gv])$
\end{itemize}
Consecuencias:
\begin{itemize}
\item $\Phi(\gor{r}, \gor{s}+\gor{t}) = \Phi(\gor{r}+\gor{s}) + \Phi(\gor{r}+\gor{t})$
\item $\Phi(\gu,\mu\gv) = \mu\Phi(\gu,\gv)$
\end{itemize}
\paragraph{Ejemplo} en $\real^3$ para facilitar las cuentas.
\[\Phi(\gu,\gv) = \Phi(u_1e_1+u_2e_2+u_3e_3,v_1e_1+v_2e_2+v_3e_3)\]
Aplicando las propiedades anteriores obtenemos:
\begin{gather*}
\overbrace{u_1v_1\Phi(e_1,e_1)}^{\equiv 0} + u_1v_2\Phi(e_1,e_2) + u_1v_3+\Phi(e_1,e_3)+\\
u_2v_1+\Phi(e_2,e_1)+u_2v_2+\Phi(e_2,e_2)+u_2v_3+\Phi(e_2,e_3)+\\
u_3v_1\Phi(e_3,e_1)+u_3v_2+\Phi(e_3,e_2)+u_3v_3+\Phi(e_3,e_3) = \\
\underbrace{(u_1v_2-u_2v_1)}_{\left|\begin{matrix}
u_1&u_2\\v_1&v_2
\end{matrix}\right|}\overbrace{\Phi(e_1,e_2)}^{C_1}+(u_1v_3-u_3v_1)\Phi(e_1,e_3)+(u_2v_3-u_3v_2)\Phi(e_2,e_3)
\end{gather*}
Hemos demostrado que \[\Phi(\gu,\gv) = C_1B_{12}(\gu,\gv) + C_2B_{13}(\gu,\gv) + C_3B_{23}(\gu,\gv)\]
\subparagraph{Notación:} $B_{ij} = dx_i\y dx_j$
\[dx\y dx_j [\gu,\gv] = \det \begin{pmatrix}
u_i&u_j\\v_i&v_j
\end{pmatrix} = \det \begin{pmatrix}
dx_i[\gu]&dx_j[\gu]\\dx_[\gv]&dx_j[\gv]
\end{pmatrix}\]
\begin{defn}[2-forma]
\[\beta = \sum_{i,j=1}^N F_i(\gx) dx_i\y dx_j\]
\begin{itemize}
\item Se evalúan en puntos $x\in\real^N$
\item Actúan sobre pares de vectores $[\gu,\gv]\in\real^N\x\real^N$.
\end{itemize}
Es decir:
\[\beta(\gx)[\gu,\gv] = \sum F_{ij}(\gx) dx_i\y dx_j[\gu,\gv] = \sum F_{ij} \det \begin{pmatrix}
u_i&v_i\\u_j&v_j
\end{pmatrix}\]
\emph{Ojo} El cambio del orden (en el determiante)es aposta por la segunda propiedad de las 2 formas
\end{defn}
\subsection{Generalización: k-formas}
\index{k-forma}
\index{Formas!k}
Vamos a dar una definición general de una k-forma.
Elementos básicos:
\[\dfl{x_{i_1}}{x_{i_k}}[\gu^1,\gu^2,...,\gu^k] = \det\begin{pmatrix}
u_{i_1}^1 & ... & u_{i_k}^1\\
\vdots & \ddots & \vdots\\
u_{i_1}^k & ... & u_{i_k}^k
\end{pmatrix}\]
\begin{defn}[K-forma] Una k-forma es una expresión como la que sigue
\[
\sum_{i_1,...,i_k=1}^N F_{i_1,...,i_k}(\gx)\dfl{x_{i_1}}{x_{i_k}}
\]
Se evalúa en puntos $\gx\in\real^N$ y actúa sobre grupos de $K$ vectores.
\end{defn}
\begin{lemma} Si dos índices están repetidos, la diferencial vale 0:
\[ i_j = i_s \implies \df{x_{i_j},x_{i_s}} = 0 \]
\end{lemma}
Esto nos dice que en $\real^N$, teniendo $K$-formas (con $K<N$) tenemos $\comb{N}{K}$ combinaciones distintas.
\obs Si $K>N$ y $\omega$ es una k-forma, entonces $\omega \equiv 0$
\paragraph{Ejemplos:} En $\real^3$.
\begin{itemize}
\item 0-forma $\leadsto f(x,y,z) = 0$
\item 1-forma $\leadsto f_1(x,y,z)\df x + f_2(x,y,z)\df y + f_3(x,y,z)\df z$
\item 2-forma $\leadsto g_1(x,y,z)\df{y,z} + g_2(x,y,z)\df{z,x} + g_3(x,y,z)\df{x,y}$
\item 3-formas $\leadsto h(x,y,z)\df{x,y,z}$
\end{itemize}
\index{Orden!cíclico}
\emph{Ojo} Al cambio en la 2-forma, que es $dzdx$. Esto es para seguir el \textbf{orden cíclico} (por temas de la orientación). Esto es $x\to y \to z \to x$
\obs Las \textit{funciones escalares} las podemos interpretar como 0-formas y como 3-formas. Los \textit{campos vectoriales} los podemos interpretar como 1-formas y también como 2-formas.
\paragraph{Notación}
Para escribir un conjunto de subíndices $\{i_1,i_2,...,i_k\} \equiv I$
También acortaremos $\dfl{x_{i_1}}{x_{i_k}} \equiv dx_I$.
La definición quedaría $\displaystyle \sum_I F_I(\gx)dx_I$
\subsection{Operaciones}
Siempre se puede multiplicar por 0-formas y sumar formas del mismo orden. Estas operaciones son triviales porque son operaciones internas.
Vamos a definir las operaciones externas:
\subsubsection{Producto exterior}
\begin{defn}[Producto\IS exterior]
Sean
\begin{gather*}
\omega = \sum_I F_I \df x_I\quad (\text{k-forma}\,\in\real^N) \\
\beta = \sum_J G_j \df x_J\quad (\text{s-forma}\,\in\real^N)
\end{gather*}
Se define el producto exterior de $ω$ y $β$ de la siguiente forma
\[\omega\y\beta = \sum_{I,J} F_IG_J \df{x_I,x_J} (\text{k+s-forma})\]
\end{defn}
\obs Si $K+S>N \implies \omega\y\beta=0$
Vamos a por un ejemplo de producto exterior en $ℝ^3$. Consideramos las dos siguientes formas diferenciales:
\begin{gather*}
\omega = f_1(x,y,z)\df x + f_2(x,y,z)\df y + f_3(x,y,z) \df z \\
\beta= g_1(x,y,z)\df x + g_2 (x,y,z) \df y + f_3 (x,y,z) \df z
\end{gather*}
y calculamos su producto exterior, $\omega\y\beta$
\begin{multline*}
\omega\y\beta  = f_1g_1\df{x,x} + f_1g_2\df{x,y} + f_1g_3\df{x,z} + f_2g_1\df{y,x} +\\
+ f_2g_2\df{y,y}+ f_2g_3\df{y,z}  + f_3g_1\df{z,x}+f_3g_2\df{z,y}+f_3g_3\df{z,z}
\end{multline*}
Tachamos los que sean 0 ($\df{x,x} = 0$) y tenemos cuidado con el orden cíclico, y nos queda
\[ (f_2g_3-f_3g_2)\df{y,z} + (f_3g_1-f_1g_3)\df{z,x} + (f_1g_2 - f_2g_1) \df{x,y} \]
Partiendo de 2 campos vectoriales que eran 1-formas hemos llegado a una 2-forma. Además, si nos fijamos, hemos llegado a la definición de \textbf{producto vectorial} en $ℝ^3$:
\[ \overrightarrow{F} \x \overrightarrow{G} =
\left((f_2g_3-f_3g_2),(f_3g_1-f_1g_3),(f_1g_2 - f_2g_1)\right) \]
\subsubsection{Diferencial exterior}
El diferencial exterior trata de ampliar el concepto del diferencial (la matriz de derivadas parciales) más allá de las funciones, de tal forma que podamos aplicarlo a formas diferenciales.
\begin{defn}[Diferencial\IS exterior] Definimos la diferencial exterior de una k-forma como
\[\dif ω = \dif \left(\sum_I F_i(\gx)\df x_I\right) = \sum_I \underbrace{\df F_I}_{\text{1-forma}} \overbrace{\y}^{\text{Prod. ext}} \underbrace{\df x_I}_{\text{k-forma}} \]
donde
\[ \dif f = \sum_i^N \dpa{f}{x_i} \df x_i \]
La diferencial exterior de una k-forma es una k+1-forma.
\end{defn}
Veamos algunos ejemplos, empezando en $ℝ^3$.
Partimos de un campo vectorial $G = (g_1,g_2,g_3)$ al que asociamos una 2-forma $ω$:
\[ \omega = g_1 \df{y,z} + g_2 \df{z,x} + g_3 \df{x,y} \]
Calculamos ahora la diferencial exterior, $\dif\omega$. Para calcularla, recordamos que $\df{x,x} = 0$ y que podemos cambiar el orden del producto exterior si respetamos el orden cíclico ($x,y,z$).
\begin{align*}
\dif\omega 	&= 	\df{g_1,y,z} + \df{g_2,z,x} + \df{g_3,x,y} = \\
			&= 	\left(\dpa{g_1}{x} \df x + \dpa{g_1}{y} \df y + \dpa{g_1}{z}\df z \right)\y \df{y,z}\\ &\qquad
			+	\left(\dpa{g_2}{x} \df x + \dpa{g_2}{y} \df y + \dpa{g_2}{z}\df z \right)\y \df{z,x}\\ &\qquad
	 		+	\left(\dpa{g_3}{x} \df x + \dpa{g_3}{y} \df y + \dpa{g_3}{z}\df z \right)\y \df{x,y} = \\
			&= \dpa{g_1}{x}\df{x,y,z} + \dpa{g_2}{y}\df{y,z,x} + \dpa{g_3}{z}\df{z,x,y} = \\
			&= \left(\dpa{g_1}{x} + \dpa{g_2}{y} + \dpa{g_3}{z}\right)\df{x,y,z}
\end{align*}
Hemos llegado a una 3-forma que además es la forma diferencial asociada a la \textbf{divergencia} de $G$.
Pasamos a otro ejemplo, donde vamos a calcular la diferencial exterior de una 1-forma $ω=F_1\df x + F_2 \df y + F_3 \df z$. Recordamos que si invertimos el orden del producto exterior pagamos con un cambio de signo, esto es, $\df{x,z} = - \df{z,x}$.
\begin{align*}
\dif ω 	&= \dif\left(F_1\df x + F_2\df y+F_3\df z\right) =\\
		&= \df{F_1,x} + \df{F_2,y} + \df{F_3,z} = \\
		&= \left(\dpa{F_1}{x}\df x + \dpa{F_1}{x}\df y + \dpa{F_1}{x}\df z \right)\y \df x +
\left(\dpa{F_2}{x}\df x + \dpa{F_2}{x}\df y + \dpa{F_2}{x}\df z \right)\y \df y + \\ & \qquad \qquad
		+  \left(\dpa{F_3}{x}\df x + \dpa{F_3}{x}\df y + \dpa{F_3}{x}\df z \right)\y \df z = \\
		&= \left(\dpa{F_3}{y} - \dpa{F_2}{z} \right)\df{y,z} + \left(\dpa{F_1}{z} - \dpa{F_3}{dx}\right)\df{z,x} +
\left(\dpa{F_2}{x} - \dpa{F_1}{y}\right) \df{x,y}
\end{align*}
Nos ha quedado un campo de la forma:
\[\left(\left(\dpa{F_3}{y} - \dpa{F_2}{z} \right) ,\left(\dpa{F_1}{z} - \dpa{F_3}{x}\right),\left(\dpa{F_2}{x} - \dpa{F_1}{y}\right)\right)\]
que coincide con el \textbf{rotacional}.
\paragraph{Propiedades de la diferencial exterior}
\subparagraph{Diferencial de la suma} $\dif(\omega + \beta) = \dif\omega + \dif\beta$
\subparagraph{Diferencial del producto} Siendo $\omega = \sum_I F_I \dif x_I$ una k-forma, $f$ una 0-forma, tenemos que
\[ f\omega = \sum_I fF_I\dif x_I \]
y entonces
\[ \dif (f\omega) = \sum_I \df{(fF_I),x_I} \]
, donde \[ \dif (fF_I) = \sum_{j=1}^N \dpa{fF_I}{x_j} \df x_j = \sum_{j=1}^N\dpa{f}{x_j} F_I \df x_j + \sum_{j=1}^N\dpa{F_I}{x_j} f \df x_j = F_I \dif f + f \dif F_I \]
De esta forma, nos queda que
\begin{align*}
\dif (fω)	&= \sum_I \left(F_I \dif f + f \dif F_I\right)\y \dif x_I = \\
			&= \sum_I F_I \df{f,x_I} + \sum_I f \df{F_I,x_I} = \\
			&= \sum_I \dif f \y F_I \dif x_I + f \dif ω = \\
			&= \dif f \y \left(\sum_I F_I \dif x_I\right) + f \dif ω = \\
			&= ω \df{f} + f \dif ω
\end{align*}
Hemos llegado a una expresión similar a la de la derivada de un producto de funciones
\[d(f\omega) = ω \df{f} + f \dif ω \]
\subparagraph{Diferencial del producto exterior}
Sean dos k-formas diferenciales $ω$ y $β$:
\[ \omega =\sum f_i \df x_i ;\; \beta = \sum_j  g_j\df x_j \]
Calculamos el diferencial de su producto exterior:
\begin{align*}
\dif (\omega \y \beta) &= \dif\left(\sum_{i,j=1}^N f_ig_jdx_y\y dx_j\right) =\\
	&= \sum_{i,j=1}^N \df{(f_ig_j),x_i,x_j} = \\
	&= \sum_{i,j=1}^N \left(\sum_{k=1}^N \dpa{(f_ig_j)}{x_k} \dif x_k\right)\y \df{x_i,x_j} = \\
	&= \sum_{i,j,k=1}^N \left(\dpa{f_i}{x_k}g_j + f_i\dpa{g_j}{x_k}\right) \df{x_k,dx_i,dx_j} = \\
	&= \sum_{i,j,k=1}^N \dpa{f_i}{x_k}g_j \df{x_k,dx_i,dx_j}+ \sum_{i,j,k=1}^N f_i\dpa{g_j}{x_k}\df{x_k,dx_i,dx_j}
\end{align*}
Ahora tratamos de encontrar $ω$ y $β$ en ese engendro para volver a una expresión más agradable:
\begin{align*}
\dif (\omega \y \beta) &= \sum_{i,j,k=1}^N \dpa{f_i}{x_k}g_j \df{x_k,x_i,x_j}
	+ \sum_{i,j,k=1}^N f_i\dpa{g_j}{x_k}\df{x_k,dx_i,dx_j} \\
	&= \sum_{i,j,k=1}^N \dpa{f_i}{x_k}\df{x_k,x_i}\y(g_j\df x_j)
	+ \sum_{i,j,k=1}^N\dpa{g_j}{x_k}\df{x_k} \y f_i \df{x_i,dx_j} = \\
	&= \sum_{i} \left(\sum_k \dpa{f_i}{x_k}\df{x_k}\right) \y \dif x_i \y  \left(\sum_j g_j\dif x_j\right) \\ &\qquad
	+  \sum_{j} \left(\sum_k \dpa{g_j}{x_k}\df{x_k}\right) \y \left(\sum_i f_i\dif x_i\right) \y \dif x_j = \\
	&= \sum_i \df{f_i,x_i} \y β + \sum_j \df{g_j} \y ω \y \dif x_j = \\
	&= \left(\sum_i \df{f_i,x_i}\right) \y β - ω \y \left(\sum_j \df{g_j,x_j}\right) = \\
	&= \dif ω \y β - ω \y \dif β
\end{align*}
Entonces, si $\omega,\beta$ son 1-formas tenemos que $\dif(\omega \y \beta) = \dif\omega \y \beta - \omega \y\dif\beta$. Si por el contrario tuviésemos que $\omega$ es una k-forma y $\beta$ una s-forma, repitiendo las cuentas de nuevo llegaríamos a
\[\dif \omega \y \beta + (-1)^k \omega \y \dif\beta\]
\subparagraph{Diferencial del diferencial}
Sea $\omega$ k-forma con coeficientes $C^2$. Entonces,
\[ \dif (\dif ω) = 0 \]
\paragraph{Propiedades del diferencial exterior} Resumiendo las propiedades del diferencial:
\index{Diferencial!propiedades}
\begin{itemize}
\item $\dif (ω + β) = \dif ω + \dif β$.
\item $\dif (fω) = ω \dif f + f \dif ω$.
\item $\dif (ω \y β) = \dif ω \y β + (-1)^k ω \y \dif β$ siendo $ω$ una k-forma.
\item $\dif(\dif ω) = 0$.
\end{itemize}
\subsubsection{Relación con operaciones en funciones vectoriales}
Partiendo de un campo en $\real^3$, podemos interpretarlo como una 1-forma o como una 2-forma.
\begin{itemize}
\item La diferencial exterior de un campo interpretado como 1-forma es la 2-forma asociada a la \textbf{divergencia}.
\item La diferencial exterior de un campo interpretado como 2-forma es la 3-forma asociada al \textbf{rotacional}.
\item El producto exterior de 2 campos interpretados como 2-formas nos da el campo asociado al \textbf{producto vectorial}.
\item ¿Cómo tengo que interpretar los campos para conseguir un producto escalar?
\end{itemize}
\subsubsection{Pull-back}
Queremos saber cómo llevar k-formas de $\real^N$ a $\real^M$. Partimos de la base de que existe una transformación $\appl{T}{ℝ^N}{ℝ^M}$ tal que $T(s)=x$, y buscamos otra aplicación $\appl{\pb}{\real^M}{\real^N}$.
En caso de 0-formas, el \emph{pull-back} es lo mismo que la composición. Es decir, dada una función $\appl{f}{ℝ^M}{ℝ}$, $\pb f = f \circ T$.
Basándonos en esta misma idea sobre las funciones escalares, vamos a tratar de hallar el pullback para las formas diferenciales. Supongamos que tenemos una k-forma $\omega$ en $\real^M$. Queremos construir $T^{\ast}$ en términos de $T$ y $\omega$. Partimos de  $\gor{s} \in \real^N$ (el punto donde se evalúa la k-forma), y $\gv_1,\gv_2,..,\gv_k$ los vectores en $\real^N$ sobre los que actúa $ω$. Entonces
\[
(T^{\ast}\omega)(\gor{s}) [\gv_1,\dotsc,\gv_k] = \omega(\underbrace{T(s)}_{\in\real^M}) [\underbrace{DT(s)\gv_j}_{\in\real^M}]
\]
Es decir, transformamos el punto en el que se evalúa $ω$, que pasa a ser $T(\gor{s})$ en lugar de $\gor{s}$, y los vectores sobre los que actúa también los "movemos" usando la matriz diferencial.
Vemos que
\[\omega(T(s)) [DT(s)\gv]\equiv \sum f_i(T(s))\dif x_i[DT(s)\gv]\]
\[DT(s) = \begin{pmatrix}
\dpa{T_1}{s_1}(s) & ... & \dpa{T_1}{s_N}\\
\vdots & \ddots & \vdots \\
\dpa{T_M}{s_1} & \dots & \dpa{T_M}{s_N}
\end{pmatrix} \cdot \begin{pmatrix}
v_1\\
\downarrow\\
v_N
\end{pmatrix}\]
¿Que significa $\dif x_i[DT(s)\gv]$? Vamos a ver que pasa con el producto de una de las filas de la matriz.
\[\df{x_i} [DT(s)\gv] = \dpa{T_i}{s_1}v_1 + ... + \dpa{T_i}{s_N}v_n\]
Podemos darnos cuenta de que $v_1 = \dif s_1[\gv]$. Con esto tenemos:
\[\df{x_i} [DT(s)\gv] = \left(\dpa{T_i}{s_1}\dif s_1 + ... + \dpa{T_i}{s_N}\dif s_N \right)[\gv] = \dif T_i [\gv] \]
y por lo tanto
\[ (\pb ω)(\gor{s})[\sample[\gor{v}][k]] =  \omega(T(s)) [DT(s)\gv] = \sum f_i (T(s))  \dif T_i [\gv] \]
\paragraph{Ejemplos}
\subparagraph{Ej. 1)} Sea  $f(x)\dif x_i$ una 1-forma de la que queremos calcular el \emph{pull-back}
\[T^{\ast}(f\dif x_i)(s)[v] = f(T(s)) \dif x_1[DT(s)\gv]\]
Supongamos $f\equiv 1$
\[T^{\ast}(fdx_i)(s)[v] = \dif x_1[DT(s)\gv] = \dif T_i[\gv]\]
\textbf{Conclusión: } $T^{\ast}\dif x_i = \dif T_i$.
\subparagraph{Ej. 2)} Sea $\omega = \sum_i f_i \dif x_i$ una 1-forma de la que queremos calcular el \emph{pull-back}
\[
 (T^{\ast} \omega )(s)[\gv]= \sum_i f_i(T(s))\dif x_i [DT(s)\gv] = \sum_i f_i(T(s)) \dif T_i [\gv ] = T^{\ast} (\sum_i f_i \dif x_i ) = \sum_i f_i \circ T \dif T_i
\]
\textbf{Conclusión: } $T^{\ast} (\sum_i f_i\dif x_i) = \sum_i (f_i \circ T) \dif T_i$
\subparagraph{Ej. 3: Pullback del producto exterior} ¿Cómo se comporta con el producto exterior? Vamos a trabajar con $f\equiv 1$.
\begin{gather*}
T^{\ast}(\df{x_i,x_j} [\gu,\gv] = \df{x_i,x_j} \left[DT(s)[\gu], DT(s)[\gv]\right] = \\
= \left|\begin{matrix}
\dif x_i[DT(s)\gu] & \dif x_j[DT(s)\gu] \\
\dif x_i[DT(s)\gv] & \dif x_j[DT(s)\gv]
\end{matrix}\right|
= \left| \begin{matrix}
\dif T_i[\gu] & \dif T_j[\gu]\\
\dif T_i[\gv] & \dif T_j[\gv]
\end{matrix}\right|
\stackrel{(1)}{=} \df{T_i,T_j} [\gu,\gv]
\end{gather*}
(1): Por las propiedades del producto exterior de 1-formas.
\textbf{Conclusión: } $T^{\ast} (dx_i \y dx_j) = dT_i \y dT_j$.
\subparagraph{Ej. 4)} ¿Qué pasa cuando tenemos el producto de 2-formas generadas?
\[\omega = \sum f_idx_i\,;\,\beta=\sum g_jdx_j\]
Vamos con el producto exterior.
\begin{gather*}
T^{\ast} (\omega \y \beta) (s) [\gu,\gv] = \sum_{i,j} f_i(T(s))g_j(T(s)) \underbrace{\df{x_i,x_j} [DT(s)\gu, DT(s),\gv]}_{\text{Calculado justo arriba}}\\
= \sum_{i,j} (f_i\circ T) = \dotsb \\
= \left(\sum (f_i\circ T)\dif T_i\right)\y\left(\sum(g_j \circ T) \dif T_j\right) = T^{\ast}\omega \y T^{\ast}\beta
\end{gather*}
\textbf{Conclusión: } $T^{\ast}(\omega \y \beta) = T^{\ast}\omega \y T^{\ast}\beta$.
Esto es válido para multiíndices $I$, es decir, para $\omega$ k-forma y $\beta$ s-forma.
\paragraph{Pull-back y diferencial exterior}
Una vez visto cómo se comporta el \emph{pull-back} respecto del producto exterior vamos a ver como se comporta con respecto de la diferencial exterior.
\begin{gather*}
\dif (T^{\ast} \omega) = \dif \left(\sum_i f_i(T(s)) \dif x_i [DT(s)\gv]\right) = \dif\left(\sum (f_i \circ T)(s) \dif T_i[\gv]\right)\\
= \sum_i \dif(f_i\circ T)\y dT_i
\end{gather*}
Vamos a ver qué significa $\dif(f_i\circ T)$:
\begin{gather*}
\dif (f_i\circ T) =  \sum_k \dpa{f_i\circ T}{s_k} \dif s_k \\
\dpa{f_i\circ T}{s_k} = \sum_j \dpa{f_i}{x_j}(T(s))\cdot \dpa{x_j}{s_k}
\end{gather*}
Donde $x_j = T_j(s)$. Juntando todo tenemos:
\[
\dif (T^{\ast} \omega) = \sum_{i,j,k} \dpa{f_i}{x_j}(T(s)) \dpa{T_j(s)}{s_k} \df{s_k,T_i} = \sum_{i,j} \dpa{f_i}{s_j}(T(s)) \df{T_j,T_i} = T^{\ast}(d(\sum f_i \dif x_i))
\]
\textbf{Conclusión: } $\dif (T^{\ast}\omega) = T^{\ast}(\dif \omega)$
\paragraph{Ejemplo concreto: Cambio a coordenadas polares} El cambio a coordenadas polares $(\rho,\theta)$ se define por la siguiente transformación:
\[T(\rho,\theta) =\left( T_1(\rho,\theta),T_2(\rho,\theta)\right) = (\rho \cos\theta,\rho \sen\theta)\]
 Vamos a calcular los pull-backs:
\begin{gather*}
 T^{\ast}(\dif x) = \dif T_1 = \dpa{T_1}{ρ}\dif ρ + \dpa{T_1}{θ}\dif θ = \cos θ \dif ρ - ρ \sen θ \dif θ \\
 T^{\ast}(\dif y) = \dif T_2 = \dpa{T_2}{ρ}\dif ρ + \dpa{T_2}{θ}\dif θ = \sen θ \dif ρ + ρ \cos θ \dif θ
\end{gather*}
 Juntando ahora lo que tenemos:
\begin{align*}
\pb(\df{x,y}) &= (\pb \dif x) \y (\pb \dif y) = \\
	&= (\cos θ \dif ρ - ρ \sen θ \dif θ) \y (\sen θ \dif ρ + ρ \cos θ \dif θ) = \\
	&= ρ \cos^2 θ \df{ρ,θ} - ρ \sen^2 θ \df{θ,ρ} = \\
	&= \left(ρ \cos^2 θ + ρ \sen^2 θ\right) \df{ρ,θ} = \\
	&= ρ \df{ρ,θ}
\end{align*}
\paragraph{Propiedades fundamentales de la operación}
\index{Pullback!propiedades}
\begin{enumerate}
\item $T^\ast f = f\circ T$, siendo $f$ una 0-forma.
\item $T^\ast(dω) = d(T^\ast ω)$. En particular $T^\ast (dx_I) = dT_I$.
\item $T^\ast(ω\y β)=(T^\ast ω) \y (T^\ast β)$.
\item $T^\ast(fω) = (f\circ T)(T^\ast ω) = (T^\ast f)(T^\ast ω)$
\item $T^\ast(ω+β)=T^\ast+T^\ast β$.
\item $(T\circ S)^\ast ω = S^\ast(T^\ast ω)$.
\end{enumerate}
\begin{example} Tenemos una aplicación $φ(s,t) = (φ_1(s,t), φ_2(s,t))$. Calculamos su pullback y entonces
\[ φ^\ast(\dif x) = \dif φ_1 = \dpa{φ_1}{s}\dif s + \dpa{φ_1}{t}\dif t \]
y de la misma forma
\[ φ^\ast(\dif y) = \dif φ_2 = \dpa{φ_2}{s}\dif s + \dpa{φ_2}{t}\dif t \]
\begin{gather*}
 φ^\ast(dx\y dy) = dφ_1\y dφ_2 =\left( \dpa{φ_1}{s}ds + \dpa{φ_1}{t}dt \right) \y\left( \dpa{φ_2}{s}ds + \dpa{φ_2}{t}dt \right) = \\
 0 + \dpa{φ_1}{s}\dpa{φ_2}{t}ds\y dt + \dpa{φ_1}{t}\dpa{φ_2}{s} dt\y ds + 0
\end{gather*}
 Los diferenciales están cambiados de orden así que seguimos pagando con un cambio de signo:
\[ \left(\dpa{φ_1}{s}\dpa{φ_2}{t} - \dpa{φ_1}{t}\dpa{φ_2}{s}\right)ds\y dt= \left|\begin{matrix}
\dpa{φ_1}{s} & \dpa{φ_1}{t} \\
\dpa{φ_2}{s} & \dpa{φ_2}{t}
\end{matrix}\right| =  \det \left(\dpa{φ}{s,t}\right) ds\y dt \]
\end{example}
\begin{example}
 Tenemos $β$, la 2-forma asociada a un campo $\vf=(F_1, F_2, F_3)$:
\[ β = F_1\df{y,z} + F_2\df{z,x} + F_3 \df{x,y} \]
 Queremos calcular su pullback mediante una aplicación $\appl{Φ}{ℝ^2}{ℝ^3}$. Entonces
\[ Φ^\ast β = g(s,t) \df{s,t} \]
 ¿Quién es $g$? Calculamos el pullback:
\[ φ^\ast β = F_1\circ Φ\df{Φ_2,Φ_3} + F_2\circ Φ\df{Φ_3,Φ_2} + F_3\circ Φ\df{Φ_1,Φ_2} \]
Se tiene que
\[ =\pesc{\vf\circ Φ, \left(\dpa{Φ_1}{s}, \dpa{Φ_2}{s}, \dpa{Φ_3}{s}\right) × \left(\dpa{Φ_1}{t}, \dpa{Φ_2}{t}, \dpa{Φ_3}{t}\right)} \df{s,t} \]
 Sin embargo, el producto vectorial de esos dos vectores parece el producto vectorial de $T_s × T_x$, el factor que teníamos que poner para integrar un campo en una superficie. Poderosa magia hombre blanco.
\end{example}
\begin{example} Tenemos una 1-forma asociada a $\vf$:
\[ ω = \sum_i F_i\dif x_i \]
 y una aplicación (curva) $\appl{σ}{ℝ}{ℝ^n}$. Entonces $σ^\ast ω$ es de la forma $g(t)\dif t$.
 Entonces
\begin{gather*} (σ^\ast ω)(t)[λ] = \sum_i F_i(σ(t)) \dif x_i[Dσ(t)λ] = \sum_i F_i(σ(t)) \dif x_i[σ_1'(t)λ, \dotsc, σ_N'(t)λ = \\
 = \sum_i F_i(σ(t)) σ_i'(t) \dif t[λ] = \\
 = \pesc{\vf \circ σ, σ'} \dif t [λ]
\end{gather*}
 Que, oh, sorpresa de nuevo, es lo que aparece cuando integrábamos un campo sobre una curva.
\end{example}
 Al final, querremos integrar k-formas en $ℝ^N$ sobre variedades de dimensión $k$.
\section{Integración de formas diferenciales}
Vamos a partir de un conjunto Ω abierto de $\real^N$.
Sea ω una n-forma definida en un entorno de Ω, es decir $\omega = f(\gx) \underbrace{\dfl{x_1}{x_n}}_{\text{Elemento de volumen}}$. Definimos la integral como sigue:
\begin{defn}[Integral\IS de n-formas en $\real^N$.]
\[
\int_Ω\omega = \int f(\gx) \id x_1 \dotsc \id x_N
\]
\end{defn}
Supongamos que tenemos una $\appl{\Phi}{\real^K}{\real^N}$, tal que $\Phi(\gor{s}) = \gx$. Para que lo de la derecha sea una variedad tenemos que $\Phi$ tiene que ser regular, homeomorfismo y rango máximo.
Supongamos $\omega \in \real^N$, con $\omega$ una x-forma.
¿Qué pasaría si queremos integrar $T^{\ast}\omega$?
Si queremos integrar $\pb{\omega}$ en $\real^k, \omega$ tiene que ser una k-forma para poder aplicar la definición.
\begin{example}
Variedad 1-dimensional.
$\appl{\sigma}{\real}{\real^3}$
Sea $\omega = f_1(x,y,z)\dif x + f_2(x,y,z)\dif y + f_3(x,y,z)\dif z$ la forma diferencial asociada al campo $\vf$.
Tenemos que $\sigma^{\ast}\omega = \pesc{\overrightarrow{F}\circ \sigma,\sigma'}\dif t$
La integral quedaría:
\begin{equation}
\int_{\sigma(I)} ω = \int_I  \pesc{\overrightarrow{F}\circ \sigma,\sigma'}\dif t \label{eqIntFDifCurva}
\end{equation}
Integrar 1-forma sobre la variedad 1-dimensional es integrar el trabajo del campo $\overrightarrow{F}$ a lo largo de $\sigma(I)$.
\end{example}
\begin{example}
Una variedad de dimensión 2 en $\real^3$.
$\appl{\Phi}{\real^2}{\real^3}$, con $\Phi(s,t) =  (x,y,z)$.
Sea $\beta$ 2-forma asociada al campo $\vec{G}$.
\[\beta = G_1(x,y,z) \df{y,z} + G_2(x,y,z) \df{z,x} + G_3(x,y,z) \df{x,y}\]
El pullback (calculado anteriormente es)
\[\Phi^{\ast}\beta = \pesc{\overrightarrow{G}\circ\Phi,\Phi_s\x\Phi_t}\df{s,t}\]
La integral sería:
\begin{equation}
\int_{\Phi(D)} ß = \iint\limits_D \pesc{\overrightarrow{G}\circ\Phi,\Phi_s\x\Phi_t}\id{s,t} \label{eqIntFDifSup}
\end{equation}
Es decir, integrar una 2-forma sobre $\Phi(D)$ es integrar el \textbf{flujo} del campo $\overrightarrow{G}$ a través de $\Phi(D)$
\end{example}
\subsection{Integración de formas diferenciales sobre variedades genéricas}
Después de haber visto los casos específicos, vamos a ver cómo integrar, de forma genérica, una forma diferencial sobre una variedad diferencial.
Sea $M$ una variedad de dimensión k en $\real^N$. Supongamos que $(D,\Phi)$ es una carta local, es decir:
$\appl{\Phi}{D\subset\real^K}{\real^N}, \Phi(D)\subset M$, siendo Φ una parametrización ($\Phi(\gor{t}) = \gx$).
Sea ω una k-forma definida en $ℝ^N$:
\[\omega = \sum_I f_I\dif x_I; \quad I=\{i_1,i_2,...,i_k\}\]
Por definición:
\begin{equation}
\int_{\Phi(D)} \omega = \int_D \Phi^{\ast}\omega \label{eqIntFDifVar}
\end{equation}
El pull-back nos va a dar una k-forma definida en $\real^k$.
\[
\Phi^{\ast}\omega =g(\gor{t})\dfl{t_1}{t_k}
\]
Aplicando esto:
\[
\int_{\Phi(d) \omega} = \int_D g(\gor{t})\dfl{t_1}{t_k}
\]
Vamos a identificar la función $g$ remangándonos y haciendo cuentas:
\[
\Phi^{\ast} \omega = \sum_I f_I\circ\Phi \dif \Phi_I =
\]
Vamos a fijarnos en $\dif \Phi_I = \df{\Phi_{i_1},...,\Phi_{i_k}}$, que va a actuar sobre k-vectores, es decir:
\[
\dif \Phi_I[\gv_1,...,\gv_k] = \dfl{\Phi_{i_1}}{\Phi_{i_k}} [\gv_1,\dotsc,\gv_k]
= \det \begin{pmatrix}
\dif \Phi_{i_1}[\gv_1] 	& \cdots & \dif \Phi_{i_1}[\gv_k] \\
\vdots 					& \ddots & \vdots\\
\dif \Phi_{i_k}[\gv_1] 	& \cdots & \dif \Phi_{i_k}[\gv_k] \\
\end{pmatrix}
\]
Vamos a desarrollar uno de los elementos de la matriz (escribiendo $\gw$ para generalizar a cualquiera de los vectores sobre los que actúa):
\[
\dif \Phi_{i_1}[\gw] = \sum_{j=1}^k \left(\dpa{\Phi_{i_1}}{t_j} \dif t_j\right)[\gw] = \sum_{j=1}^k \dpa{\Phi_{i_1}}{t_j}w_j = \pesc{\grad \Phi_{i_1},\gw}
\]
Aplicando esto:
\begin{gather*}
\dif \Phi_I[\gv_1,...,\gv_k] =
\det \begin{pmatrix}
\pesc{\grad \Phi_{i_1},\gv_1} 	& \cdots & \pesc{\grad \Phi_{i_1},\gv_k}\\
\vdots 							& \ddots & \vdots\\
\pesc{\grad \Phi_{i_k},\gv_1} 	& \cdots & \pesc{\grad \Phi_{i_k},\gv_k} \\
\end{pmatrix} =
\det \left(\begin{pmatrix}
\grad \Phi_{i_1} \rightarrow \\
\cdots \\
\grad \Phi_{i_k} \rightarrow
\end{pmatrix}
\cdot
\begin{pmatrix}
\gv_1 		& \cdots & \gv_k\\
\downarrow 	& \cdots & \downarrow
\end{pmatrix}\right) = \\
= \det\begin{pmatrix}
\grad \Phi_{i_1} \longrightarrow \\
\cdots \\
\grad \Phi_{i_k} \longrightarrow
\end{pmatrix}
\cdot
\det \begin{pmatrix}
\gv_1 		& \cdots & \gv_k \\
\downarrow 	& \cdots & \downarrow
\end{pmatrix} \stackrel{(1)}{=}
\det\begin{pmatrix}
\grad \Phi_{i_1} \longrightarrow \\
\cdots \\
\grad \Phi_{i_k} \longrightarrow
\end{pmatrix} \dfl{t_1}{t_k}[\gv_1,\dotsc,\gv_k]
\end{gather*}
(1): Aplicamos que $\dif t_1(\gv)$ es la primera coordenada del vector $\gv$. Un paso intermedio es \[\det \begin{pmatrix}
\dif t_1(\gv_1) & \cdots & \dif t_1(\gv_k)\\
\vdots 			& \ddots & \vdots\\
\dif t_k(\gv_1) & \cdots & \dif t_k(\gv_k)
\end{pmatrix} \]
\textbf{Conclusión:}
\[
\Phi^{\ast} \omega = \sum_I f_I\circ\Phi \dif \Phi_I =
\overbrace{\sum_I f_i\circ\Phi
\det\begin{pmatrix}
\grad \Phi_{i_1} \longrightarrow \\
\cdots \\
\grad \Phi_{i_k} \longrightarrow
\end{pmatrix}}^{\text{Esta es la g que buscamos}} \dfl{t_1}{t_k}
\]
Aplicando a una integral:
\begin{equation}
\int_{\Phi(D)} \omega = \int_D \sum_I f_i\circ\Phi
\det \begin{pmatrix}
\grad \Phi_{i_1} \longrightarrow \\
\cdots\\
\grad \Phi_{i_k} \longrightarrow
\end{pmatrix}\id{t_1,\dotsb,t_k}
\label{eqPbIntFDif}
\end{equation}
Donde la matriz enorme sería el equivalente al cambio en la medida cuando hacíamos un cambio de coordenadas.
\section{Teoremas de Green, divergencia y Stokes en términos de formas diferenciales}
Para entender los teoremas de Green, de divergencia (o Gauss) y Stokes en términos de las formas diferenciales, vamos a empezar con el caso básico: el cubo unidad.
En $ℝ^2$, el cubo unidad es $\mathcal{Q} = [0,1]\x[0,1]$. Para calcular la integral sobre la frontera, tenemos que integrar sobre cada una de las aristas:
\[\begin{array}{cc}
I_{11} =\{(1,y),y\in[0,1]\}&\text{ Orientación: }\, +\\
I_{21} =\{(x,1),x\in[0,1]\}&\text{ Orientación: }\, -\\
I_{10} =\{(0,y),y\in[0,1]\}&\text{ Orientación: }\, -\\
I_{20} =\{(x,0),x\in[0,1]\}&\text{ Orientación: }\, +\\
\end{array}
\]
Para nombrar las aristas usamos la notación $I_{ij}$, donde $i$ es la variable fija ($1=x$,$2=y$) y $j$ el valor que toma la variable fija.
La orientación está calculada con la regla de la mano izquierda. Me coloco en la frontera mirando hacia la dirección en la que nos movemos. Si la mano izquierda estirada apunta hacia el interior, la orientación es positiva. Si apunta hacia fuera, la orientación es negativa.
Sea $\omega = f(x,y)\dif x + g(x,y)\dif y$ la forma diferencial que queremos integrar, cuyo diferencial es
\[\dif \omega= \dpa{f}{y}\df{y,x} + \dpa{g}{x}\df{x,y} = \left(\dpa{g}{x} - \dpa{f}{y}\right) \df{x,y}\]
Consideramos $\mathcal{C}^+$ como la frontera de $\mathcal{Q}$ orientada positivamente. Vamos a intentar calcular la integral de ω sobre esa frontera.
\begin{align*}
\int_{C^+} \omega &= \int_{I_11}\omega\, - \int_{I_20}\omega\, - \int_{I_21}\omega\, + \int_{I_10}\omega = \\
	&= \int_0^1 g(1,y)\dif y + \int_0^1 f(x,0)\dif x - \int_0^1f(x,1)\dif x - \int_0^1 g(0,y)\dif y = \\
	&= \int_0^1 \left(g(1,y)-g(0,y)\right) \dif y - \int_0^1 \left( f(x,1)-f(x,0)\right) \dif x = \\
	&= \int_0^1\int_0^1 \dpa{g}{x}(x,y)\id{x,y} - \int_0^1\int_0^1 \dpa{f}{x}(x,y)\id{y,x} = \\
	&= \iint\limits_Q\left( \dpa{g}{x} - \dpa{f}{y}\right)\id{x,y} = \\
	&= \iint\limits_Q \dif \omega
\end{align*}
Operando, hemos llegado a que
\[ \int_{C^{+}} \omega = \iint\limits_Q \dif \omega \]
Esto escrito en términos de cálculo II es: \[ \int_{C^{+}}(P,Q) = \iint\limits_Q \dpa{Q}{x} - \dpa{P}{y} \], que es el \textbf{teorema de Green}.\index{Teorema!de Green}
Ahora vamos a hacer algo lo mismo en $\real^3$, sea $Q=[0,1]\x[0,1]\x[0,1]$, trabajando con la normal exterior para las orientaciones. Vamos a distinguir las caras con la notación anterior:
\[\begin{array}{cc}
I_{10} = \{(0,y,z), y\in[0,1],z\in[0,1]\} & \text{ Orientación: -} \\
I_{11} = \{(1,y,z), y\in[0,1],z\in[0,1]\} & \text{ Orientación: +} \\
I_{20} = \{(x,0,z), x\in[0,1],z\in[0,1]\} & \text{ Orientación: +} \\
I_{21} = \{(x,1,z), x\in[0,1],z\in[0,1]\} & \text{ Orientación: -} \\
I_{30} = \{(x,y,0), x\in[0,1],y\in[0,1]\} & \text{ Orientación: -} \\
I_{31} = \{(x,y,1), x\in[0,1],y\in[0,1]\} & \text{ Orientación: +} \\
\end{array}
\]
Las orientaciones están calculadas (según el primer caso) \[\left.\begin{array}{cc}
T_y = (0,1,0)\\T_z=(0,0,1)\end{array}\right\}\implies T_y\x T_z = (1,0,0)\] Mirando en el dibujo, identificamos que la cara en la que estamos trabajando (en este caso la de detrás) y comprobamos que apunta hacia dentro del cubo (dirección contraria a la normal exterior), y concluimos orientación negativa.
Repitiendo el proceso llegamos a la conclusión de: \[
\begin{array}{cc}
T_y\x T_z &= (0,0,1)\\
T_x\x T_z &= (0,-1,0)\\
T_x\x T_y &= (1,0,0)
\end{array}\]
Si la suma de los subíndices es par, la orientación es positiva. Si por el contrario es impar, es negativa. Detrás de esta idea hay un teorema que no vamos a ver. Además hay que tener cuidado con el orden en el que se hacen las cosas y se escriben los vectores.
Trabajamos con nuestra forma diferencial asociada a un campo $\vf$:
\[\omega = F_1(x,y,z)\df{y,z}+F_2(x,y,z)\df{y,x}+F_3(x,y,z)\df{x,y}\]
cuyo diferencial es
\begin{align*}
\dif \omega &= \dpa{F_1}{x}\df{x,y,z} + \dpa{F_2}{y}\df{y,x,z} + \dpa{F_3}{z}\df{z,x,y} \\
	&= \left(\dpa{F_1}{x}+\dpa{F_2}{y} + \dpa{F_3}{z}\right) \df{x,y,z}
\end{align*}
Vamos a calcular \[\int_{dQ^+} \omega\] siendo $dQ^+$ la frontera del cubo unidad.
\[\int_{Q^+} \omega =\underbrace{ -\int_{I_{10}} \omega +  \int_{I_{11}} \omega}_{(1)} + \int_{I_{20}} \omega -  \int_{I_{21}} \omega  -\int_{I_{30}} \omega +  \int_{I_{31}} \omega\]
Operamos (1) por separado. Aplicando (\ref{eqIntFDifVar}) y la ecuación de la integral de una forma diferencial sobre una superficie (\ref{eqIntFDifSup}) tenemos que
\begin{gather*}
 -\int_{I_{10}} \omega +  \int_{I_{11}} \omega = \int_0^1\int_0^1\Phi^{\ast}_{11}\omega - \int_0^1\int_0^1 \Phi^{\ast}_{10} \omega = \\
 = \int_0^1\int_0^1 \pesc{\overrightarrow{F}\circ \Phi_{11},(1,0,0)}\id{y,z}
 -\int_0^1\int_0^1 \pesc{\overrightarrow{F}\circ \Phi_{10},(1,0,0)}\id{y,z}= \\
= \int_0^1\int_0^1 F_1(\Phi_{11}(y,z))-F_1(\Phi_{10}(y,z))dydz = \iiint\limits_Q \dpa{F_1}{x}\id{x,y,z}
\end{gather*}
Aplicando las mismas cuentas con las que faltan llegamos al \textbf{teorema de la divergencia} para el cubo.
\paragraph{Conclusión}
\[\int_{dQ^+} \omega = \int_{Q}\dif \omega\]
Las ideas sobre formas diferenciales se traducen en $\real^2$ en el Teorema de Green y en $\real^3$ en el Teorema de la divergencia. ¿Dónde queda el Teorema de Stokes? Después de unos ejemplos de aplicación de los teoremas vamos a verlo.
\subsection{Aplicaciones de los teoremas de integración}
\subsubsection{Teorema de Green}
Sea $\omega$ 1-forma en $\real^2$, y $D$ un conjunto cerrado con frontera orientable. Entonces
\[
\int_{\partial  D^+} P\dif x+Q\dif y = \iint_D \dif(P\dif x+Q\dif y) = \int\int_D \dpa{Q}{x} - \dpa{Q}{y}\id{x,y}
\]
\obs Podemos elegir $(P,Q)$ de tal modo que $\displaystyle \dpa{Q}{x}-\dpa{Q}{y} = 1$.
Entonces el área de $D$ sería $\displaystyle\int_{\partial  D^+} (P,Q)d\sigma$. Podemos aplicar esta idea para hallar el área de la hoja folium de Descartes (imagen \ref{lblFolium}), cuya ecuación es
\[x^3+y^3 = mxy\]
\easyimgw{imgs/FoliumDescartes.png}{Folium de Descartes}{lblFolium}{0.3}
Vamos a parametrizarla, siguiendo la indicación: $t = \frac{y}{x}$. Se deja como ejercicio para el lector llegar a la fórmula:
\begin{gather*}
x=\frac{mt}{1+t^3}\\
y= xt = \frac{mt^2}{1+t^3}
\end{gather*}
Quedando por definir que valores toman los parámetros. En este caso es $(0,\infty)$. Estos valores parametrizan la región cerrada.
Podríamos plantearnos para qué valores de $t$ que recorren las ramas que se van a infinito. En $t=-1$, se va a infinito, entonces una de las ramas será $t\in(-1,0)$ y la otra será $t\in(-\infty,-1)$.
¿Que orientación nos da esta parametrización?
La idea es ver el vector tangente en el 0. Si es horizontal empezaremos por la rama de abajo. Si es vertical, empezaremos por la rama de arriba
\[\sigma'(t) = \left(\frac{m(1+t^3)-3mt^3}{(1+t^3)^2},\frac{2mt(1+t^3) - 3mt^4}{(1+t^3)^2}\right)\]
Podemos comprobar que $\sigma'(t) \convs[][t][0^+] (m,0)$. Además, $\sigma'(t) \convs[][t](0,m)$, quedando una orientación positiva.
\[
A(D) = \int_{\partial  D^+} (0,x)d\sigma = \int_0^{+\infty} \pesc{\left(0,\frac{mt}{1+t^3}\right), \left(\ast,\frac{2mt(1+t^3)-3mt^4}{(1+t^3)^2}\right)}dt = ...
\]
Wolfram dice que el resultado de la integral es $\frac{m^2}{6}$ y que el área encerrada por el folium de Descartes es también $\frac{m^2}{6}$ lo que nos hace pensar que está bien planteado y bien resuelto el problema.
\paragraph{Ejercicio para el lector} Hacer lo mismo con la curva $x^4+y^4=4xy$. El área de la hoja contenida en el primer cuadrante.
%\easyimgw{imgs/FoliumALaCuarta.png}{$x^4+y^4=4xy$}{lblFoliumALaCuarta}{0.3}
\subsubsection{Teorema de Stokes en $\real^3$}
El teorema decía: \[
\int_{\Gamma^+}\overrightarrow{F}d\sigma = \int \int_{S^+} \rot\overrightarrow{F} dS
\]
Siendo $S$ la superficie, $\Gamma$ la ¿frontera?, tomando la orientación positiva con la normal exterior.
\subparagraph{Ejemplo}
\[
\left.\begin{array}{cc}
z=x^2+y^2\\
z=mx \end{array} \right\} \equiv \Gamma
\]
Queremos calcular $\displaystyle \int_{\Gamma}y \dif z$
Esto es lo mismo que calcular la integral del campo $(0,0,y)$.
El primer paso es \textbf{parametrizar} $\Gamma$
Tenemos que la proyección en el plano xy es \[mx=x^2+y^2 \equiv \left(x-\frac{m}{2}\right)^2 + y^2 = \frac{m^2}{4}\]
Viendo los cuadrados lo lógico es pensar en utilizar polares.
Llamando $x=rsen(\theta),y=rsen(\theta)$ tenemos:
\[\sigma(\theta) = \left(mcos^2(\theta),mcos(\theta)sen(\theta),m^2cos^2(\theta)\right)\,\,\,\theta\in\left(\frac{-\pi}{2},\frac{\pi}{2}\right)\]
Calculamos el vector tangente para ver en que orientación recorre la curva esta parametrización:
\[\sigma'(\theta) = ()\]
\[\sigma'(0) = (0,m,0)\]
Suponemos (porque no me lo dicen, que $m>0$) y nos da la orientación. Como en el enunciado no nos hablan de hacerlo con ninguna orientación, la integral que calculemos será de acuerdo con esta orientación.
Vamos con la integral:
\[\int_{\Gamma}(0,0,y) d\sigma =\int_{\frac{-\pi}{2}}^{\frac{\pi}{2}}\pesc{\underbrace{\left(0,0,mcos(\theta)sen(\theta)\right)}_{\overrightarrow{F}(\sigma(\theta))},\ast} d\theta\]
Como camino alternativo a la fórmula, podemos aplicar el teorema:
\[ = \int\int_{D^+}  rot(0,0,y)dS\] Siendo el vector normal el que tenga la tercera componente positiva (razonando geométricamente).
Calculamos el rotacional del campo:$rot\overrightarrow{F} =\left|\begin{matrix}
i&j&k\\dx&dy&dz\\0&0&y
\end{matrix}\right| = (1,0,0)$.
Utilizamos la parametrización: $S = (x,y,mx), x,y\in C$
\[ = \int\int_D^+ rot(0,0,y)dS = \int \int_C \pesc{(1,0,0) ,T_x\x T_y} dxdy= (1) =\]
\[ \int \int_C \pesc{(1,0,0),(-m,0,1)} = \int\int -m dxdy = -m \cdot \, Area (C) = -m\frac{m^2}{4}\pi \]
$(1): T_x = (1,0,m); T_y = (0,1,0) $. Otra cosa aplicada es que el vector normal $(-m,0,1)$ como la tercera componente es positiva, tenemos que esta parametrización induce la orientación positiva.
\section{Teorema de Stokes}
Partimos, igual que en la sección anterior, del cubo unidad en $ℝ^n$. Contamos además con la aplicación $\appl{\Phi}{Q}{\Phi(Q)\subset\real^n}$ que "deforma" ese cubo.
\begin{figure}[hbtp]
\centering
\input{tikz/TeoremaStokes-ApplPhi.tex}
\caption{Esquema para la aplicación de Stokes en un cubo unidad}
\end{figure}
 Sea $\omega$ una k-forma en $\real^n$. Queremos calcular la integral de su diferencial en $Φ(Q)$.
\[
\int_{\Phi(Q)} \dif \omega = \int_Q \Phi^{\ast}\dif\omega = \int_Q \dif(\Phi^{\ast}\omega) = \int_{∂Q^{+}} \Phi^{\ast}\omega
\]
Donde $∂Q^{+}$ es la frontera del cubo $Q$ orientada debidamente. El último paso es aplicar el teorema anterior.
Sea $\appl{\sigma}{I}{∂Q}$. Entonces, $\appl{\Phi\circ\sigma}{I}{\Gamma}$, siendo $\Gamma$ la frontera de $\Phi(Q)$.
Aplicando esto a la integral que estamos calculando:
\[
\int_{\Phi(dQ^{+})} \omega \equiv \int{\Phi\circ\sigma(I)} = \int_I (\Phi\circ\sigma)^{\ast} \omega = \int_I \sigma^{\ast}\left(\Phi^{\ast}(\omega)\right) = \int_{\sigma(I)} \Phi^{\ast}\omega = \int_{∂Q}\Phi^{\ast}\omega
\]
Hemos llegado finalmente a que \[ \int_{∂Q^+} \Phi^{\ast} \omega = \int_{\Phi(∂Q^+)} \omega \]
Ahora querríamos dar el siguiente paso:
\[\int_{\Phi(∂Q^+)} \omega = \int_{∂(\Phi^{\ast}(Q))} \omega \]
Es decir, que la imagen de la frontera sea la frontera de la imagen. Esto no es inmediato: en el cambio a coordenadas polares, por ejemplo, no se cumple a primera vista (ver figura \ref{imgCambioPolaresFrontera}). Cuando el ángulo (θ) se mantiene fijo y $r$ varía (segmentos azules), la imagen de esa parte de la frontera es un radio de la circunferencia, y cuando $r=0$ y variamos el ángulo (segmento verde) la imagen es un punto.
\begin{figure}[hbtp]
\centering
\input{tikz/TeoremaStokes-CambioPolares.tex}
\caption{La frontera no es la misma en el cambio a polares: las partes verde y azul forman parte de $∂Q$ pero no de $∂(Φ(Q))$.}
\label{imgCambioPolaresFrontera}
\end{figure}
Ahora bien, podemos dividir la región $Q$ en celdas disjuntas, como se puede ver en la figura \ref{imgPolaresDisjuntas}. De esta forma, las fronteras que sean comunes a varias celdas tendrán orientación incompatible y se anularán al integrar. Esto nos resuelve el problema y podemos enunciar el teorema de Stokes para celdas:
\begin{figure}[hbtp]
\centering
\input{tikz/TeoremaStokes-PolaresDisjuntas.tex}
\caption{Podemos dividir $Q$ en dos celdas disjuntas}
\label{imgPolaresDisjuntas}
\end{figure}
\begin{theorem}[Teorema\IS de Stokes (para celdas)]\label{thmStokesCeldas}
\[ \int_M \dif \omega = \int_{\partial  M^+}\omega \]
, si la variedad $M$ se puede descomponer como unión de celdas con interior disjunto.
\end{theorem}
\paragraph{Frontera de una superficie}
Vamos a intentar definir en serio la frontera de objetos en $\real^3$, que es algo que necesitamos tener realmente muy claro.
\easyimg{imgs/StokesCeldasTipo.png}{ψ nos lleva $P$ a un punto que no está en la frontera de la imagen por ψ de su celda correspondiente (llamada de tipo I). En el caso de $Q$, ψ lo lleva a un punto en la frontera de la imagen de su celda por ψ (de tipo II), por lo tanto sí es un punto de la frontera.}{imgTiposCelda}
Hace un tiempo, cuando definíamos una subvariedad, demostramos la existencia de un difeomorfismo Ψ que "aplanaba un trozo" de subvariedad. La frontera de una superficie es el conjunto de los puntos (llamados en clase de Tipo 2) que al aplanar nos quedan en la frontera de un objeto de dimensión 2 (ver imagen \ref{imgTiposCelda}).
\index{Frontera}
Una vez aclarado el concepto de frontera, pasamos a demostrar el teorema de Stokes.
\begin{theorem}[Teorema\IS de Stokes]
Sea $M$ una subvariedad compacta, orientable, con frontera relativa $\partial  M$.
Entonces
\[\int_{\partial  M^+}\omega = \int_M \dif \omega \]
\end{theorem}
\begin{proof} La demostración ya está vista para celdas en la sección anterior, así que vamos a extender la idea.
\subparagraph{Paso 1: Compacidad}
Para todo punto $P\in M$ existe una celda $C_p$ tal que $P \in C_p$. Por lo tanto, está claro que $M\subset \bigcup_{p\in M} C_p$. Tomamos el interior de las celdas, para trabajar con conjuntos abiertos.
Hemos recubierto con infinitos abiertos la subvariedad, así que por compacidad (\ref{thmCerradoAcotado}) existe un subrecubrimiento \textbf{finito}.
Sin embargo, no podemos garantizar que las celdas son disjuntas. Si lo fueran, aplicaríamos el teorema a cada celda y listo. Hay que ver qué ocurre cuando las celdas no son disjuntas.
\subparagraph{Paso 2: Particiones de la unidad}
Vamos a intentar resolver el problema de los solapamientos. Buscamos una función que valga cero fuera de la celda que consideramos y sea mayor que cero dentro de ella, algo como pueda ser la figura \ref{imgStokesPhi}.
\begin{wrapfigure}{r}{0.6\textwidth}
\begin{center}
\includegraphics[width=0.58\textwidth]{imgs/TeoremaStokes-PartUnidad.png}
\end{center}
\caption{La función Φ que buscamos sería algo así.}
\label{imgStokesPhi}
\end{wrapfigure}
Sea $\appl{\Phi}{\real^N}{\real}$. Además,
\begin{itemize}
\item $\Phi>0$ en $\mathcal{Q}$
\item $\Phi = 0$ en $\partial  \mathcal{Q}$
\item $\Phi = 0$ en $\real^N-\mathcal{Q}$
\item $\Phi\in C^1$.
\end{itemize}
Consideramos $\Phi_i = \Phi\circ\Psi_{p_i}$, siendo $\Psi_{p_i}$ el difeomorfismo que cubre la celda $p_i$, con $i=1,...,k$ y la lleva al cubo unidad ($\mathcal{Q}$).
Además, nos gustaría que la suma de todas las aplicaciones $Φ_i$ sobre un punto sea 1:
\[ \sum_i \Phi_{i}(\gx) = 1\;\forall \gx \in M\]
Aunque parece una cosa imposible, vamos a ver que es algo perfectamente factible:
\[\tilde{\Phi}(\gx) = \frac{\Phi_i (\gx)}{\sum_{i=1}{k}\Phi_i(\gx)}\]
Estas $\tilde{\Phi}_i$ satisfacen todas las propiedades que nos interesan.
\subparagraph{Paso 3: Descomposición del problema}
Lo que nosotros queremos es calcular $\int_M d\omega$. Tal y como habíamos definido $\tilde{Φ}$ antes, es obvio que sobre la variedad $M$
\[ \omega=\sum_i^k\tilde{\Phi}_i(x)\omega \]
Entonces
\[\dif \omega = \sum_{i=1}^k \dif (\tilde{\Phi}_i,\omega) = \sum_{i=1}^k \left( \dif \tilde{\Phi}_i\y \omega + \tilde{\Phi}_i \dif \omega \right) =  \dif\left(\sum_i \tilde{\Phi}_i\right) \y \omega + \sum \tilde{\Phi}_i \dif \omega\]
Dado que $\sum_i \tilde{Φ}_i = 1$, $\dif\left(\sum_i \tilde{\Phi}_i\right) = 0$ y por lo tanto
\[ \dif \omega = \sum \tilde{\Phi}_i \dif \omega \]
Aplicando esto descomponemos:
\[\int_M \dif \omega = \sum_{i=1}^k \int_M \tilde{\Phi}_i \dif\omega = \sum_{i=1}^k \int_{C_{p_i}} \tilde{\Phi}_i \dif\omega=\sum_{i=1}^k \int_{C_{p_i}} \dif(\tilde{\Phi}_i\omega)
\]
Hemos conseguido definir la integral como una suma finita de integrales sobre celdas en las que sí podemos aplicar el teorema de Stokes (\ref{thmStokesCeldas})
Entonces tenemos:
\[\int_M \dif \omega = \sum_{i=1}^k \int_{\partial  C_{P_i}^{+}} \tilde{\Phi}_i\omega\]
Por como hemos definido $\tilde{\Phi}_i$ tenemos que todas las celdas de tipo 1 valen 0. En cambio en las celdas de tipo 2 (ver \ref{imgTiposCelda} para los tipos de celda), tenemos una parte sobre la que $\tilde{\Phi}_i \neq 0$ (ver figura \ref{imgStokesCeldasIntegral}).
Esto nos deja: \[\int_M d\omega = \sum_{i=1}^k \int_{\partial  C{P_i}^{+}} \tilde{\Phi}_i\omega = \sum \int_{\partial M^+} \tilde{\Phi}_i \omega = \int_{\partial M^+} \omega\]
\end{proof}
\begin{figure}[hbtp]
\begin{center}
\input{tikz/TeoremaStokes-CeldasIntegral.tex}
\end{center}
\caption{Sólo influyen a la integral los puntos de la frontera de la variedad, los que llevan a celdas de tipo II.}
\label{imgStokesCeldasIntegral}
\end{figure}
\begin{example}
Sea $M$ una superficie en $\real^3$, un trozo de $x^2+y^2+z^2 = 1$ dentro de $x^2+y^2\leq y$, con $z\geq 0$. Ver figura \ref{imgEsferaCono}. Consideramos la orientación positiva como la de la normal hacia abajo.
\easyimg{imgs/EsferaCilindro.png}{Intersección de la esfera y el cilindro. La línea azul es la frontera de $M$, y las flechas naranjas indican su orientación positiva.}{imgEsferaCono}
Calcular las tres integrales
\[ \int_{\partial M} x \id y;\;\int_{\partial M} y \id z;\; \int_{\partial M} z \id x \]
\textbf{Previos} Nos damos cuenta de que $x^2+y^2\leq y$ es una circunferencia. Si completamos cuadrados tenemos la siguiente ecuación: \[x^2+\left(y-\frac{1}{2}\right)^2 = \frac{1}{4}\]
Es decir, una circunferencia de radio $\frac{1}{2}$ centrada en $(0,\frac{1}{2})$.
\paragraph{Resolución de $\int_{\partial M} x \dif y$}
\[
\int_{\partial M^{+}} x\dif y =\int_{\partial M^{+}} (0,x,0) \dif\sigma \stackrel{\mathrm{Stokes} }{=} \iint\limits_M \rot (0,x,0) \dif S = \iint\limits_M (0,0,1) \dif S
\]
Para calcular esta integral (que es calcular el flujo) aplicamos la fórmula de siempre. Para ello necesitamos parametrizar la superficie $M$:
\begin{equation}\label{eqEjStokes}
\Phi(x,y) = (x,y,\sqrt{1-x^2+y^2}), (x,y)\in D = \{x^2+y^2\leq y\}
\end{equation}
Calculamos $T_x\x T_y =\displaystyle \left(\frac{x}{\sqrt{\cdot}},\frac{x}{\sqrt{\cdot}},1\right)$
\[
\int \int_M (0,0,1) dS = - \int \int_D \pesc{(0,0,1),(\ast,\ast,1)} \,dx\,dy = -\text{ Area } (D) = -\pi\frac{1}{4}
\]
\[ \int_{∂M^+}y\df{z} = \int_{∂M^+}(0,0,y)\df{σ} \stackrel{Stokes}{=} \int\int_{M^+} \rot (0,0,y)\df{S} \]
En \ref{eqEjStokes} teníamos la parametrización, así que la aplicamos. Teniendo en cuenta la orientación, tenemos que cambiar el signo y nos queda
\[
- \iint_D \pesc{(1,0,0),\left(\frac{x}{\sqrt{\ast}}, \frac{y}{\sqrt{\ast}}, 1}\right) \df{x}\df{y}
= -\iint_D\frac{x}{\sqrt{1-x^2-y^2}} \d{x,y} 
\]
Viendo que estamos integrando una función impar en una región simétrica, la integral vale 0.
\paragraph{Resolución de $\int_{\partial M} z \dif x$}
Pasamos ahora a calcular la integral de $z$. Tenemos lo mismo que antes:
\begin{gather*}
\int_{∂M^+}z\df{x} = \int_{∂M^+}(z,0,0)\df{σ} \stackrel{Stokes}{=} \iint_{M^+} \rot (z,0,0)\df{S} = \iint_{M^+}(0,1,0)\id{S}= \\
 - \iint_D \pesc{(0,1,0),\left(\frac{x}{\sqrt{\ast}}, \frac{y}{\sqrt{\ast}}, 1\right)}\id{x,y}
= -\iint_D\frac{y}{\sqrt{1-x^2-y^2}} \id{x,y}
\end{gather*}
Vemos que esta integral es muy complicada y nos va a ganar, así que pasamos a tratar de integrar como una curva. Deberemos parametrizar la curva, encontrar la orientación correcta y aplicar la fórmula.
Empezamos con la parametrización:
\[ ∂M = \left\{ \begin{matrix}
x^2+y^2+z^2 = 1 \implies y + z^2 = 1 \implies z = \sqrt{1-y} \\
x^2 + y^2 = y \implies x = \pm \sqrt{y-y^2}
\end{matrix}\right. \]
Por lo tanto, podemos parametrizar en dos trozos
\begin{align*}
Γ_1\equiv &(\sqrt{y-y^2}, y, \sqrt{1-y});\;y∈[0,1] \\
Γ_2\equiv &(-\sqrt{y-y^2}, y, \sqrt{1-y});\;y∈[0,1] \\
\end{align*}
\easyimgw{imgs/OrientacionesEsferaCilindro.png}{Orientaciones de $Γ_1$ y $Γ_2$}{imgOrientacionesEsferaCilindro}{0.7}
Tal y como vemos en la figura \ref{imgOrientacionesEsferaCilindro}, la orientación es negativa en $Γ_1$ y positiva en $Γ_2$. Entonces
\[ \int_{∂M^+}(z,0,0)\df{σ} = \int_{Γ_1^+}(z,0,0)\dif{σ_1} +  \int_{Γ_2^+}(z,0,0)\dif{σ_2} \]
Operando con la primera integral:
\[  \int_{Γ_1^+}(z,0,0)\dif{σ_1} = - \int_0^1\pesc{(\sqrt{1-y},0,0),\left(\frac{1-2y}{2\sqrt{y-y^2}},\ast,\ast\right)}\dif y =
-\int_0^1\frac{1-2y}{2\sqrt{y}}\dif y = \]
Separamos en dos sumandos
\[ = \int_0^1\sqrt{y}\d y - \int_0^1 \frac{1}{2\sqrt y}\dif y = \dotsb \]
Podríamos tomar otra parametrización alternativa usando coordenadas esféricas. La esfera queda determinada por la parametrización
\[ \left\{\begin{matrix}
x &=& \cos θ \sin φ \\
y &=& \sin θ \sin φ \\
z &=& \cos φ
\end{matrix}\right. \]
Añadiendo la restricción de $x^2+y^2=y$, nos queda que $\sin φ = \sin θ$. Entonces podemos seguir parametrizando
\[\left. \begin{matrix}
x = \cos θ \sin θ \\
y = \sin^2 θ \\
 z = \sqrt{1-\sin^2 θ} = \abs{\cos θ}
\end{matrix} \right\} θ∈[0,π]
\]
y tenemos que
\[ σ_1(θ) = (\cos θ \sin θ, \sin^2 θ, \cos θ) \]
Por otra parte, si pusiésemos los límites de integración en la región D pasaría algo.
\end{example}
\section{Campos conservativos}
\begin{defn}[Campo\IS conservativo] Consideramos $\vf$, un campo en $ℝ^N$. Se dice que $\vf$ es conservativo si y sólo si $∃\appl{V}{ℝ^N}{ℝ}$ tal que $F=\grad V$, donde $V$ es el \textbf{potencial}\index{Potencial} del campo $\vf$.
\end{defn}
\begin{theorem} Sea $\vf$ un campo $C^1$ en $ℝ^3$. Entonces $\vf $ es conservativo si y sólo si $\rot \vf = \vec{0}$.
\end{theorem} \label{consImpRot}
\begin{proof}
\paragraph{Implicación a la derecha} Como $F=\grad V$, y $F∈C^1$, entonces $V∈C^2$. Calculamos ahora el rotacional:
\[ \rot\vf = \left|\begin{matrix}
\vec{i} & \vec{j} & \vec{k} \\
\pd{}{x} & \pd{}{y} & \pd{}{z} \\
F_1 & F_2 & F_3
\end{matrix}\right| = \left(\dpa{F_3}{y}-\dpa{F_2}{z}, \dpa{F_1}{z}-\dpa{F_3}{x}, \dpa{F_2}{x}-\dpa{F_1}{y} \right) \]
Sustituyendo con $F=\grad V$ veríamos que sale todo cero.
\paragraph{Implicación hacia la izquierda}
Supongamos $Γ$ una curva cerrada, que sea la frontera de una superficie $M$. Entonces
\[ \int_{M^+}\vf  \stackrel{Stokes}{=} \iint_M\rot \vf\dif S = 0 \]
Es decir, que la integral de $F$ sobre cualquier curva cerrada va a dar 0. Buscamos ahora un $V$ tal que $\grad V = \vf$.
Supongamos un punto cualquiera $(x,y,z)$: A ese punto podemos llegar a través de varias rectas paralelas a los ejes. Con esas rectas podríamos construir un camino, y entonces tendríamos que
\todo[inline]{Poner dibujito aquí}
\[ \int_{Γ_1}\vf = \int_{Γ_2} \vf = \int_{Γ_3}\vf \]
ya que cogiendo dos pares $Γ_i$ y cambiando la orientación de uno de ellos construimos una curva cerrada.
Parametrizamos $Γ_1$:
\[ Γ_1 \equiv \{ (t,0,0)\,t∈[0,x]\}
\cup \{ (x,s,0)\,s∈[0,y]\}
\cup \{ (x,y,r)\,r∈[0,z]\} \]
Entonces
\begin{align*}
\int_{Γ_1}\vf&= \int_0^x\pesc{(F_1(t,0,0),F_2(t,0,0), F_3(t,0,0),(1,0,0)}\dif t \\
&+\int_0^y\pesc{(F_1(x,s,0),F_2(x,s,0), F_3(x,s,0),(0,1,0)}\dif s \\
&+\int_0^x\pesc{(F_1(x,y,r),F_2(x,y,r), F_3(x,y,r),(1,0,0)}\dif r \\
&=\int_0^x F_1(t,0,0)\dif t + \int_0^y F_2(x,s,0)\dif s+ \int_0^z F_3(x,y,r)\dif r 
\end{align*}
De la misma forma, tendríamos
\begin{gather*}
\int_{Γ_2}\vf = \int_0^y F_2(0,t,0)\dif t + \int_0^z F_3(0,y,s)\dif s+ \int_0^x F_1(x,y,r)\dif r \\ 
\int_{Γ_3}\vf = \int_0^x F_1(t,0,0)\dif t + \int_0^z F_3(x,0,s)\dif s+ \int_0^y F_1(x,r,z)\dif r \\
\end{gather*}
Las tres integrales son iguales, así que podemos derivar con respecto de la que nos venga mejor para construir la función $V$, que es la que buscábamos.
\end{proof}
La versión de este teorema vista en clase de prácticas (que es una versión más práctica)
\begin{theorem}[Campos conservativos]
$F$ es un campo vectorial $C^1$ en $\real^3$ excepto en un número finito de puntos entonces son equivalentes:
\begin{itemize}
\item Existe un potencial
\item La integral sobre una curva cerrada simple es 0
\item Las integrales por un camino o por otro para llegar a un punto son iguales
\item rot $\vf=0$.
\end{itemize}
\end{theorem}
Además, para calcular el potencial se puede utilizar cualquiera de estas 3 fórmulas:
\begin{gather*}
\int_{Γ_1}\vf=\int_0^x F_1(t,0,0)\dif t + \int_0^y F_2(x,s,0)\dif s+ \int_0^z F_3(x,y,r)\dif r \\
\int_{Γ_2}\vf = \int_0^y F_2(0,t,0)\dif t + \int_0^z F_3(0,y,s)\dif s+ \int_0^x F_1(x,y,r)\dif r \\ 
\int_{Γ_3}\vf = \int_0^x F_1(t,0,0)\dif t + \int_0^z F_3(x,0,s)\dif s+ \int_0^y F_1(x,r,z)\dif r \\
\end{gather*}
\subsection{Ejemplos}
\begin{example} Tenemos un cono de base $D$ y altura $h$, y buscamos integrar el campo $\vf(x,y,z)= (x,y,z)$. $Ω$ es el espacio del cono, y $∂Ω$, su superficie, se divide en la superficie lateral y la base.
\todo[inline]{Dibujito L1244}
Si escribimos el teorema de Gauss, tenemos que
\[ \iiint_Ω \dv \vf \id{x,y,z} = \iint_{∂Ω^+} \vf \dif S \]
En este caso, tenemos la suerte de que $\dv \vf = 3$, y por lo tanto
\[ \iiint_Ω \dv \vf \id{x,y,z} = 3 \cdot \mathrm{Volumen}\,(Ω) \]
Por lo tanto, para hallar el volumen calculamos la integral sobre la superficie y dividimos entre tres.
La idea geométrica es que en la cara lateral, la componente normal de $\vf$ es 0. Lo vemos fácilmente sabiendo que la recta definida por el vector $(x,y,z)$ y que pasa por el origen (el vértice del cono), tiene exactamente la misma dirección de la generatriz. Entones,\textbf{ la integral sobre la cara lateral es 0} y por lo tanto podemos ignorarla. Nos centramos sólo en la integral de la base:
\[ \iint_{\mathrm{Base}}\vf \id S \]
Parametrizar $S$ es sencillo:
\[ S \equiv \{ (x,y,h)\tq (x,y)∈ D \} \]
Calculamos su vector normal:
\[ \left.\begin{matrix}
T_x = (1,0,0) \\
T_y = (0,1,0)
\end{matrix}\right\} T_x × T_y = (0,0,1) \]
y entonces
\[ \iint_{\mathrm{Base}}\vf \id S = \iint_D\pesc{(x,y,h),(0,0,1)} \id{x,y} = \iint_D h \id{x,y} = h \cdot \mathrm{Area}\,(D) \]
Finalmente
\[ \mathrm{Volumen}\,(Ω) = \frac{h \cdot \mathrm{Area}\,(D)}{3} \]
\end{example}
\begin{example}[Cálculo del campo eléctrico o gravitatorio]
La expresión del campo eléctrico es
\[ \vf(\vx) = C \frac{\vx}{\norm{\vx}^3} \]
Calculando las derivadas parciales
\begin{align*}
\dpa{F_1}{x}&=\frac{y^2+z^2-2x^2}{(x^2+y^2+z^2)^{\frac{5}{2}}} \\
\dpa{F_2}{y}&=\frac{x^2+z^2-2y^2}{(x^2+y^2+z^2)^{\frac{5}{2}}} \\
\dpa{F_3}{z}&=\frac{x^2+y^2-2z^2}{(x^2+y^2+z^2)^{\frac{5}{2}}}
\end{align*}
nos queda que
\[ \dv\vf = 0 \]
Consideramos ahora una bola de radio $R$ centrada en el origen, es decir, $B_R(0,0,0)$. Integramos sobre su superficie:
\[ \iint\limits_{∂B_R^+} \vf \id{S} =
\iint\limits_{B_R} \left(\frac{x}{R^3},\frac{y}{R^3},\frac{z}{R^3} \right) \id S = \frac{1}{R^3} \iint\limits_{B_R} (x,y,z)\id S = \]
Dado que integrar el vector es integrar su componente escalar, la integral nos queda
\[ = \frac{1}{R^3} \iint\limits_{B_R} R\id{x,y} = \frac{1}{R^2}\cdot \mathrm{Area\; esfera} = 4π \]
Ahora bien, si no supiésemos ese argumento geométrico, empezaríamos parametrizando la esfera:
\[ Φ(θ,φ) =(R\cos θ \sin φ, R\sin θ\sin φ, R\cos φ);\, θ∈[0,2π], φ∈[0,π] \]
Calculamos los vectores tangentes y el normal:
\[ \begin{matrix} \\ T_θ = \\ T_φ= \end{matrix}
\left|
\begin{matrix}
\vec{i} 		& \vec{j} 		 & \vec{k} \\
-R\sin θ \sin φ & R\cos θ \sin φ & 0 \\
R\cos θ\cos φ 	& R\sin θ \cos φ & -R\sin φ
\end{matrix}\right|: T_θ×T_φ = -R\sin (R\cos θ, \]
La normal es interior, así que pagamos con un cambio de signo:
\begin{gather*} \iint\limits_{x^2+y^2+z^2 = R^2} \left(\frac{x}{R^3},\frac{y}{R^3},\frac{z}{R^3} \right) \id S = \\
- \int_0^{2π}\int_0^π\pesc{\left(\frac{R\cos θ \sin φ}{R^3},{R\sin θ \sin φ}{R^3},{R\cos φ}{R^3}\right), (,,)} = \dotsb \mathrm{Calculos\; aqui} \end{gather*}
y al final sale lo mismo que antes pero con cuentas mucho más desagrable.
¿Por qué el teorema de Gauss no funciona? La divergencia es 0 y la superficie es cerrada. Sin embargo, $\vf$ no es $C^1$ en el origen (no existe en ese punto) así que no podemos aplicarlo.
Pero, por otra parte, siempre hemos visto que la integral no se ve afectada por lo que ocurra en un punto. ¿Por qué no funciona el teorema de Gauss sólo por lo que pasa en el origen?
En realidad en el origen la divergencia vale $4π$ por la Delta de Dirac (δ).
Pero también podemos hacer un apaño. Consideramos un conjunto $Ω$, y una bola $B_ε(0,0,0)$. Entonces
\[ Ω_ε = Ω - B_ε \]
de tal forma que $\vf∈C^1$ en $Ω_ε$. Aplicando el teorema de Gauss:
\[ 0 = \iiint\limits_{Ω_ε}\dv \vf \id{x,y,z} = \iint\limits_{∂Ω_ε^+}\vf \id{S} \]
La frontera se divide en dos partes: $∂Ω_ε = ∂Ω + ∂B_ε^+$. Entonces
\[ 0 = \iint\limits_{∂Ω^+}\vf \id S - \iint\limits_{∂B_ε^+}\vf \id S \]
y por lo tanto, tenemos que
\[ \iint\limits_{∂Ω^+}\vf \id{S} = 4π\; ∀Ω \tq 0 ∈ Ω \]
\end{example}
\begin{theorem} Dado un campo $\vf \in C^1$, se tiene que
\[ \dv \vf = 0\dimplies \exists \vg\in C^2 \tlq \rot \vg = \vf \]
\end{theorem}
\begin{proof}
Con el lenguaje de las formas diferenciales es muy fácil esta demostración.
\todo[inline]{reescribir bien}
$\vf$ es una 1-forma a la que aplicamos la diferencial exterior y obtenemos una 2-forma, que es su rotacional. Entonces, al volver a hacer la diferencial (para hallar la divergencia) estamos aplicando dos veces el diferencial, y por lo tanto su valor es 0.
Sin formas diferenciales tenemos:
\[G=(G_1,G_2,G_3)\]
\[\rot G = \left(\ast_1,\ast_2,\ast_3\right)\]
\[\dv(\rot G) = \dpa{}{x}(\ast_1) + \dpa{}{y}(\ast_2) + \dpa{}{z}(\ast_3)\]
Por la igualdad de las derivadas cruzadas (toerema de Euler) al ser $G\in C^2$ se cancela todo.
$\implies$ Buscamos $\vg$ tal que $(F_1,F_2,F_3) = \rot \vg$.
Podemos definir el sistema:
\[\begin{array}{cc}
\dpa{G_3}{y} - \dpa{G_2}{z} &= F_1\\
\dpa{G_1}{z} - \dpa{G_3}{x} &= F_2\\
\dpa{G_2}{x} - \dpa{G_1}{y} &= F_3
\end{array}\]
Como tenemos varios grados de libertad, supongamos que $G_3\equiv 0$
\[\begin{array}{cc}
 - \dpa{G_2}{z} &= F_1\\
\dpa{G_1}{z} - &= F_2\\
\dpa{G_2}{x} - \dpa{G_1}{y} &= F_3
\end{array} \begin{array}{cc}
\longrightarrow & G_2 = -\int_0^z F_1(x,y,t)dt+A(x,y)\\
\longrightarrow & G_1 = \int_0^2 F_2(x,y,t)dt + B(x,y)\\
\longrightarrow & F_3 = \dpa{}{x} \left\{-\int_0^z F_1(x,y,t)dt + A(x,y)\right\}
- \dpa{}{y}\left\{\int_0^2 F_2(x,y,t)dt + B(x,y) \right\}
\end{array}
\]
Vamos a ver que ocurre con  $F_3$
\[-\dpa{}{x}\left(\int_0^z F_1(x,y,t)dt\right) + \dpa{A}{x} - \dpa{}{y}\int_0^z F_2(x,y,t)dt - \dpa{B}{y}\]
Por la regularidad de $F_1$ podemos meter dentro la derivada (el argumento que está detrás de esto se ve en teoría de la medida, asíque de momento nos fiamos)
\[-\left(\int_0^z \dpa{}{x}F_1(x,y,t)dt\right) + \dpa{A}{x} - \int_0^z \dpa{}{y}F_2(x,y,t)dt - \dpa{B}{y}\]
\[-\int_0^z \left(\dpa{F_1}{x} + \dpa{F_2}{y}\right)(x,y,t)dt + \dpa{A}{x} - \dpa{B}{y} \]
Utilizamos que la $\dv = 0$ que nos dice:
\[\dpa{F_1}{x} + \dpa{F_2}{y} + \dpa{F_3}{z} = 0\]
\[ = \int_0^z \dpa{F_3}{z} (x,y,t)dt + \dpa{A}{x} - \dpa{B}{y} = F_3(x,y,z) - F(x,y,z) + \dpa{A}{x} - \dpa{B}{y}\]
Hemos llegado a \[F_3(x,y,z) =  F_3(x,y,z) - F(x,y,z) + \dpa{A}{x} - \dpa{B}{y}\]
Quedando entonces definidas $A$ y $B$ así:
\[\dpa{A}{x} - \dpa{B}{y} = F_3(x,y,0)\]
Y aquí nuevamente tenemos muchas opciones. Tomamos $B=0$ por tomar algo
\[A(x,y) = \int_0^x F_3(s,y,0)ds + C(y)\]
\end{proof}




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


\chapter{Superficies y variedades diferenciales}
\section{Introducción: repaso en $\real^3$}
  En $\real^3$ tenemos puntos (dimensión 0), curvas (dimensión 1), superficies (dimensión 2) y abiertos (dimensión 3) sobre los que integrar en los que la imaginación resulta bastante útil. Pero... ¿qué pasa en $\real^N$?
  Entonces en $\real^N$ tenemos objetos de dimensión $0,...,N$ sobre los que vamos a poder definir propiedades, integrales, etc.
\subsection{Cálculo del plano tangente en $\real^3$}
  Repasamos la idea de que en $\real^3$ podíamos representar una superficie de varias maneras y cómo cálculabamos su plano tangente.
\paragraph{Gráfica: $z=f(x,y)$} Dada una superficie como una gráfica, simplemente construíamos el vector normal al plano derivando parcialmente:
\[ \vn = \left( \dpa{f}{x},\dpa{f}{y}, 1 \right) \]
\paragraph{Parametrización}  Con una parametrización $\phi$
\begin{align*}
\appl{\phi}{D\subset\real^2 &}{\real^3} \\
\phi(u,v) &= (x(u,v),y(u,v),z(u,v))
\end{align*}
     calculamos el plano tangente tomando los dos vectores directores y calculamos el normal al plano:
\begin{gather*}
      	T_u = \left( \dpa{x}{u},\dpa{y}{u},\dpa{z}{u}\right)\\
      	T_v = \left( \dpa{x}{v},\dpa{y}{v},\dpa{z}{v}\right)\\
\overrightarrow{n} = T_u\times T_v\\
\end{gather*}
     Nos podemos encontrar el problema de que $\overrightarrow{n} = \overrightarrow{0}$. Para evitar ese caso, estableceremos que el rango de la matriz de las 6 derivadas tiene que ser 2.
\paragraph{Conjunto de nivel} Supongamos que nos dan una gráfica definida como un conjunto de nivel $F(x,y,z) = 0$ .
   Para calcular el plano tangente en este caso tenemos que $\overrightarrow{n} = \nabla F$.
   Nos puede ocurrir que $F$ no sea derivable o que $\nabla F = \overrightarrow{0}$. Supongamos que sea diferenciable, ¿cómo preveer que puede salir? Para evitarlo, debemos forzar de nuevo que la matriz de las derivadas tenga rango máximo (en este caso 1).
\subsection{Cálculo de la recta tangente en $ℝ^3$}
  Vamos a ver que pasa con las curvas en $\real^3$ y cómo calcular la recta tangente
\begin{itemize}
\item Parametrizada: \[\sigma(t) = (x(t),y(t),z(t))\]
\item Intersección de 2 superficies transversales, es decir,
\[C = \left\{\begin{array}{cc} F_1(x,y,z) &= 0\\ F_2(x,y,z) &= 0 \end{array} \right.\]
   Posibles enemigos que nos podemos encontrar: superficies cuya intersección sea un plano. Si se da este caso, entonces tenemos que los vectores normales a las 2 superficies son paralelos. Para evitar esto, la matriz formada por los 2 vectores normales debe tener rango máximo.
\end{itemize}
 	Vemos claramente que las condiciones para poder calcular superficies tangentes llegan siempre a obligar a que la matriz tenga \textbf{rango máximo} (ver sección \ref{secThmRango}). A partir de aquí, podemos crear nuestra definición de subvariedad diferenciable:
\section{Subvariedades diferenciables}
\begin{defn}[Subvariedad\IS diferenciable]\label{defSubDif}
  Sea $M \subset \real^{M+N}$. Diremos que $M$ es una subvariedad diferenciable en $\real^{N+M}$ de dimensión $n$ y codimensión $k$\index{Codimensión} si y sólo si para todo punto $\ga$ existe un entorno abierto $U \subset \real^{N+K}$ con $\ga \in U$ de tal forma que $U \cap M = \{\gx\in U\tq F(\gx) = \gor{0}\}$ \textbf{para alguna función} $F\in C^1(U)$ con
\[\appl{F}{U\subset \real^{N+K}}{\real^K} \]
  cuya diferencial $DF$ tenga rango máximo (en este caso, rango $k$). De esta forma podremos expresar $U\cap M$ como
\[U\cap M = \left\{\begin{array}{cc}
                     F_1(x_1,...,x_{n+k}) = 0\\
                     F_2(x_1,...,x_{n+k}) = 0\\
\vdots\\
                     F_k(x_1,...,x_{n+k}) = 0
\end{array}\right.\]
\end{defn}
Veamos ejemplos de si algunos objetos son variedades diferenciables o no:
\paragraph{1) Superficie en $\real^3$}
\[\appl{F}{U\subset\real^3}{\real}\]
\[\{(x,y,z) \tq F(x,y,z) = 0\}\]
  En este caso tenemos $N=2, K=1$.
  La condición de rango nos dice que $\nabla F(\gx) \neq (0,0,0)$. Esto es, obliga a en cada punto existe un vector normal $\overrightarrow{n}$, exactamente la misma condición que habíamos visto antes.
\begin{remark} Si tuviésemos la superficie expresada como gráfica de una función ($M = \{z = f(x,y)\}$) bastaría con tomar $F(x,y,z) = f(x,y)-z$. En este caso
\[DF = \left(\dpa{f}{x},\dpa{f}{y},-1\right) \neq (0,0,0)\]
  Por lo tanto, las gráficas de funciones de 2 variables en $\real^3$ son siempre subvariedades (la condición de rango es gratuita).
\end{remark}
\paragraph{2)  Curvas en $\real^3$}
\[\sigma(t) = (x(t),y(t),z(t))\equiv S_1 \cap S_2 = \]
\[= \{F_1(x,y,z) = 0\}\cap \{F_2(x,y,z) = 0\}\]
  Si tomamos $U\cap \sigma = \{(x,y,z)\in\real^3 \tq F_1 = 0 \y F_2 = 0\}$
  Siendo \[\appl{F}{U\subset\real^3}{\real^2}, N+K=3,K=2\]\[F(x,y,z) = (F_1(x,y,z),F_2(x,y,z))\]
  Veamos la condición de rango en este caso:
\[rango \begin{pmatrix} \dpa{F_1}{x}&\dpa{F_1}{y}&\dpa{F_1}{z}\\\dpa{F_2}{x}&\dpa{F_2}{y}&\dpa{F_2}{z}\end{pmatrix}\]
  Para que el rango sea máximo, los vectores tienen que ser no paralelos, es decir, $S_1, S_2$ sean transversales, no paralelas. De nuevo, la misma condición que habíamos visto antes.
\paragraph{3) Punto en $ℝ^k$}
  Podemos definir un punto de una manera un tanto rebuscada:
\begin{gather*}
\appl{F}{\real^K}{\real^K}\\
\gx \rightarrow \gx - \ga
\end{gather*}
 En este caso, la subvariedad $M$ es nuestro punto $\ga$:
\[M = \{\gx \in \real^K \tq F(\gx) = \gor{0}\} = \{\ga\}\]
 Tenemos $DF = Id $, que tiene rango máximo y por lo tanto $\{\ga\}$ es una subvariedad diferenciable (dimensión 0, codimensión $k$).
\paragraph{4)} $\appl{F}{\Omega\subset\real^N}{0}$. En este caso tenemos codimensión $0$ y dimensión $N$.
\paragraph{5)}
\begin{gather*}
\appl{F}{\real^2}{\real}\\
   F(x,y) = x^3 - y^6 \\
  M = \{(x,y) \tq x^3-y^6 = 0\} \\
  DF = (3x^2-6y^5) \\
  DF(0,0) = (0,0)
\end{gather*}
  La matriz diferencial tiene rango $0$ en el punto $(0,0)$. ¿Quiere esto decir que $M$ no es una subvariedad diferenciable en el 0?
  No. Lo que quiere decir que no hemos encontrado la función que cumpla las hipótesis. Podemos operar
\[M = \{x^3=y^6\} = \{x = y^2\}  = \{x-y^2 = 0\}\]
  Y vemos que si tomamos $G(x,y) = x-y^2$, esta función representa la misma subvariedad $M$, y $DG(x,y) = (1,2y)$ tiene rango 1 en el origen.
\paragraph{6)}
\[M = \{(x,y)\in \real^2 \tq x^2-y^2 = 0\}\]
	Definimos una función $F$:
\[\appl{F}{\real^2}{\real}\]
\[F(x,y) = x^2-y^2\]
$DF = (2x,-2y)$. La condición de rango falla en $(0,0)$.
  Valoramos si este objeto no es una subvariedad o si tendremos que definir una función de una manera más inteligente, tal y como hicimos en el caso anterior.
\begin{wrapfigure}{r}{0.4\textwidth}
\begin{center}
\begin{tikzpicture}
\draw (-1.6,-1.6) -- (1.6,1.6);
\draw (-1.6,1.6) -- (1.6,-1.6);
\node[circle, draw, fill=black, inner sep=1pt, label=left:{$(0,0)$}] at (0,0) {};
\node[label=above right:{$y=-x$}] at (1.6,-1.6) {};
\node[label=below right:{$y=x$}] at (1.6,1.6) {};
\end{tikzpicture}
\caption{Subvariedad $M = \{ y=x \cup y = -x \}$}
\label{figSubX}
\end{center}
\end{wrapfigure}
  En este caso, vemos que $M = \{ y=x \cup y = -x \}$. No debería ser una subvariedad porque en el $(0,0)$ no es derivable (ver figura \ref{figSubX}). Intentaremos demostrarlo por reducción al absurdo.
  Supongamos que $M$ es una subvariedad. Entonces, según la definición (\ref{defSubDif})  existe un $U, (0,0) \in U$ y una aplicación  $\appl{G}{U\subset\real^2}{\real}$ con $U\cap M = \{G(x,y) = 0\}$. Entonces tendríamos que
\[\rango DG(x,y) = 1, \forall(x,y) \in U \implies \rango \left(\dpa{G}{x},\dpa{G}{y}\right) = 1\]
Ahí tenemos dos casos, o bien que la primera componente no sea $0$ o que sea la segunda la que no es nula. Supongamos primero que $\dpa{G}{x}(0,0) \neq 0$. Podemos aplicar el Teorema de la unción implícita (\ref{TFImp}), que nos dice que podemos despejar $x = x(y)$. En este caso:
$U \cap M = \{x(y)^2-y^2 = 0\}$.
Si fijamos $y=\varepsilon$, entonces $x(\varepsilon) = \pm \varepsilon$ No es una función, lo que contradice el Teorema de la función implícita, y por lo tanto es imposible que $\dpa{G}{x}(0,0) \neq 0$. Análogamente, tampoco puede cumplirse que $\dpa{G}{y}(0,0) \neq 0$.
Hemos demostrado por lo tanto que no puede existir una función que defina esto como subvariedad diferencial. Este es el ejemplo de que cualquier objeto que tenga autointersección no puede ser subvariedad.
\paragraph{7)} $M = \{(x,y) \in \real^2 \tq x^2-y^2 = 0, y\ge 0\}$
Vamos a suponer que existe una función $F \in C^1$ que representa ese objeto (que viene definido por 2 condiciones). $M = \{F(x,y) = 0\}$ para alguna $F$.
Condición de rango: $\left(\dpa{F}{x},\dpa{F}{y}\right) \neq (0,0)$.
 Condición de rango: $\left(\dpa{F}{x},\dpa{F}{y}\right) = (0,0), x=y=0$.
 Vamos a ver si es subvariedad o no. En este caso intuimos que no debería serlo. Volvemos a demostrar por reducción al absurdo:
 Supongamos que $M$ es subvariedad, entonces $\exists G(x,y)$ tal que $\appl{G}{U\subset\real^2}{\real}, U \cap M = \{G(x,y) = 0\}$
 Supongamos $\displaystyle \dpa{G}{x}\neq 0$. Entonces tenemos \[ M\cap U = \{y(x)^2 - y^2 = 0\} \]
 Si fijamos $x=\varepsilon \implies y(x) = \abs{\varepsilon}$, pero esto quiere decir que $G \notin C^1$. De forma análoga con la segunda coordenada, vemos que $M$ no es una subvariedad.
\paragraph{8)} Nos quitamos el punto conflictivo del caso anterior, el $(0,0)$.
$N = \{(x,y)\in \real^2 \tq x^2-y^2 = 0, y>0\}$
La lógica nos dice que este caso si debería ser subvariedad diferencial:  la definición de la función es local, y siempre podremos encontrar un entorno que no incluya el 0, que es el punto problemático.
Comprobamos que efectivamente el rango de $\nabla F$ es máximo $\forall (x,y)\in \real^2$ y por lo tanto $M$ es una subvariedad.
\subsection{Subvariedades y parametrizaciones}
\paragraph{Ejemplo} Superficie en $\real^3$ parametrizada: $S = \{\Phi(u,v) = (x(u,v),y(u,v),z(u,v))\}$.
A la hora de trabajar con superficies parametrizadas, nos interesaría poder definir una especie de función inversa que nos permita hacer cambios en el plano y llevarlos a la superficie o al reves, pero... ¡tienen dimensiones distintas! La esperanza que nos queda es que la superficie parametrizada tiene dimensión 2, igual que el plano.
\begin{defn}[Homeomorfismo] \label{defHomeomorfismo}
Sea $\appl{\Phi}{\Omega\subset\real^N}{\real^{N+K}}, \Omega$ abierto.
$\Phi$ es un \emph{homeomorfismo} sobre su imagen $\dimplies $ la restricción $\appl{\Phi}{\Omega}{\Phi(\Omega)}$ es continua y tiene una inversa continua,
es decir, \[\exists \appl{\Psi}{\Phi(\Omega)}{\Omega} \tlq
\left\{ \begin{array}{cc}
\Psi(\Phi(\gor{u})) = \gor{u}, &\forall \gor{u} \in \Omega\\
\Psi(\Phi(\gor{x})) = \gx, &\forall \gx \in \Phi(\Omega)
\end{array}\right.\]
\paragraph{Definición 1)}
Dado un $\displaystyle x_0 \in \Phi(\Omega) \implies \forall \varepsilon >0, \exists \delta>0 \tlq$
si $\begin{array}{lc}
\norm{\gx-\gor{x_0})} < \delta \implies \norm{\Psi(\gx)-\Psi(\gor{x_0})}<\varepsilon\\
\gx \in \Phi(\Omega)
\end{array}$
\paragraph{Definición alternativa de continuidad}
Si $\{X_n\}\subset\Phi(\Omega), \gor{X_n} \rightarrow \gor{x_0}\in\Phi(\Omega) \implies \Psi(\gor{X_n}) \rightarrow \Psi(\gor{x_0})$
\end{defn}
\subsubsection{Ejemplos}
\paragraph{Ejemplo 1}
\[\appl{\sigma}{[0,2\pi)}{\real^2}\]
\[t \rightarrow \sigma(t) = (cos(t),sen(t))\]
Inversa: $\Psi(x,y) = t$ ángulo de la representación en polares.
Vamos a estudiar el problema de la continuidad:
Tomamos $\{(X_n,Y_n)\}$ con $x^2+y^2 = 1 \tlq (x_n,y_n) \convs (1,0)$
Si $\Psi$ es continua, debe ser $\Psi(x_n,y_n) \convs (1,0) = 0$. En este caso no es continua porque:
Si tomamos \begin{align*}
P_n &= \left(cos\left(2\pi - \frac{1}{n}\right), sen\left(2\pi - \frac{1}{n}\right) \right)\\
P_n &\convs (1,0)\\
\Psi(P_n) &= 2\pi - \frac{1}{n} \convs 2\pi\neq\Psi(1,0)
\end{align*}
\paragraph{Ejemplo 2}
\[\appl{f}{(0,1)\subset\real}{\real^2}\]
\[t \rightarrow f(t) = (t,g(t)), \text{continua, con inversa continua}\]
Vamos a definir la  inversa:
\[P\in f(0,1) \implies P(x,g(x)) \text{Para algún } x\in(0,1)\]
$P = (x,g(x))$
\[\Psi(P) = t \in (0,1) \tlq f(t) = (x,g(x)) \implies t = x\]
Vamos a estudiar la continuidad:
\[\{P_n\} \subset f(0,1), P_n \rightarrow P \in f(0,1)\]
\[P_i = (x_i,g(x_i)), \text{ para algún } i \in (0,1)\]
\[P_n \convs P_0 \dimplies (x_n,g(x_n)) \rightarrow (x_0,g(x_0)) \implies x_n (= \Psi(P_n)) \rightarrow x_0 (=\Psi(P_0)) \]
\obs ¿La gráfica de una función es homeomorfismo sobre su imagen?
\paragraph{Ejemplo 3}
\[\appl{\sigma_3}{(0,4\pi)}{\real^2}\]
\[t \rightarrow \sigma(t) = (cos(t),sen(t))\]
No es inyectiva $\implies \nexists \Psi$.
\paragraph{Ejemplo 4: Circunferencia}
\[\appl{\sigma_4)}{(0,2\pi)}{\real^2}\]
\[t \rightarrow \sigma(t) = (cos(t),sen(t))\]
La diferencia con el ejemplo 1, es que es cerrado.
Hay que percatarse de que la tangente no es inyectiva, entonces... la inversa es algo más complicada que $\arctan$, así que vamos a definirla a trozos siguiendo el esquema de la figura \ref{imgCirc_2}.
\begin{figure}[hbtp]
\begin{center}
\begin{tikzpicture}[scale=1]
% Ejes
\draw[->] (-3,0) -- (3,0);
\draw[->] (0,-3) -- (0,3);
% Partes de la circunferencia
\draw[very thick,red] (2,0) arc (0:90:2);
\draw[very thick,blue] (0,2) arc (90:270:2);
\draw[very thick,green] (0,-2) arc(270:360:2);
% Etiquetas
\node[red] at (1.7, 1.7) {(1)};
\node[blue] at (-2.3, 0.3) {(2)};
\node[green] at (1.7, -1.7) {(3)};
\end{tikzpicture}
\caption{Circunferencia definida en tres trozos}
\label{imgCirc_2}
\end{center}
\end{figure}
\[\Psi(x,y) =
\begin{cases}
\arctan\left(\frac{y}{x}\right) & (x,y)\in 1\\
\arctan\left(\frac{y}{x}\right) + \pi & (x,y) \in 2\\
\arctan\left(\frac{y}{x}\right)+2\pi& (x,y) \in 3
\end{cases}
\]
Hay que estudiar la continuidad en $(0,-1)$ y en $(0,1)$.
\subparagraph{Continuidad en (0,1)}
Tomamos $\{P_n\} \rightarrow (0,1), P_n \in S_1$
Queremos probar que $\Psi(P_n) \rightarrow \Psi(0,1) = \frac{\pi}{2}$.
Ejercicio para el lector:
Sucesiones que se acercan por la derecha o por la izquierda y comprobar que vale lo que tiene que valer.
\paragraph{Ejemplo 5: Lemniscata}
\begin{figure}[hbtp]
\begin{center}
\begin{tikzpicture}[scale=2,declare function={
	lemnx(\x)=2.5*cos(\x) / ( sin(\x)^2+ 1);
	lemny(\x)=3*sin(\x) * cos(\x) / ( sin(\x) ^2 + 1;
	}]
% Ejes
\draw[->] (-3,0) -- (3,0);
\draw[->] (0,-2) -- (0,2);
% La curva
\draw[gray,domain=-90:270,samples=200] plot ({lemnx(\x)}, {lemny(\x)});
% Sucesión 1
\foreach \x in {-86,-82,...,-66}
\node[circle, red, draw,inner sep=2pt] at ({lemnx(\x)}, {lemny(\x)}) {};
% Sucesión 2
\foreach \x in {72,76,...,108}
\node[rectangle, blue, draw,inner sep=2pt] at ({lemnx(\x)}, {lemny(\x)}) {};
% Sucesión 3
\foreach \x in {242,246,...,266}
\node[diamond, orange, draw,inner sep=2pt] at ({lemnx(\x)}, {lemny(\x)}) {};
% Puntos t = 0, t=π
\node[label=above right:$t\eq 0$, draw, fill=white,circle, inner sep=2pt] at (2.5,0) {};
\node[label=above left:$t\eq \pi$, draw, fill=white,circle, inner sep=2pt] at (-2.5,0){};
% Flechas para indicar hacia donde va la t.
\foreach \x in {-45,44,134,224}
\draw[-angle 90] ({lemnx(\x)},{lemny(\x)}) -- ({lemnx(\x + 1)},{lemny(\x +1)});
% Etiquetas de las sucesiones.
\node[label={[red]below:(1)}] at ({lemnx(-66)},{lemny(-66)}) {};
\node[label={[blue]above:(2)}] at ({lemnx(72)},{lemny(72)}) {};
\node[label={[orange]above:(3)}] at ({lemnx(242)},{lemny(242)}) {};
\end{tikzpicture}
\caption{Curva Lemniscata}
\end{center}
\end{figure}
La parametrización es \[\sigma_5 (x(t),y(t)) = \left(\frac{\cos(t)}{\sin^2(t)+1},\frac{\sin(t)\cos(t)}{\sin^2(t)+1}\right), t\in \left(\frac{-\pi}{2},\frac{3\pi}{2}\right)\]
Al origen podemos acercarnos de distintas formas:
\begin{itemize}
\item Cuando $t \to - \frac{\pi}{2}$, nos acercamos por la sucesión 1 (desde abajo a la derecha).
\item Cuando $t \sim \frac{\pi}{2}$, nos acercamos por la sucesión 2 (la mitad de la curva, de arriba-derecha a abajo-izquierda).
\item Cuando $t \to \frac{3\pi}{2}$, nos acercamos por la sucesión 3 (desde arriba a la izquierda)
\end{itemize}
Sea $\{P_n\}\subset \sigma_5(t) \rightarrow (0,0)$.
Podemos tomar la sucesión $\{P_n\} = \{P_1,P_2,P_3,...\}$ cada uno en una región (1,2,3 ciclicamente).
\[\Psi(P_n) \begin{cases}
\in 3 & \text{ si }n \text{ es múltiplo de }3\\
\in 2 & \text{ si } n\equiv 2\ mod \ 3\\
\in 1 & \text{ si } n \equiv 1\ mod \ 3
\end{cases}\]
Por tanto $\nexists \displaystyle \lim_{n\rightarrow \infty} \Psi(P_n)$
\begin{remark} A pesar de que hemos demostrado que $\sigma$ es continua e inyectiva, esto no garantiza que la inversa sea continua.\end{remark}
\subsection{Parametrizaciones}
\paragraph{Objetivo} definir "parametrización".
\subparagraph{Ejemplo 1} Curva parametrizada en $\real^3$
$\Gamma = \{\sigma(t) = (x(t),y(t),z(t)), t \in (a,b)\}$
Queremos excluir:
\begin{itemize}
\item Picos (valor absoluto. FOTO)
Basta con imponer: $\sigma \in C^1 \y (x',y',z') \neq (0,0,0)$
\item Auto-intersecciones o Lemniscata (que no se auto-intersecciona pero por poquito)
Basta imponer $\sigma$ sea un homeomorfismo sobre su imagen.
\end{itemize}
\paragraph{Ejemplo 2} Superficies de parametrización en $\real^3$.
\[S = \{\Phi(u,v) = (x(u,v),y(u,v),z(u,v)), (u,v)\in D\}\]
Queremos evitar:
\begin{itemize}
\item Cono, tienda de campaña
$Rango \begin{pmatrix}
T_u \rightarrow\\
T_v \rightarrow
\end{pmatrix} = 2 \implies $ Podemos calcular plano tangente
\item Autointersección
Aquí sí tenemos rango máximo, asíque impondremos la condición de homeomorfismo sobre su imagen.
\end{itemize}
Ya tenemos todo lo necesario para definir parametrización:
\begin{defn}[Parametrización\IS local] \label{defParametrizacion}
Diremos que $\appl{\Psi}{\omega \subset \real^N}{\real^{N+K}}, \Psi \in C^1(\omega)$, es una parametrización local $\dimplies \left\{ \begin{array}{c}
 rango D\Psi = n \text{ máximo}\\
 \Psi \text{ es un homeomorfismo sobre su imagen}
\end{array}\right.$
\end{defn}
\subsubsection{Repaso de coordenadas cilíndricas y esféricas.}
\input{CALII/repaso_coordenadas.tex}
\subsubsection{Ejemplos}
\subparagraph{Esfera en $\real^3$}
$\Phi_{1,2}(x,y) = (x,y,\pm \sqrt{1-x^2-y^2})$. Esta \emph{"carta de parametrización"} nos deja sin definir el ecuador. Para ello tenemos que definir más \emph{cartas de parametrización} \index{Carta!de parametrización}
 Estas cartas son expresando x,y en función de las otras 2. En total hacen falta 3 parametrizaciones.
\subparagraph{Existe} otra manera de parametrizar, la proyección estereográfica.
\index{Proyección\IS estereográfica}
El dibujo de la proyección es:
\input{tikz/ProyeccionEstereografica.tex}
\[(u,v) \in \real^2 \rightarrow (u,v,0) \rightarrow r\equiv (0,0,R) + t(u,v,-R) = (tu,tv,R(1-t)\]
 Imponiendo $\underbrace{P}_{r(t_0)} \equiv r\cap S$ tenemos: \[(t_0u)^2+(t_0v)^2 + R^2(1-t)^2 = R^2 \rightarrow ... \rightarrow t_0 = \frac{2R^2}{u^2+v^2+R^2}\]
 Conclusión: \[P = (tu,tv,R(1-t) = \frac{2R^2}{u^2+v^2+R^2}u,\frac{2R^2}{u^2+v^2+R^2}v,\frac{R(u^2+v^2-R^2)}{u^2+v^2+R^2} = \Phi(u,v)\].
 Vemos que $\Phi\in C^1, \Phi(\real^2) = S_R-\{(0,0,R)\}$ ¿Es una parametrización?
 Hay que comprobar \begin{itemize}
\item rango $D\Phi$ máximo. (Se deja como ejercicio para el lector)
\item $\Phi$ es homeomorfismo sobre su imagen, es decir, ¿Existe una inversa continua?
\emph{Inversa}
 Dado $(x,y,z)$ queremos despejar $(u,v)$.
 Idea: $(u,v,0)$ es la intersección de la recta que unie $(x,y,z)$ con $(0,0,R)$ y el plano $z=0$.
 Recta: $s(t) = (tx,ty,R+t(z-R))$.
 Punto de corte con el plano $z=0$: El punto de corte tendrá coordenada tercera = 0, es decir:
$R+t(z-R)$
 Buscamos $t_0$ tal que $R+t_0(z-R)=0 \dimplies t_0=\frac{R}{R-z}$.
 Sustituyendo en la recta obtenemos: $u = t_0x, v=t_0y$
 Si calculamos $\Phi^{-1}(x,y,z) = \left(\frac{Rx}{R-z},\frac{Ry}{R-z}\right)$. Esta inversa es continua en $Img(\Phi(\real^2)) \equiv \{Esfera - \{(0,0,R)\}\}$  (El punto (0,0,R) no está incluido, por definición, en la imagen).
\end{itemize}
\subsection{Teoremas de las subvariedades}
\begin{theorem}\label{thmSubvariedades}
Los siguientes enunciados son equivalentes:
\begin{itemize}
\item[1] $M$ es una subvariedad diferenciable n-dimensional en $\real^{N+K}$. \label{eq_1}
\item[2] $\forall \gor{a} \in M $ existe una parametrización local $\appl{\Phi}{\omega\subset \real^N}{\real^{N+K}}$ con $\gor{a}\in \Phi(\omega)$\label{eq_2}
\item[3] $\forall \gor{a} \in M$ existe un abierto $V\subset \real^{N+K}, \gor{a}\in V$ y una aplicación
\label{eq_3}
\[\appl{\Psi}{V}{\real^{N+K}}, \Psi\ \text{un difeomorfismo} \tlq \Psi = (\Psi_1,...,\Psi_n,\Psi_{n+1},...,\Psi_{n+k})\]
Si $\gx \in V\cap M \implies$
\[\Psi_{n+1}(\gx) = ... = \Psi_{n+k}(\gx) = 0\]
\end{itemize}
\end{theorem}
\paragraph{Observación 1:} En \ref{eq_2}.2, llamaremos \textbf{carta local}\index{Carta!local} al conjunto definido por la fórmula y el dominio, $(\Phi,\omega)$. El conjunto de todas las cartas locales que definen una subvariedad se llama Atlas.
\subparagraph{Ejemplo:}
 La proyección estereográfica tiene 2 cartas, la del polo norte (que excluye ese punto) y la del polo sur.
\paragraph{Observación 2:} $\ref{eq_1}.1 \dimplies \ref{eq_2}.2$. Si tenemos una subvariedad dada como conjunto de nivel la podemos parametrizar (y viceversa).
\begin{defn}[Difeomorfismo]
$\Psi$ es un difeomorfismo $\dimplies \Psi\in C^1,\exists \Psi^{-1}, \tlq \Psi^{-1}\in C^1$
\end{defn}
\begin{proof}
Esquema: $1\implies 2, 2\implies 3, 3 \implies 1$
\paragraph{1 $\implies$ 2\\}
Sea $\ga \in M, \exists U\subset\real^{N+K}$ abierto con $\ga \in U$ y una función $\appl{F}{U\subset \rnk}{\rk}, F\in C^1(U), \tlq U\cap M = \{\gx \in U\tq F(\gx) = \gor{0}\}$. Además $DF$ tiene rango máximo (K).
Queremos demostrar que existe una parametrización $\Phi$.
\subparagraph{Permutando} el orden de las variables, suponemos que el menor de orden $K$ con determinante no nulo corresponde con las $K$ últimas variables.
Por el teorema de la función implícita, $F(x_1,...,x_n,x_{n+1},...,x_{n+k}) = \gor{0}$, con $x_{n+1},...,x_{n+k}$ despejable en función de las $\{x_i,i=1,...,n\}$ en un entonro de $\gor{a}$.
Es decir: existen $\omega\subset \real^N, \omega'\subset\rk$ abiertos tales que $\gor{a}\in \omega \times \omega'$ y una función $\appl{g}{\omega\subset\real^N}{\omega'\subset\rk}$ de manera que
$$\left\{\begin{array}{c}
g(a_1,...,a_n) = (a_{n+1},...,a_{n+k})\\
F(\gx,g(\gx)) = \gor{0}, \forall \gx \in \omega\end{array}\right.$$
Idea: la parametrización es $\Phi (\gx) = (\gx,g(\gx))$
Vamos a comprobar las condiciones:
\begin{itemize}
\item $\Phi \in C^1$. Por el teorema de la función implícita, tenemos que $\Phi$ es diferenciable (porque $F$ y $g$ lo son).
\item \[D\Phi = ... =
\begin{pmatrix}
Id_{n \times n}\\
\hline
Dg
\end{pmatrix}\] con rango máximo.
\item ¿Homeomorfismo sobre su imagen? $(x,y)\in M$ en un entorno de $\ga \in \omega\times\omega'$ En ese entonrno $y=g(\gx)$.
\end{itemize}
Es decir, $(x,y) = (x,g(x)) \xrightarrow{\Phi}) \gx \xrightarrow{\Phi^{-1}} (x,g(x)) = (x,y) $. También $\inv{\Phi}(x,y) = x, \forall(x,y)\in (\omega\times\omega') \cap M$ Continua.
\paragraph{2 $\implies$ 3} Vamos a emplear un argumento como el de la demostración del segundo teorema del rango. \ref{TR2}
Buscamos:
\begin{align*}
\appl{\Phi}{\rnk}{\rnk} \tlq \Phi(V\cap M) = (\ast &,0)\\
&\uparrow\\
k \text{ últimas coor} & \text{denadas}
\end{align*}
Siendo $\Phi$ un difeomorfismo.
\paragraph{Sabemos:} existe una parametrización local $\appl{\Psi}{\real^N}{\rnk}$.
\begin{itemize}
\item $D\Psi$ rango máximo.
\item $\Psi$ homeomorfismo sobre su imagen.
\end{itemize}
\subparagraph{Idea:} Completar el número de variables
Definimos
\begin{align*}
\appl{\alpha}{\omega\times\real^K \subset \real^N\times\real^K}&{\real^N\times\real^K}\\
(\gor{u},\gor{v})\longrightarrow &\alpha(\gor{u},\gor{v}) = \Psi(\gor{u}) + (\gor{0},\gor{v})\\
\gor{u} \in \real^N,\gor{v} \in \real^K, \Phi(\gor{u})\in \real^{N+K}
\end{align*}
\paragraph{Paso 2)} Aplicar el teorema de la función inversa (\ref{thmInv}) a $\alpha$.
\[D\alpha =
\left(t.
\begin{array}{c|c}
		D\Psi_k  \rightarrow & 0\\
\hline
		D\Psi_{n+i}  \rightarrow & I
\end{array}\right.
\]

--------------

\chapter{Superficies y variedades diferenciales}
\section{Introducción: repaso en $\real^3$}
  En $\real^3$ tenemos puntos (dimensión 0), curvas (dimensión 1), superficies (dimensión 2) y abiertos (dimensión 3) sobre los que integrar en los que la imaginación resulta bastante útil. Pero... ¿qué pasa en $\real^N$?
  Entonces en $\real^N$ tenemos objetos de dimensión $0,...,N$ sobre los que vamos a poder definir propiedades, integrales, etc.
\subsection{Cálculo del plano tangente en $\real^3$}
  Repasamos la idea de que en $\real^3$ podíamos representar una superficie de varias maneras y cómo cálculabamos su plano tangente.
\paragraph{Gráfica: $z=f(x,y)$} Dada una superficie como una gráfica, simplemente construíamos el vector normal al plano derivando parcialmente:
\[ \vn = \left( \dpa{f}{x},\dpa{f}{y}, 1 \right) \]
\paragraph{Parametrización}  Con una parametrización $\phi$
\begin{align*}
\appl{\phi}{D\subset\real^2 &}{\real^3} \\
\phi(u,v) &= (x(u,v),y(u,v),z(u,v))
\end{align*}
     calculamos el plano tangente tomando los dos vectores directores y calculamos el normal al plano:
\begin{gather*}
      	T_u = \left( \dpa{x}{u},\dpa{y}{u},\dpa{z}{u}\right)\\
      	T_v = \left( \dpa{x}{v},\dpa{y}{v},\dpa{z}{v}\right)\\
\overrightarrow{n} = T_u\times T_v\\
\end{gather*}
     Nos podemos encontrar el problema de que $\overrightarrow{n} = \overrightarrow{0}$. Para evitar ese caso, estableceremos que el rango de la matriz de las 6 derivadas tiene que ser 2.
\paragraph{Conjunto de nivel} Supongamos que nos dan una gráfica definida como un conjunto de nivel $F(x,y,z) = 0$ .
   Para calcular el plano tangente en este caso tenemos que $\overrightarrow{n} = \nabla F$.
   Nos puede ocurrir que $F$ no sea derivable o que $\nabla F = \overrightarrow{0}$. Supongamos que sea diferenciable, ¿cómo preveer que puede salir? Para evitarlo, debemos forzar de nuevo que la matriz de las derivadas tenga rango máximo (en este caso 1).
\subsection{Cálculo de la recta tangente en $ℝ^3$}
  Vamos a ver que pasa con las curvas en $\real^3$ y cómo calcular la recta tangente
\begin{itemize}
\item Parametrizada: \[\sigma(t) = (x(t),y(t),z(t))\]
\item Intersección de 2 superficies transversales, es decir,
\[C = \left\{\begin{array}{cc} F_1(x,y,z) &= 0\\ F_2(x,y,z) &= 0 \end{array} \right.\]
   Posibles enemigos que nos podemos encontrar: superficies cuya intersección sea un plano. Si se da este caso, entonces tenemos que los vectores normales a las 2 superficies son paralelos. Para evitar esto, la matriz formada por los 2 vectores normales debe tener rango máximo.
\end{itemize}
 	Vemos claramente que las condiciones para poder calcular superficies tangentes llegan siempre a obligar a que la matriz tenga \textbf{rango máximo} (ver sección \ref{secThmRango}). A partir de aquí, podemos crear nuestra definición de subvariedad diferenciable:
\section{Subvariedades diferenciables}
\begin{defn}[Subvariedad\IS diferenciable]\label{defSubDif}
  Sea $M \subset \real^{M+N}$. Diremos que $M$ es una subvariedad diferenciable en $\real^{N+M}$ de dimensión $n$ y codimensión $k$\index{Codimensión} si y sólo si para todo punto $\ga$ existe un entorno abierto $U \subset \real^{N+K}$ con $\ga \in U$ de tal forma que $U \cap M = \{\gx\in U\tq F(\gx) = \gor{0}\}$ \textbf{para alguna función} $F\in C^1(U)$ con
\[\appl{F}{U\subset \real^{N+K}}{\real^K} \]
  cuya diferencial $DF$ tenga rango máximo (en este caso, rango $k$). De esta forma podremos expresar $U\cap M$ como
\[U\cap M = \left\{\begin{array}{cc}
                     F_1(x_1,...,x_{n+k}) = 0\\
                     F_2(x_1,...,x_{n+k}) = 0\\
\vdots\\
                     F_k(x_1,...,x_{n+k}) = 0
\end{array}\right.\]
\end{defn}
Veamos ejemplos de si algunos objetos son variedades diferenciables o no:
\paragraph{1) Superficie en $\real^3$}
\[\appl{F}{U\subset\real^3}{\real}\]
\[\{(x,y,z) \tq F(x,y,z) = 0\}\]
  En este caso tenemos $N=2, K=1$.
  La condición de rango nos dice que $\nabla F(\gx) \neq (0,0,0)$. Esto es, obliga a en cada punto existe un vector normal $\overrightarrow{n}$, exactamente la misma condición que habíamos visto antes.
\begin{remark} Si tuviésemos la superficie expresada como gráfica de una función ($M = \{z = f(x,y)\}$) bastaría con tomar $F(x,y,z) = f(x,y)-z$. En este caso
\[DF = \left(\dpa{f}{x},\dpa{f}{y},-1\right) \neq (0,0,0)\]
  Por lo tanto, las gráficas de funciones de 2 variables en $\real^3$ son siempre subvariedades (la condición de rango es gratuita).
\end{remark}
\paragraph{2)  Curvas en $\real^3$}
\[\sigma(t) = (x(t),y(t),z(t))\equiv S_1 \cap S_2 = \]
\[= \{F_1(x,y,z) = 0\}\cap \{F_2(x,y,z) = 0\}\]
  Si tomamos $U\cap \sigma = \{(x,y,z)\in\real^3 \tq F_1 = 0 \y F_2 = 0\}$
  Siendo \[\appl{F}{U\subset\real^3}{\real^2}, N+K=3,K=2\]\[F(x,y,z) = (F_1(x,y,z),F_2(x,y,z))\]
  Veamos la condición de rango en este caso:
\[rango \begin{pmatrix} \dpa{F_1}{x}&\dpa{F_1}{y}&\dpa{F_1}{z}\\\dpa{F_2}{x}&\dpa{F_2}{y}&\dpa{F_2}{z}\end{pmatrix}\]
  Para que el rango sea máximo, los vectores tienen que ser no paralelos, es decir, $S_1, S_2$ sean transversales, no paralelas. De nuevo, la misma condición que habíamos visto antes.
\paragraph{3) Punto en $ℝ^k$}
  Podemos definir un punto de una manera un tanto rebuscada:
\begin{gather*}
\appl{F}{\real^K}{\real^K}\\
\gx \rightarrow \gx - \ga
\end{gather*}
 En este caso, la subvariedad $M$ es nuestro punto $\ga$:
\[M = \{\gx \in \real^K \tq F(\gx) = \gor{0}\} = \{\ga\}\]
 Tenemos $DF = Id $, que tiene rango máximo y por lo tanto $\{\ga\}$ es una subvariedad diferenciable (dimensión 0, codimensión $k$).
\paragraph{4)} $\appl{F}{\Omega\subset\real^N}{0}$. En este caso tenemos codimensión $0$ y dimensión $N$.
\paragraph{5)}
\begin{gather*}
\appl{F}{\real^2}{\real}\\
   F(x,y) = x^3 - y^6 \\
  M = \{(x,y) \tq x^3-y^6 = 0\} \\
  DF = (3x^2-6y^5) \\
  DF(0,0) = (0,0)
\end{gather*}
  La matriz diferencial tiene rango $0$ en el punto $(0,0)$. ¿Quiere esto decir que $M$ no es una subvariedad diferenciable en el 0?
  No. Lo que quiere decir que no hemos encontrado la función que cumpla las hipótesis. Podemos operar
\[M = \{x^3=y^6\} = \{x = y^2\}  = \{x-y^2 = 0\}\]
  Y vemos que si tomamos $G(x,y) = x-y^2$, esta función representa la misma subvariedad $M$, y $DG(x,y) = (1,2y)$ tiene rango 1 en el origen.
\paragraph{6)}
\[M = \{(x,y)\in \real^2 \tq x^2-y^2 = 0\}\]
	Definimos una función $F$:
\[\appl{F}{\real^2}{\real}\]
\[F(x,y) = x^2-y^2\]
$DF = (2x,-2y)$. La condición de rango falla en $(0,0)$.
  Valoramos si este objeto no es una subvariedad o si tendremos que definir una función de una manera más inteligente, tal y como hicimos en el caso anterior.
\begin{wrapfigure}{r}{0.4\textwidth}
\begin{center}
\begin{tikzpicture}
\draw (-1.6,-1.6) -- (1.6,1.6);
\draw (-1.6,1.6) -- (1.6,-1.6);
\node[circle, draw, fill=black, inner sep=1pt, label=left:{$(0,0)$}] at (0,0) {};
\node[label=above right:{$y=-x$}] at (1.6,-1.6) {};
\node[label=below right:{$y=x$}] at (1.6,1.6) {};
\end{tikzpicture}
\caption{Subvariedad $M = \{ y=x \cup y = -x \}$}
\label{figSubX}
\end{center}
\end{wrapfigure}
  En este caso, vemos que $M = \{ y=x \cup y = -x \}$. No debería ser una subvariedad porque en el $(0,0)$ no es derivable (ver figura \ref{figSubX}). Intentaremos demostrarlo por reducción al absurdo.
  Supongamos que $M$ es una subvariedad. Entonces, según la definición (\ref{defSubDif})  existe un $U, (0,0) \in U$ y una aplicación  $\appl{G}{U\subset\real^2}{\real}$ con $U\cap M = \{G(x,y) = 0\}$. Entonces tendríamos que
\[\rango DG(x,y) = 1, \forall(x,y) \in U \implies \rango \left(\dpa{G}{x},\dpa{G}{y}\right) = 1\]
Ahí tenemos dos casos, o bien que la primera componente no sea $0$ o que sea la segunda la que no es nula. Supongamos primero que $\dpa{G}{x}(0,0) \neq 0$. Podemos aplicar el Teorema de la unción implícita (\ref{TFImp}), que nos dice que podemos despejar $x = x(y)$. En este caso:
$U \cap M = \{x(y)^2-y^2 = 0\}$.
Si fijamos $y=\varepsilon$, entonces $x(\varepsilon) = \pm \varepsilon$ No es una función, lo que contradice el Teorema de la función implícita, y por lo tanto es imposible que $\dpa{G}{x}(0,0) \neq 0$. Análogamente, tampoco puede cumplirse que $\dpa{G}{y}(0,0) \neq 0$.
Hemos demostrado por lo tanto que no puede existir una función que defina esto como subvariedad diferencial. Este es el ejemplo de que cualquier objeto que tenga autointersección no puede ser subvariedad.
\paragraph{7)} $M = \{(x,y) \in \real^2 \tq x^2-y^2 = 0, y\ge 0\}$
Vamos a suponer que existe una función $F \in C^1$ que representa ese objeto (que viene definido por 2 condiciones). $M = \{F(x,y) = 0\}$ para alguna $F$.
Condición de rango: $\left(\dpa{F}{x},\dpa{F}{y}\right) \neq (0,0)$.
 Condición de rango: $\left(\dpa{F}{x},\dpa{F}{y}\right) = (0,0), x=y=0$.
 Vamos a ver si es subvariedad o no. En este caso intuimos que no debería serlo. Volvemos a demostrar por reducción al absurdo:
 Supongamos que $M$ es subvariedad, entonces $\exists G(x,y)$ tal que $\appl{G}{U\subset\real^2}{\real}, U \cap M = \{G(x,y) = 0\}$
 Supongamos $\displaystyle \dpa{G}{x}\neq 0$. Entonces tenemos \[ M\cap U = \{y(x)^2 - y^2 = 0\} \]
 Si fijamos $x=\varepsilon \implies y(x) = \abs{\varepsilon}$, pero esto quiere decir que $G \notin C^1$. De forma análoga con la segunda coordenada, vemos que $M$ no es una subvariedad.
\paragraph{8)} Nos quitamos el punto conflictivo del caso anterior, el $(0,0)$.
$N = \{(x,y)\in \real^2 \tq x^2-y^2 = 0, y>0\}$
La lógica nos dice que este caso si debería ser subvariedad diferencial:  la definición de la función es local, y siempre podremos encontrar un entorno que no incluya el 0, que es el punto problemático.
Comprobamos que efectivamente el rango de $\nabla F$ es máximo $\forall (x,y)\in \real^2$ y por lo tanto $M$ es una subvariedad.
\subsection{Subvariedades y parametrizaciones}
\paragraph{Ejemplo} Superficie en $\real^3$ parametrizada: $S = \{\Phi(u,v) = (x(u,v),y(u,v),z(u,v))\}$.
A la hora de trabajar con superficies parametrizadas, nos interesaría poder definir una especie de función inversa que nos permita hacer cambios en el plano y llevarlos a la superficie o al reves, pero... ¡tienen dimensiones distintas! La esperanza que nos queda es que la superficie parametrizada tiene dimensión 2, igual que el plano.
\begin{defn}[Homeomorfismo] \label{defHomeomorfismo}
Sea $\appl{\Phi}{\Omega\subset\real^N}{\real^{N+K}}, \Omega$ abierto.
$\Phi$ es un \emph{homeomorfismo} sobre su imagen $\dimplies $ la restricción $\appl{\Phi}{\Omega}{\Phi(\Omega)}$ es continua y tiene una inversa continua,
es decir, \[\exists \appl{\Psi}{\Phi(\Omega)}{\Omega} \tlq
\left\{ \begin{array}{cc}
\Psi(\Phi(\gor{u})) = \gor{u}, &\forall \gor{u} \in \Omega\\
\Psi(\Phi(\gor{x})) = \gx, &\forall \gx \in \Phi(\Omega)
\end{array}\right.\]
\paragraph{Definición 1)}
Dado un $\displaystyle x_0 \in \Phi(\Omega) \implies \forall \varepsilon >0, \exists \delta>0 \tlq$
si $\begin{array}{lc}
\norm{\gx-\gor{x_0})} < \delta \implies \norm{\Psi(\gx)-\Psi(\gor{x_0})}<\varepsilon\\
\gx \in \Phi(\Omega)
\end{array}$
\paragraph{Definición alternativa de continuidad}
Si $\{X_n\}\subset\Phi(\Omega), \gor{X_n} \rightarrow \gor{x_0}\in\Phi(\Omega) \implies \Psi(\gor{X_n}) \rightarrow \Psi(\gor{x_0})$
\end{defn}
\subsubsection{Ejemplos}
\paragraph{Ejemplo 1}
\[\appl{\sigma}{[0,2\pi)}{\real^2}\]
\[t \rightarrow \sigma(t) = (cos(t),sen(t))\]
Inversa: $\Psi(x,y) = t$ ángulo de la representación en polares.
Vamos a estudiar el problema de la continuidad:
Tomamos $\{(X_n,Y_n)\}$ con $x^2+y^2 = 1 \tlq (x_n,y_n) \convs (1,0)$
Si $\Psi$ es continua, debe ser $\Psi(x_n,y_n) \convs (1,0) = 0$. En este caso no es continua porque:
Si tomamos \begin{align*}
P_n &= \left(cos\left(2\pi - \frac{1}{n}\right), sen\left(2\pi - \frac{1}{n}\right) \right)\\
P_n &\convs (1,0)\\
\Psi(P_n) &= 2\pi - \frac{1}{n} \convs 2\pi\neq\Psi(1,0)
\end{align*}
\paragraph{Ejemplo 2}
\[\appl{f}{(0,1)\subset\real}{\real^2}\]
\[t \rightarrow f(t) = (t,g(t)), \text{continua, con inversa continua}\]
Vamos a definir la  inversa:
\[P\in f(0,1) \implies P(x,g(x)) \text{Para algún } x\in(0,1)\]
$P = (x,g(x))$
\[\Psi(P) = t \in (0,1) \tlq f(t) = (x,g(x)) \implies t = x\]
Vamos a estudiar la continuidad:
\[\{P_n\} \subset f(0,1), P_n \rightarrow P \in f(0,1)\]
\[P_i = (x_i,g(x_i)), \text{ para algún } i \in (0,1)\]
\[P_n \convs P_0 \dimplies (x_n,g(x_n)) \rightarrow (x_0,g(x_0)) \implies x_n (= \Psi(P_n)) \rightarrow x_0 (=\Psi(P_0)) \]
\obs ¿La gráfica de una función es homeomorfismo sobre su imagen?
\paragraph{Ejemplo 3}
\[\appl{\sigma_3}{(0,4\pi)}{\real^2}\]
\[t \rightarrow \sigma(t) = (cos(t),sen(t))\]
No es inyectiva $\implies \nexists \Psi$.
\paragraph{Ejemplo 4: Circunferencia}
\[\appl{\sigma_4)}{(0,2\pi)}{\real^2}\]
\[t \rightarrow \sigma(t) = (cos(t),sen(t))\]
La diferencia con el ejemplo 1, es que es cerrado.
Hay que percatarse de que la tangente no es inyectiva, entonces... la inversa es algo más complicada que $\arctan$, así que vamos a definirla a trozos siguiendo el esquema de la figura \ref{imgCirc_2}.
\begin{figure}[hbtp]
\begin{center}
\begin{tikzpicture}[scale=1]
% Ejes
\draw[->] (-3,0) -- (3,0);
\draw[->] (0,-3) -- (0,3);
% Partes de la circunferencia
\draw[very thick,red] (2,0) arc (0:90:2);
\draw[very thick,blue] (0,2) arc (90:270:2);
\draw[very thick,green] (0,-2) arc(270:360:2);
% Etiquetas
\node[red] at (1.7, 1.7) {(1)};
\node[blue] at (-2.3, 0.3) {(2)};
\node[green] at (1.7, -1.7) {(3)};
\end{tikzpicture}
\caption{Circunferencia definida en tres trozos}
\label{imgCirc_2}
\end{center}
\end{figure}
\[\Psi(x,y) =
\begin{cases}
\arctan\left(\frac{y}{x}\right) & (x,y)\in 1\\
\arctan\left(\frac{y}{x}\right) + \pi & (x,y) \in 2\\
\arctan\left(\frac{y}{x}\right)+2\pi& (x,y) \in 3
\end{cases}
\]
Hay que estudiar la continuidad en $(0,-1)$ y en $(0,1)$.
\subparagraph{Continuidad en (0,1)}
Tomamos $\{P_n\} \rightarrow (0,1), P_n \in S_1$
Queremos probar que $\Psi(P_n) \rightarrow \Psi(0,1) = \frac{\pi}{2}$.
Ejercicio para el lector:
Sucesiones que se acercan por la derecha o por la izquierda y comprobar que vale lo que tiene que valer.
\paragraph{Ejemplo 5: Lemniscata}
\begin{figure}[hbtp]
\begin{center}
\begin{tikzpicture}[scale=2,declare function={
	lemnx(\x)=2.5*cos(\x) / ( sin(\x)^2+ 1);
	lemny(\x)=3*sin(\x) * cos(\x) / ( sin(\x) ^2 + 1;
	}]
% Ejes
\draw[->] (-3,0) -- (3,0);
\draw[->] (0,-2) -- (0,2);
% La curva
\draw[gray,domain=-90:270,samples=200] plot ({lemnx(\x)}, {lemny(\x)});
% Sucesión 1
\foreach \x in {-86,-82,...,-66}
\node[circle, red, draw,inner sep=2pt] at ({lemnx(\x)}, {lemny(\x)}) {};
% Sucesión 2
\foreach \x in {72,76,...,108}
\node[rectangle, blue, draw,inner sep=2pt] at ({lemnx(\x)}, {lemny(\x)}) {};
% Sucesión 3
\foreach \x in {242,246,...,266}
\node[diamond, orange, draw,inner sep=2pt] at ({lemnx(\x)}, {lemny(\x)}) {};
% Puntos t = 0, t=π
\node[label=above right:$t\eq 0$, draw, fill=white,circle, inner sep=2pt] at (2.5,0) {};
\node[label=above left:$t\eq \pi$, draw, fill=white,circle, inner sep=2pt] at (-2.5,0){};
% Flechas para indicar hacia donde va la t.
\foreach \x in {-45,44,134,224}
\draw[-angle 90] ({lemnx(\x)},{lemny(\x)}) -- ({lemnx(\x + 1)},{lemny(\x +1)});
% Etiquetas de las sucesiones.
\node[label={[red]below:(1)}] at ({lemnx(-66)},{lemny(-66)}) {};
\node[label={[blue]above:(2)}] at ({lemnx(72)},{lemny(72)}) {};
\node[label={[orange]above:(3)}] at ({lemnx(242)},{lemny(242)}) {};
\end{tikzpicture}
\caption{Curva Lemniscata}
\end{center}
\end{figure}
La parametrización es \[\sigma_5 (x(t),y(t)) = \left(\frac{\cos(t)}{\sin^2(t)+1},\frac{\sin(t)\cos(t)}{\sin^2(t)+1}\right), t\in \left(\frac{-\pi}{2},\frac{3\pi}{2}\right)\]
Al origen podemos acercarnos de distintas formas:
\begin{itemize}
\item Cuando $t \to - \frac{\pi}{2}$, nos acercamos por la sucesión 1 (desde abajo a la derecha).
\item Cuando $t \sim \frac{\pi}{2}$, nos acercamos por la sucesión 2 (la mitad de la curva, de arriba-derecha a abajo-izquierda).
\item Cuando $t \to \frac{3\pi}{2}$, nos acercamos por la sucesión 3 (desde arriba a la izquierda)
\end{itemize}
Sea $\{P_n\}\subset \sigma_5(t) \rightarrow (0,0)$.
Podemos tomar la sucesión $\{P_n\} = \{P_1,P_2,P_3,...\}$ cada uno en una región (1,2,3 ciclicamente).
\[\Psi(P_n) \begin{cases}
\in 3 & \text{ si }n \text{ es múltiplo de }3\\
\in 2 & \text{ si } n\equiv 2\ mod \ 3\\
\in 1 & \text{ si } n \equiv 1\ mod \ 3
\end{cases}\]
Por tanto $\nexists \displaystyle \lim_{n\rightarrow \infty} \Psi(P_n)$
\begin{remark} A pesar de que hemos demostrado que $\sigma$ es continua e inyectiva, esto no garantiza que la inversa sea continua.\end{remark}
\subsection{Parametrizaciones}
\paragraph{Objetivo} definir "parametrización".
\subparagraph{Ejemplo 1} Curva parametrizada en $\real^3$
$\Gamma = \{\sigma(t) = (x(t),y(t),z(t)), t \in (a,b)\}$
Queremos excluir:
\begin{itemize}
\item Picos (valor absoluto. FOTO)
Basta con imponer: $\sigma \in C^1 \y (x',y',z') \neq (0,0,0)$
\item Auto-intersecciones o Lemniscata (que no se auto-intersecciona pero por poquito)
Basta imponer $\sigma$ sea un homeomorfismo sobre su imagen.
\end{itemize}
\paragraph{Ejemplo 2} Superficies de parametrización en $\real^3$.
\[S = \{\Phi(u,v) = (x(u,v),y(u,v),z(u,v)), (u,v)\in D\}\]
Queremos evitar:
\begin{itemize}
\item Cono, tienda de campaña
$Rango \begin{pmatrix}
T_u \rightarrow\\
T_v \rightarrow
\end{pmatrix} = 2 \implies $ Podemos calcular plano tangente
\item Autointersección
Aquí sí tenemos rango máximo, asíque impondremos la condición de homeomorfismo sobre su imagen.
\end{itemize}
Ya tenemos todo lo necesario para definir parametrización:
\begin{defn}[Parametrización\IS local] \label{defParametrizacion}
Diremos que $\appl{\Psi}{\omega \subset \real^N}{\real^{N+K}}, \Psi \in C^1(\omega)$, es una parametrización local $\dimplies \left\{ \begin{array}{c}
 rango D\Psi = n \text{ máximo}\\
 \Psi \text{ es un homeomorfismo sobre su imagen}
\end{array}\right.$
\end{defn}
\subsubsection{Repaso de coordenadas cilíndricas y esféricas.}
\input{CALII/repaso_coordenadas.tex}
\subsubsection{Ejemplos}
\subparagraph{Esfera en $\real^3$}
$\Phi_{1,2}(x,y) = (x,y,\pm \sqrt{1-x^2-y^2})$. Esta \emph{"carta de parametrización"} nos deja sin definir el ecuador. Para ello tenemos que definir más \emph{cartas de parametrización} \index{Carta!de parametrización}
 Estas cartas son expresando x,y en función de las otras 2. En total hacen falta 3 parametrizaciones.
\subparagraph{Existe} otra manera de parametrizar, la proyección estereográfica.
\index{Proyección\IS estereográfica}
El dibujo de la proyección es:
\input{tikz/ProyeccionEstereografica.tex}
\[(u,v) \in \real^2 \rightarrow (u,v,0) \rightarrow r\equiv (0,0,R) + t(u,v,-R) = (tu,tv,R(1-t)\]
 Imponiendo $\underbrace{P}_{r(t_0)} \equiv r\cap S$ tenemos: \[(t_0u)^2+(t_0v)^2 + R^2(1-t)^2 = R^2 \rightarrow ... \rightarrow t_0 = \frac{2R^2}{u^2+v^2+R^2}\]
 Conclusión: \[P = (tu,tv,R(1-t) = \frac{2R^2}{u^2+v^2+R^2}u,\frac{2R^2}{u^2+v^2+R^2}v,\frac{R(u^2+v^2-R^2)}{u^2+v^2+R^2} = \Phi(u,v)\].
 Vemos que $\Phi\in C^1, \Phi(\real^2) = S_R-\{(0,0,R)\}$ ¿Es una parametrización?
 Hay que comprobar \begin{itemize}
\item rango $D\Phi$ máximo. (Se deja como ejercicio para el lector)
\item $\Phi$ es homeomorfismo sobre su imagen, es decir, ¿Existe una inversa continua?
\emph{Inversa}
 Dado $(x,y,z)$ queremos despejar $(u,v)$.
 Idea: $(u,v,0)$ es la intersección de la recta que unie $(x,y,z)$ con $(0,0,R)$ y el plano $z=0$.
 Recta: $s(t) = (tx,ty,R+t(z-R))$.
 Punto de corte con el plano $z=0$: El punto de corte tendrá coordenada tercera = 0, es decir:
$R+t(z-R)$
 Buscamos $t_0$ tal que $R+t_0(z-R)=0 \dimplies t_0=\frac{R}{R-z}$.
 Sustituyendo en la recta obtenemos: $u = t_0x, v=t_0y$
 Si calculamos $\Phi^{-1}(x,y,z) = \left(\frac{Rx}{R-z},\frac{Ry}{R-z}\right)$. Esta inversa es continua en $Img(\Phi(\real^2)) \equiv \{Esfera - \{(0,0,R)\}\}$  (El punto (0,0,R) no está incluido, por definición, en la imagen).
\end{itemize}
\subsection{Teoremas de las subvariedades}
\begin{theorem}\label{thmSubvariedades}
Los siguientes enunciados son equivalentes:
\begin{itemize}
\item[1] $M$ es una subvariedad diferenciable n-dimensional en $\real^{N+K}$. \label{eq_1}
\item[2] $\forall \gor{a} \in M $ existe una parametrización local $\appl{\Phi}{\omega\subset \real^N}{\real^{N+K}}$ con $\gor{a}\in \Phi(\omega)$\label{eq_2}
\item[3] $\forall \gor{a} \in M$ existe un abierto $V\subset \real^{N+K}, \gor{a}\in V$ y una aplicación
\label{eq_3}
\[\appl{\Psi}{V}{\real^{N+K}}, \Psi\ \text{un difeomorfismo} \tlq \Psi = (\Psi_1,...,\Psi_n,\Psi_{n+1},...,\Psi_{n+k})\]
Si $\gx \in V\cap M \implies$
\[\Psi_{n+1}(\gx) = ... = \Psi_{n+k}(\gx) = 0\]
\end{itemize}
\end{theorem}
\paragraph{Observación 1:} En \ref{eq_2}.2, llamaremos \textbf{carta local}\index{Carta!local} al conjunto definido por la fórmula y el dominio, $(\Phi,\omega)$. El conjunto de todas las cartas locales que definen una subvariedad se llama Atlas.
\subparagraph{Ejemplo:}
 La proyección estereográfica tiene 2 cartas, la del polo norte (que excluye ese punto) y la del polo sur.
\paragraph{Observación 2:} $\ref{eq_1}.1 \dimplies \ref{eq_2}.2$. Si tenemos una subvariedad dada como conjunto de nivel la podemos parametrizar (y viceversa).
\begin{defn}[Difeomorfismo]
$\Psi$ es un difeomorfismo $\dimplies \Psi\in C^1,\exists \Psi^{-1}, \tlq \Psi^{-1}\in C^1$
\end{defn}
\begin{proof}
Esquema: $1\implies 2, 2\implies 3, 3 \implies 1$
\paragraph{1 $\implies$ 2\\}
Sea $\ga \in M, \exists U\subset\real^{N+K}$ abierto con $\ga \in U$ y una función $\appl{F}{U\subset \rnk}{\rk}, F\in C^1(U), \tlq U\cap M = \{\gx \in U\tq F(\gx) = \gor{0}\}$. Además $DF$ tiene rango máximo (K).
Queremos demostrar que existe una parametrización $\Phi$.
\subparagraph{Permutando} el orden de las variables, suponemos que el menor de orden $K$ con determinante no nulo corresponde con las $K$ últimas variables.
Por el teorema de la función implícita, $F(x_1,...,x_n,x_{n+1},...,x_{n+k}) = \gor{0}$, con $x_{n+1},...,x_{n+k}$ despejable en función de las $\{x_i,i=1,...,n\}$ en un entonro de $\gor{a}$.
Es decir: existen $\omega\subset \real^N, \omega'\subset\rk$ abiertos tales que $\gor{a}\in \omega \times \omega'$ y una función $\appl{g}{\omega\subset\real^N}{\omega'\subset\rk}$ de manera que
$$\left\{\begin{array}{c}
g(a_1,...,a_n) = (a_{n+1},...,a_{n+k})\\
F(\gx,g(\gx)) = \gor{0}, \forall \gx \in \omega\end{array}\right.$$
Idea: la parametrización es $\Phi (\gx) = (\gx,g(\gx))$
Vamos a comprobar las condiciones:
\begin{itemize}
\item $\Phi \in C^1$. Por el teorema de la función implícita, tenemos que $\Phi$ es diferenciable (porque $F$ y $g$ lo son).
\item \[D\Phi = ... =
\begin{pmatrix}
Id_{n \times n}\\
\hline
Dg
\end{pmatrix}\] con rango máximo.
\item ¿Homeomorfismo sobre su imagen? $(x,y)\in M$ en un entorno de $\ga \in \omega\times\omega'$ En ese entonrno $y=g(\gx)$.
\end{itemize}
Es decir, $(x,y) = (x,g(x)) \xrightarrow{\Phi}) \gx \xrightarrow{\Phi^{-1}} (x,g(x)) = (x,y) $. También $\inv{\Phi}(x,y) = x, \forall(x,y)\in (\omega\times\omega') \cap M$ Continua.
\paragraph{2 $\implies$ 3} Vamos a emplear un argumento como el de la demostración del segundo teorema del rango. \ref{TR2}
Buscamos:
\begin{align*}
\appl{\Phi}{\rnk}{\rnk} \tlq \Phi(V\cap M) = (\ast &,0)\\
&\uparrow\\
k \text{ últimas coor} & \text{denadas}
\end{align*}
Siendo $\Phi$ un difeomorfismo.
\paragraph{Sabemos:} existe una parametrización local $\appl{\Psi}{\real^N}{\rnk}$.
\begin{itemize}
\item $D\Psi$ rango máximo.
\item $\Psi$ homeomorfismo sobre su imagen.
\end{itemize}
\subparagraph{Idea:} Completar el número de variables
Definimos
\begin{align*}
\appl{\alpha}{\omega\times\real^K \subset \real^N\times\real^K}&{\real^N\times\real^K}\\
(\gor{u},\gor{v})\longrightarrow &\alpha(\gor{u},\gor{v}) = \Psi(\gor{u}) + (\gor{0},\gor{v})\\
\gor{u} \in \real^N,\gor{v} \in \real^K, \Phi(\gor{u})\in \real^{N+K}
\end{align*}
\paragraph{Paso 2)} Aplicar el teorema de la función inversa (\ref{thmInv}) a $\alpha$.
\[D\alpha =
\left(
\begin{array}{c|c}
		D\Psi_k  \rightarrow & 0\\
\hline
		D\Psi_{n+i}  \rightarrow & I
\end{array}
\right)
\]
Con $1\leq i \leq k,1\leq k \leq n$.
Por hipótesis, $\mop{rango} (D\Psi)$ máximo. $\implies \exists \alpha^{-1}$.
\paragraph{Paso 3:} Comprobar que $\inv{\alpha}$ verifica las condiciones que buscamos.
Podría darse el caso de que en el conjunto $V\cap M$ hubiera 2 "trozos" de la subvariedad M, con lo que $\alpha$ no funcionaría bien. La condición de la parametrización eliminaba este caso.
Falta comprobar la condición de difeomorfismo, que se da porque... ¿porqué?
\paragraph{3 $\implies$ 1}
\textbf{Sabemos:} Existe un difeomorfismo $\Psi$.
\textbf{Buscamos:} $\appl{F}{W\subset \rnk}{\real^K} \tlq \displaystyle \left\{\begin{array}{c}
M\cap W = \{F(\gx) = \gor{0}\}\\
rango(DF) = k \text{ (máximo)}
\end{array}\right.$
Tomamos $F(\gx) = (\Psi_{n+1}(\gx),...,\Psi_{n+k}(\gx))$
Entonces: $M\cap V = \{ \gx \tq F(\gx) = \gor{0}$.
Tenemos $DF = \begin{pmatrix}
D\Psi_{n+1} \rightarrow\\
\vdots\\
D\Psi_{n+k} \rightarrow
\end{pmatrix}$
$Rango(DF) = k$ por tener $\det D\Psi \neq 0$ por hipótesis.
\end{proof}
\paragraph{Consecuencias:}
\subparagraph{1)}
Si $M$ es una variedad diferenciable de dimensión $N$ en $\rnk$, entonces, reordenando las variables puede escribirse \textbf{localmente} como la gráfica de una función $C^1, \underbrace{M\cap U}_{(*)} = \{(\gx,g(\gx))\}$
$(*) \implies$ un trozo de la variedad.
\subparagraph{2)}
\begin{theorem}
Sea  $\appl{\gamma}{\omega\subset\real^N}{\rnk}, \gamma \in C^1, rg(D\gamma) = max, \gamma(\omega)\subset M$ subvariedad de dim n.
\textbf{Entonces:} $\gamma$ es una parametrización local.
\end{theorem}
\textbf{Aplicación:} Si existe $\gamma \in C^1, rg(D\gamma) = n, \gamma(\omega)\subset M \ y \ \gamma
$ no es homeomorfismo sobre su imagen $\implies$ \textbf{M} no es subvariedad.
Pregunta: Verdadero o Falso:
¿Con encontrar una aplicación que no sea homeomorfismo basta para asegurar que M no es subvariedad?
\paragraph{3)\\}
La prueba de este teorema se deja como ejercicio para el lector.
\begin{theorem}
Sea M subvariedad diferenciable n-dimensional en $\rnk$.
Sean $\appl{\Phi_1}{U_1}{M} \ y \ \appl{\Phi_2}{U_2}{M}$ dos parametrizaciones locales con $\Phi_1(U_1)\cap \Phi_2(U_2)\neq \emptyset$
\textbf{Entonces:} $\appl{\inv{\Phi_1}\circ \Phi_2}{\real^N}{\real^N}, con \inv{\Phi_1}\circ \Phi_2 \in C^1$. Análogamente para $\inv{\Phi_2}\circ\Phi_1$
\end{theorem}
\section{Espacios tangentes}
Sea $M$ subvariedad n-dimensional en $\rnk$.
$T_{\gor{a}}M \leadsto$ espacio tangente a M en el punto $\gor{a}\in M$
Pero... ¿qué es un hiperplano tangente? El concepto no es tan simple como un plano tangente. El espacio tangente será el conjunto de todos los vectores tangentes a cada una de las curvas contenidas en la superficie. A partir de aquí buscaremos una forma más eficiente de construirlo (porque es imposible calcular todas y cada una de las curvas contenidas en la superficie).
\begin{defn}[Vector\IS tangente]
Si $\gx \in \rnk$ es tangente a M en $\gor{A} \in M \dimplies \exists \appl{\sigma}{(-1,1)}{\rnk}, \sigma \tlq \left\{\begin{array}{lc}
\sigma(t) \in M, \forall t\in (-1,1)\\
\sigma(0) = \gor{a}\\
\alpha'(0) = \gor{v}
\end{array}\right.$
\end{defn}
\begin{defn}[Espacio\IS tangente]
\[T_aM \equiv \{ \gor{v} \in \rnk \tq \gor{v} \text{ es tangente a M en }\gor{a}\}\]
\end{defn}
\obs Cualquier curva de la variedad la podremos ver como una curva en la proyección (con una parametriazación construida cuidadosamente)
\begin{theorem}
Sea $M$ subvariedad en $\real^M$, $N$ subvariedad en $\real^N$.
\[\appl{f}{\Omega\subset\real^M}{\real^N}, \tlq f(\Omega\cap M) \subset N, f\in C^1\]
Sea \[\left.\begin{array}{lc}
\gor{a} \in \Omega\cap M \\
\gor{v} \in T_aM
\end{array}\right\}
\implies Df(\gor{a})\gor{v} \in T_{f(\ga)}N\]
\end{theorem}
Es decir, si tenemos una parametrización, la diferencial lleva tangentes en tangentes.
\begin{proof}
Sea $\gor{v} \in T_{\ga} M$
Entonces $\exists \appl{\alpha}{(-1,1)}{M} \tlq \left\{\begin{array}{c}
\alpha(0) = \ga\\
\alpha'(0) = \gor{v}
\end{array}\right.$
Tomamos $\beta = f \circ \alpha$ curva sobre $N$
tal que $\left\{\begin{array}{lc} \beta(0) = f(\alpha(0)) = f(\ga)\\
\beta'(0) = Df(\alpha(0))\cdot \alpha'(0) = Df(\ga)\gor{v}\end{array}\right.$ (Aplicando la regla de la cadena sin más.)
\end{proof}
\subsection{Caracterizaciones del espacio tangente}
\textbf{Caracterización 1)}
\begin{theorem}\label{thmCaractTangente1}
$M$ subvariedad n-dimensional en $\rnk$. $\ga \in M$
Entonces:
\begin{itemize}
\item $T_{\ga}M$ es un espacio vectorial n-dimensional
\item $M$ definida como $\{F = 0\}$. Entonces $T_{\ga} M = \ker(DF(\ga))$
\end{itemize}
\end{theorem}
\begin{proof}
$U\cap M =\{ \gx \in \rnk \tq F(\gx) = \gor{0}\}$ para alguna $\appl{F}{\rnk}{\real^N}, rg(DF) = max$
\[\appl{F}{U\cap M}{\gor{0}}\]
Entonces: $DF(\ga)$ lleva $T_a M$ al espacio $T_0\{\gor{0}\}$
Es decir: $DF(\ga)\gor{v} = \gor{0}, \forall \gor{v}\in T_{\ga} M$
Esto demuestra $T_{\ga} M \subset \ker DF(\ga)$
Como el rango es máximo, sabemos que $\ker(DF(\ga))$ tiene dimensión $n$.
La idea a aplicar es encontrar $n$ vectores independientes en ese espacio tangente ¿Cómo vamos a encontrarlos? En el espacio de los parámetros tenemos n rectas independientes (los n ejes de coordenadas)
La parametrización nos lleva esas $n$ rectas en $n$ curvas.
Por el teorema anterior, la diferencial lleva tangentes en tangentes, es decir, aplicando la diferencial a los vectores directores de las $n$ rectas encontramos los vectores tangentes a las $n$ curvas.
¿Cómo podemos saber que esos vectores son independientes? Porque la diferencial tiene rango $n$.
Acabamos de demostrar  $\ker DF(\ga) \subset $\{ espacio vectorial de dimensión n\}
Si $T_{\ga} M$ contiene un espacio vectorial de dimensión $n$ y está contenido por el núcleo (espacio vectorial de dimensión $n$).
\end{proof}
\paragraph{Caracterización 2)}
\begin{corol}
\label{CaractSubv_2}
$M$ dada por una parametrización $\Phi$ tal que $\Phi(\gor{u_0}) = \ga$
Entonces $T_{\ga} M = \img D\Phi(\gor{u_0})$
\end{corol}
El teorema y el corolario son las 2 caracterizaciones del espacio tangente.
Pero también podemos definir el espacio tangente con una tercera caracterización:
\paragraph{Caracterización 3)} Como gráfica. Sea $\appl{f}{\real^N}{\real^{K}}$
\[M\equiv \left\{(\gu,f(\gu)),\begin{matrix}
(\gu,f(\gu))\in \rnk\\
\gu \in \Omega\subset\real^N\\
\appl{f}{\real^N}{\real^K}\end{matrix}\right\} \]
Salvo reordenación de las variables.
Sea $p=(\ga,f(\ga))$ el punto en el que queremos calcular el hiperplano tangente a $M$.
La caracterización será
\[T_p(M) = \{(\gu,v)\in\real^N\x\real^{K} \tq v = Df(a) \gu\}\]
\obs la otra alternativa es definir la subvariedad como $M = \{(\gu)\in\real^k \tq f(\gu) = f(\ga)$
\begin{defn}
$M\subset\rnk$ subvariedad n-dimensional, $\ga \in M$
\begin{itemize}
\item Espacio tangente $T_{\ga}M$
\item Hiperplano tangente $T_{\ga}$ "trasladado" al punto $\ga$
\[\{\gx \in \rnk \tq \gx-\ga \in T_{\ga}M\}\]
\item Hiperplano normal $\equiv \{\gx\in\rnk \tq \gx -\ga \in (T_{\ga}M)^{\bot}\} = \{\gx \in \rnk \tq \pesc{\gx-\gor{a},\gor{v}} = 0, \forall \gor{v}\in T_{\ga}M\}$. El hiperplano normal es k-dimensional.
\end{itemize}
\end{defn}
\paragraph{Ejemplos:}
\subparagraph{1)}
$ M = \{(x,y) \in \real^2 \tq x^2+y^2 = 1\}$.
\textit{Comprobación previa} Es una subvariedad porque...
Vamos a calcular \[T_{(a,b)}M = \ker \{\begin{pmatrix} 2x & 2y \end{pmatrix}\} =\]
\[ \{(u,v) \tq \begin{pmatrix}
2a & 2b
\end{pmatrix}\begin{pmatrix}
u\\v
\end{pmatrix} = 0\} = ... =  \{(u,v)\in \real^2 \tq \pesc{(a-0,b-0),(a,b)-(u,v)} = 0\].
El espacio tangente es el formado por todos los vectores perpendiculares al radio.
\subparagraph{Ejemplo 2: Toro (donut) en $\real^4$}
\[M = \{ (x,y,z,t)\in \real^4 \tq x^2+y^2 = 1, z^2+t^2 = 1\}\]
Vamos a calcular: $T_{(1,0,0,1)}M$
\textbf{Comprobación previa}...
Tenemos definida la variedad de forma implícita: $M = \{F = 0\}$ donde \[F(x,y,z,t) = (x^2+y^2-1,t^2+z^2-1)\]
\[DF = \begin{pmatrix}
2x&2y&0&0\\
0&0&2z&2t
\end{pmatrix}\]
En este caso tenemos $rg(DF) = 2, \forall (x,y,z,t)\in \real^4$. (El único punto que podría dar rango 0 es el origen, que en este caso no pertenece a la subvariedad)
Vamos con el espacio tangente:
\[T_{(1,0,0,1)}M = \ker DF (1,0,0,1) = \ker \begin{pmatrix}
2&0&0&0\\
0&0&0&2
\end{pmatrix} =\]
\[ \{ (\alpha_1,\alpha_2,\alpha_3,\alpha_4) \in \real^4 \tq \begin{pmatrix}
2&0&0&0\\
0&0&0&2
\end{pmatrix} \begin{pmatrix}
\alpha_1\\
\alpha_2\\ \alpha_3\\ \alpha_4
\end{pmatrix} = \begin{pmatrix}
0 \\
0
\end{pmatrix}\} \implies \left\{\begin{array}{cc}2\alpha_1 &= 0\\ 2\alpha_4 & =0\end{array}\right.\]
Hiperplano tangente:
\[
\begin{pmatrix}
1\\0\\0\\1
\end{pmatrix}
+ \alpha_2 \begin{pmatrix}
0\\1\\0\\0
\end{pmatrix}
+ \alpha_3
\begin{pmatrix}
0\\0\\1\\0
\end{pmatrix}, \alpha_2,\alpha_3 \in \real
\]
Y el hiperplano normal:
\[
\begin{pmatrix}
1\\0\\0\\1
\end{pmatrix}
+ \mu \begin{pmatrix}
1\\0 \\0\\0
\end{pmatrix}
+
\lambda
\begin{pmatrix}
0\\0\\0\\1
\end{pmatrix}, \lambda,\mu \in \real
\]
¿Una posible parametrización de esto?
\begin{align*}
\Phi : D \subset \real^2 \longrightarrow &\real^4\\
(u,v) \longrightarrow &\Phi(u,v) = (x,y,z,t) = \left(cos(u),sen(u),cos(v),sen(v)\right)\\
(u,v)\in (-\pi,\pi)\times(0,2\pi)
\end{align*}
¿¿Por qué $(u,v)\in (-\pi,\pi)\times(0,2\pi)$ y no $(u,v)\in (0,2\pi)\times(0,2\pi)$??
Porque el punto que tenemos $(1,0,0,1) \notin \img$.
Vamos a calcular la el hiperplano tangente. Como tenemos una parametrización, calcularemos la imagen de la diferencial (\ref{CaractSubv_2})
\[T_{(1,0,0,1)}M = \img D\Phi\left(0,\frac{\pi}{2}\right)\]
\[D\Phi = \begin{pmatrix}
-sen(u) & 0\\
cos(u) & 0\\
0 & -sen(v)\\
0&cos(v)
\end{pmatrix}\]
\[D\Phi\left(0,\frac{\pi}{2}\right) = \begin{pmatrix}
0&0\\1&0\\0&-1\\0&0
\end{pmatrix}\]
Entonces el hiperplano tangente es:
\[\begin{pmatrix}
1\\0\\0\\1
\end{pmatrix} + u \begin{pmatrix}
0\\1\\0\\0
\end{pmatrix}
- v \begin{pmatrix}
0\\0\\1\\0
\end{pmatrix}
\]
Lógico y normal que nos de el mismo hiperplano tangente si estamos trabajando con el mismo objeto (desde una parametrización o desde un conjunto de nivel). ¿Cierto y verdad que sí?
\paragraph{Ejemplo 3: El toro en $\real^3$}
\index{Toro}
El \textbf{toro} (una especie de flotador) se produce al girar una circunferencia de radio $R_1$ en el plano $XZ$ con el centro sobre el eje $X$ a $R_2$ del origen alrededor del eje $Z$.
\[ \Phi(\theta, \phi) = ((R_2+R_1\cos\phi)\cos\theta,(R_2+R_1\cos\phi)\sin \theta,R1\sin \phi)\;\; \theta, \phi \in (0, 2\pi) \]
\easyimg{CALII/Toro.png}{Toro}{lblToro2}
¿Es $\Phi$ una parametrización?
\begin{itemize}
\item Opción 1: Comprobar homeomorfismo sobre la imagen
\item Opción 2: Aplicar el teorema. Si el toro es una subvariedad $\implies \Phi$ parametrización.
\end{itemize}
Vamos con la opción 1:
\[\Phi(\alpha,\theta) = (x,y,z)\]
\[¿(\alpha,\theta) = \Phi^{-1} (x,y,z)?\]
\[z = rsen(\alpha) \implies \alpha = arcsen\left(\frac{z}{r}\right)\]
\[\frac{y}{x} = tg(\theta) \implies \theta = arctg \left(\frac{y}{x}\right)\]
%Revisar
Esto no es suficiente, porque $\appl{arcsen}{(-1,1)}{\left(\frac{-\pi}{2},\frac{\pi}{2}\right)}$ no toma todos los posibles valores. Lo mismo con la $\appl{arctg}{\real}{\left(\frac{-\pi}{2},\frac{\pi}{2}\right)}$
Tenemos que repetir el argumento de (\ref{imgCirc}) que ya hemos hecho para la $arctg$ vamos a repetirlo para el $arcsen$.
\begin{figure}[hbtp]
\begin{center}
\begin{tikzpicture}[scale=1]
% Ejes
\draw[->] (-3,0) -- (3,0);
\draw[->] (0,-3) -- (0,3);
% Partes de la circunferencia
\draw[very thick,red] (2,0) arc (0:90:2);
\draw[very thick,blue] (0,2) arc (90:270:2);
\draw[very thick,green] (0,-2) arc(270:360:2);
% Etiquetas
\node[red] at (1.7, 1.7) {(1)};
\node[blue] at (-2.3, 0.3) {(2)};
\node[green] at (1.7, -1.7) {(3)};
\end{tikzpicture}
\caption{Circunferencia definida en tres trozos}
\label{imgCirc}
\end{center}
\end{figure}
\[f(x,y,z) =\left\{ \begin{matrix}
Si & (x,y,z) \in 1 &\implies &\arcsin\left(\frac{z}{r}\right)\\
Si & (x,y,z) \in 2 &\implies &\displaystyle\frac{\alpha + \arcsin\left(\frac{z}{r}\right)}{2} = \frac{\pi}{2}\\
Si & (x,y,z) \in 3 &\implies & \alpha = \arcsin\left(\frac{z}{r}\right) + 2\pi
\end{matrix}\right.
\]
Ahora tenemos que estudiar la continuidad des esta función. (Ejercicio para el lector)
\subparagraph{$T_{\ga}M$}
En este caso (al tratarse de una diferencial) tendremos que hallar la imagen de $D\Phi$.
Ejercicio propuesto: $T_{\left(\frac{\pi}{2},\frac{\pi}{2}\right)}M$.
\begin{problem}[4.4]
Sea $\sigma(t) = \left(\cos t,\sen t,t^2(2\pi - t)^2\right), t \in [0,2\pi]$.
\solution
Siempre hemos hablado de parametrizaciones es espacios abiertos, para asegurar la condición de homeomorfismo en casos como este, en el que los puntos cerca de $0$, la inversa me los lleva a puntos lejanos si nos acercamos a $0$ por el $0$ o por el $2\pi$.
Posibles soluciones
\begin{itemize}
\item  Trabajar con el intervalo abierto, pero entonces... el punto $(1,0,0)$ que es el que nos piden no pertenece. ¿Cómo calcular el espacio tangente en $(1,0,0)$? Podríamos hacer los "límites laterales" y calcular el $T_{(1^{-},0,0)}M, T_{(1^{+},0,0)}$ por decirlo de alguna manera y si coinciden, ese tiene que ser el hiperplano tangente en el punto $(1,0,0)$.
\item Definir otro intervalo en el que trabajar.
Con el $sen$ y $cos$ no tenemos problema porque son periódicas y podríamos trabajar en $\left(\frac{\pi}{2},\frac{\pi}{2}\right)$ pero con la tercera coordenada es más problemático porque no es periódica. Es de la forma:
%\easyimg{imgs/TercCoor.png}{TercCoor}{lblTercCoor}
Idea:
\begin{itemize}
\item Escribir la extensión $2\pi$ periódica al intervalo $[-2\pi,2\pi]$.
\item Tomar $\tilde{\sigma}(t) = (cos(t),sen(t),\tilde{z}(t)), t\in (-\pi,\pi)$
\end{itemize}
\end{itemize}

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
aleatoria $X$. En esta seccion trabajaremos sobre el espacio de
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
Las $\sigma$-algebras minimales independientes sobre clases
independientes cerradas para la intersección finita son independientes
\end{theorem}
Esto tiene tres aplicaciones fundamentales:
\begin{enumerate}
\item Si los eventos $A_t$ son independientes, también lo son los
$\sigma$ campos $(A_t , A_t^c , \emptyset , \Omega)$.
\item Si la imagen inversa $\mathcal{C}_t$ de las clases de todos los
intervalos $(-\infty, x_t)$ en los espacios de Borel $R_t$ son
independientes, también lo son las imágenes inversas $\mathcal{B}_t$
de los campos de Borel en $R_t$. Para todo $\mathcal{C}_t$, éste es
cerrado para la intersección finita y $\mathcal{B}_t$ es el $\sigma$
campo minimal sobre $\mathcal{C}_t$
\item Sean $\mathcal{B}_t$ sigma algebras de eventos y sea $T_s$ un
subconjunto de $T$. La $\sigma$-algebra$\mathcal{B}_T$ compuesto por
componentes $\mathcal{B}_t$, con $t\in T_s$, es el $\sigma$ campo
minimal sobre la clase $\mathcal{C}$ de todas las intersecciones
finitas de eventos $A_t$ y contiene a todos sus componentes
\end{enumerate}
\subsubsection{Teorema de composición}
\begin{theorem}
Los $\sigma$ sigma algebras compuestos son independientes si y solo si sus
$\sigma$ sub sigma algebras finitamente compuestos son independientes
\end{theorem}
\subsection{Familia de variables aleatorias}
Una familia de variables aleatorias $X_{T_s}=\{ X_t \, , \, t\in T_s
\}$ induce $\sigma$ campos $\mathcal{B}(X_{T_s})$ de eventos
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
De donde se deduce por el teorema de la convergencia dominada que
$E(XY) = E(X)E(Y)$
\qed
\end{proof}
\subsubsection{Teorema de la multiplicación}
\begin{theorem}
Sean $X_1,\ldots X_n$ variables aleatorias independientes. Si dichas
variables aleatorias son integrables, también lo es su producto y
además $E\displaystyle\prod_{k=1}^n X_k=\displaystyle\prod_{k=1}^n E
X_k$
\\\\
Reciprocamente, si su producto es integrable y ninguna de ellas degenera
a $0$, entonces todas ellas son integrables.
\end{theorem}
\begin{proof}
La independencia de $X,Y$ nos da la independencia de $X', Y'$, donde
$X' \in {X^+, X^-, |X|}; Y' \in {Y^+, Y^-, |Y|}$, por lo que $E(X'Y')
= E(X')E(Y')$.\\
Si $X,Y$ son integrables, también lo son $X',Y'$ y por la anterior
igualdad también lo es $X'Y'$, lo cual nos da $|XY|$, y por tanto $XY$
integrables con:
$$ E(XY) = E[(X^+-X^-)(Y^+-Y^-)] = E(X^+)E(Y^+) - E(X^+)E(Y^-) - $$
$$ - E(X^-)E(Y^+) + E(X^-)E(Y^-) = E(X)E(Y) $$
\qed
\end{proof}
\subsubsection{Teorema de equivalencia}
\begin{theorem}
Para cada clase finita de conjuntos de Borel $S_t$ y de puntos $x_t,
u_y \in \mathbb{R}$, son equivalentes las tres definiciones siguientes
de independencia de variables aleatorias $X_t$:
\begin{enumerate}
\item $P\bigcap_{k=1}^n [X_{tk}\in S_{tk}]=\displaystyle\prod_{k=1}^n
P[X_{tk}\in S_{tk}]$
\item $F_{t_1\ldots t_n}(x_{t_1},\ldots
,x_{t_n})=F_{t_1}(x_{t_1})\ldots F_{t_n}(x_{t_n})$
\item $f_{t_1\ldots t_n}(u_{t_1},\ldots
,u_{t_n})=f_{t_1}(u_{t_1})\ldots f_{t_n}(u_{t_n})$
\end{enumerate}
\end{theorem}
\begin{proof}$\,$\\
$i) \Rightarrow ii)$\\
Tomamos $S_t = ]-\infty, x_t[$ y aplicamos la definición.\\
$ii) \Rightarrow i)$\\
$S_t = ]-\infty, x_t[$, $\mathcal{C}_t = {]-\infty, x_y[, t \in T}$
son independientes. Por el teorema de extensión, los $\sigma$-campos
minimales sobre ellos son independientes.\\
$i) \Rightarrow iii)$\\
Aplicación directa del teorema de la multiplicación.\\
$iii) \Rightarrow ii)$\\
Tenemos que $F_{t_1,...,t_n}([a_{t_1},...,a_{t_n};b_{t_1},...,b_{t_n}])
= F_{t_1}([a_{t_1},...,a_{t_n};b_{t_1},...,b_{t_n}])$\\$F_{t_2}([a_{t_1},...,a_{t_n};b_{t_1},...,b_{t_n}])...F_{t_n}([a_{t_1},...,a_{t_n};b_{t_1},...,b_{t_n}])$.
Haciendo $a_t \rightarrow - \infty$, $b \uparrow x_t$ tenemos $ii)$
\end{proof}
\subsubsection{Lema de Borel-Cantelli}
\begin{lemma}
Lema de Borel-Cantelli
\\\\
Sea $(\Omega,\mathcal{A},P) \, , \, A_n \in \mathcal{A}$. Entonces:
\begin{itemize}
\item $\displaystyle\sum P(A_n) < \infty \Longrightarrow
P(\displaystyle \lim_{sup}A_n)=0$
\item Si $ A_n$ son independientes:
\begin{itemize}
\item $\displaystyle\sum P(A_n) < \infty \Longrightarrow
P(\displaystyle \lim_{sup}A_n)=0$
\item $\displaystyle\sum P(A_n) = \infty \Longrightarrow
P(\displaystyle \lim_{sup}A_n)=1$
\end{itemize}
\end{itemize}
\end{lemma}


Sean $X_1,\ldots X_n$ variables aleatorias independientes e
idénticamente distribuidas tales que $P[X_n=1]=p$ y $P[X_n=0]=q=1-p$.
Entonces se tiene que:
$$\dfrac{S_n}{n}-p \stackrel{\mathcal{P}}{\longrightarrow}0$$
El Teorema del Límite Central, que desarrollaremos más adelante, es
una consecuencia directa del perfeccionamiento de esta ley por parte
de Moivre y Laplace.
\\\\
Además enunciamos también otra ley muy parecida a esta y también muy
importante que es la \textbf{Ley fuerte de Borel de los grandes
números}, que constituye una versión de esta pero con la convergencia
casi segura.
\subsubsection{Ley fuerte de Borel de los grandes números}
Si se tienen las hipótesis anteriores, entonces: $\dfrac{S_n}{n}-p
\stackrel{c.s.}{\longrightarrow}0$
\begin{theorem}
Sea f(x) continua en $[0,1] \Rightarrow \exists {P_n(x)}$ tal que
$\lim P_n (x) = f(x)$ uniformemente $ \forall x \in [0,1]$.
\end{theorem}
\begin{proof}
\end{proof}
\subsection{Centramiento y truncamiento}
Diremos que centramos $X$ a $c$ si reemplazamos $X$ por $X-c$. Si $X$
es integrable, entonces podemos centrarla a su esperanza $EX$ de forma
que $X$ es reemplazada por $X-EX$. Es decir, diremos que una variable
aleatoria está centrada a su media si y solo si su media existe y es
igual a 0.
\\\\
Ahora vamos a introducir la varianza matemática. Sea $X$ integrable,
llamaremos varianza de $X$ al segundo momento de $X-EX$. Dicho momento
existe pero podría ser $\infty$ y lo denotaremos como $\sigma^2 X$.
Por consiguiente:
$$\sigma^2 X=E(X-EX)^2=EX^2-(EX)^2$$
Se tiene que para todo $c$ finito:
$$\sigma^2(X-c)=E(X-c-E(X-c))^2=E(X-EX)^2$$
lo que quiere decir que cuando centramos una variable su varianza no cambia

\\\\
Se dice que truncamos $X$ a $c>0$ (finita) cuando reemplazamos $X$ por
$X^c=X$ o $0$ dependiendo de si $|X|<c$ o si $|X|\geq c$ ; se dice
entonces que $X^c$ es $X$ truncada a $c$. Lo que estamos haciendo en
realidad es definir una variable truncada, $X^c$ como hemos visto
anteriormente.
\\\\
Tenemos entonces que si $F$ es el diferencial de $X$, entonces existen
todos los momentos de $X^c$ y son finitos; estos son:
$$EX^c=\int_{|X|<c}x\, dF\,\,\, , \,\,\, E(X^c)^2=\int_{|X|<c}x^2\, dF
\,\,\, , \,\,\, \ldots$$
Siempre podremos seleccionar un $c$ suficientemente grande para hacer
que $P[X\neq X^c]=P[|X|\geq c]$ sea arbitrariamente pequeño. Además
nosotros también podemos seleccionar el $c_j$ suficientemente grande
para conseguir $P\bigcup [X_j\neq X_j^{c_j}]$ arbitrariamente pequeño,
de tal forma que, dado $\epsilon > 0$, tenemos:
$$P\bigcup [X_j\neq X_j^{c_j}]\leq \sum P[|X_j|\geq c_j]<\frac{\epsilon}{2^j}$$
Por consiguiente, dada una familia contable de variables aleatorias,
podemos hacer corresponder una familia de variables aleatorias que
difiere de la primera en un evento de probabilidad pequeña. Además, si
estamos interesados principalmente en propiedades en el límite, no
necesitamos probabilidades pequeñas arbitrarias.


\textbf{Definición de convergencia equivalente: } Se dice que $X_n$ y
$X_n^{\prime}$ son equivalentes en la convergencia si el conjunto de
convergencia de ambos es el mismo c.s.
\begin{lemma}
Si las series $\sum P[X_n\neq X_n^{\prime}]$ convergen, entonces las
sucesiones $X_n$ y $X_n^{\prime}$ son cola-equivalentes, y por tanto,
las series $X_n$ y $X_n^{\prime}$ son equivalentes en la convergencia
y las series $\dfrac{S_n}{b_n}$ y $\dfrac{S_n^{\prime}}{b_n}$ con
$b\rightarrow\infty$ convergen al mismo evento y al mismo límite,
excluyendo el evento nulo.
\end{lemma}
\begin{proof}
\end{proof}
\textbf{Corolario: } Si las series $\sum P[X_n\neq X_n^{\prime}]$
convergen, entonces las sucesiones $X_n$ y $X_n^{\prime}$ son
cola-equivalentes, y por tanto, las series $\sum X_n$ y $\sum
X_n^{\prime}$ son equivalentes en cuanto a convergencia.\\
Sean $X_1$ , $X_2$ integrables. Entonces, como el centramiento no
modifica la varianza, podemos asumir, cuando computamos varianzas, que
esas variables aleatorias están centradas a la media. Entonces:
$$\sigma^2 S_n=ES_n^2=\sum_{k=1}^n
EX_k^2+\sum_{j,k=1}EX_jX_k=\sum_{k=1}^n\sigma^2 X_k$$
como $X_j$ y $X_k$ son independientes, tenemos que:
$$EX_jX_k=EX_j\cdot EX_k=0$$
Con esto en mente podemos enunciar la:
\textbf{Desigualdad de Bienaymé: }Si las variables aleatorias
independientes $X_n$ son independientes e integrabless, entonces:
$$ \sigma^2 S_n=\sum_{k=1}^n \sigma^2 X_k$$
Con la desigualdad anterior obtenemos la \textbf{desigualdad de
Bienaymé}:
$$\frac{\displaystyle\sum_{k=1}^n \sigma^2 X_k-\epsilon
^2}{sup(S_n-ES_n)^2}\leq P[|S_n-ES_n|\geq \epsilon]\leq
\frac{\sigma^2(S_n-ES_n)}{\epsilon^2} \leq
\frac{1}{\epsilon^2}\sum_{k=1}^n\sigma^2 X_k$$
Esta desigualdad, aplicada a $(S_{n+k}-ES_{n+k})-(S_n-ES_n)$ y
remplazando $\epsilon$ por $b_n$ y pasando al límite se tiene el
siguiente corolario:
\\\\
\textbf{Corolario: }
\begin{itemize}
\item Si las series $\sum\sigma^2 X_n$ convergen, entonces las series
$\sum (X_n-EX_n)$ convergen en probabilidad.
\item Si $\dfrac{1}{b_n^2}\displaystyle\sum_{k=1}^n \sigma^2
X_k\rightarrow 0$, entonces $\dfrac{S_n -
ES_n}{b_n}\stackrel{\mathcal{P}}{\rightarrow}0$\\
\end{itemize}
\begin{proof}

La demostración pasa por notar que:
$$P[\sum_{k}^{n+h}(X_k - EX_k)\geq\epsilon]\leq
\dfrac{\displaystyle\sum_{k}^{n+h}\sigma^2
X_k}{\epsilon^2}\longrightarrow 0$$
\end{proof}
Este último corolario es debido a Tchebichev (cuando $b_n=n$). En el
caso de Bernouilli, donde $b_n=n$, $EX_n=p$ , $\sigma^2 X_n=pq$ se
reduce a la ley de Bernouilli de los grandes números.

\subsection{Ley débil de los grandes números}
\subsection{Ley fuerte de los grandes números DE Kolmogorov}
Sea ${X_n}$ una sucesión de variables aleatorias independientes e
idénticamente distribuidas con una ley común $\mathcal{L}(X)$.
Entonces:
$$E|X|<\infty \Longleftrightarrow \dfrac{S_n}{n}=\dfrac{\sum_{k=1}^n
X_k}{n}=\dfrac{X_1 \ldots X_n}{n}\stackrel{c.s}{\longrightarrow}EX$$

\chapter{El problema central del límite}
El problema del límite central en probabilidad es el problema de
convergencia de leyes de secuencias de sumas de variables aleatorias.
\section{Preeliminares}
Consideramos $S_n$ el número de ocurrencias de un determinado evento
con probabilidad $p$ en $n$ intentos idénticos e independientes. Para
evitar trivialidades asumimos que $pq\neq 0$, donde $q=1-p$. Si $X_k$
denota el indicador del evento en el $k$-ésimo intento, entonces
$S_n=\displaystyle\sum_{k=1}^n X_k$ con $n=1,2,\ldots$ donde los
sumandos son indicadores independientes e idénticamente distribuidos.
Este es el caso de Bernouilli; como $EX_k=p$ y $EX_k^2=p$, entonces
$\sigma^2 X_k=p-p^2=pq$ de donde se sigue que:
$$ES_n=\sum_{k=1}^nEX_k=np \,\,\, , \,\,\, \sigma^2 S_n=\sum_{k=1}^n
\sigma^2 X_k=npq$$
EL primer teorema del límite central publicado en 1713 dice que
$\dfrac{S_n}{n}\stackrel{\mathcal{P}}{\longrightarrow}p$
\\\\
Puliendo este resultado, de Moivre obtuvo el segundo teorema de
límites, que en la forma integral dada por Laplace, dice que:
$$P\left[ \frac{S_n -np}{\sqrt{npq}}< x \right]\rightarrow
\frac{1}{\sqrt{2\pi}}\int_{-\infty}^{x}e^{-\frac{1}{2}y^2}dy\, ,\,\,\,
-\infty\leq x\leq \infty$$
\\\\
El tercer teorema del límite central fue obtenido por Poisson, quien
modificó el caso de Bernouilli asumiendo que la probabilidad $p=p_n$
depende del número de intentos de tal manera que
$np_n\rightarrow\lambda>0$. Por consiguiente, escribiendo ahora
$X_{nk}$ y $S_{nn}$ en lugar de $X_k$ y $S_n$, el caso de Poisson
corresponde a una serie de sumas $S_{nn}=\displaystyle\sum_{k=1}^n
X_{nk}$ donde, para cada n, los sumandos $X_{nk}$ son indicadores
independientes e idénticamente distribuidos con
$P[X_{nk}=1]=\dfrac{\lambda}{n}+o \left( \dfrac{1}{n}\right)$



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

\cleardoublepage 

# (APPENDIX) Apéndice {-}

# Software Tools

For those who are not familiar with software packages required for using R Markdown, we give a brief introduction to the installation and maintenance of these packages.

## R and R packages

R can be downloaded and installed from any CRAN (the Comprehensive R Archive Network) mirrors, e.g., https://cran.rstudio.com. Please note that there will be a few new releases of R every year, and you may want to upgrade R occasionally.

To install the **bookdown** package, you can type this in R:


```r
install.packages("bookdown")
```

This installs all required R packages. You can also choose to install all optional packages as well, if you do not care too much about whether these packages will actually be used to compile your book (such as **htmlwidgets**):


```r
install.packages("bookdown", dependencies = TRUE)
```

If you want to test the development version of **bookdown** on GitHub, you need to install **devtools** first:


```r
if (!requireNamespace('devtools')) install.packages('devtools')
devtools::install_github('rstudio/bookdown')
```

R packages are also often constantly updated on CRAN or GitHub, so you may want to update them once in a while:


```r
update.packages(ask = FALSE)
```

Although it is not required, the RStudio IDE can make a lot of things much easier when you work on R-related projects. The RStudio IDE can be downloaded from https://www.rstudio.com.

## Pandoc

An R Markdown document (`*.Rmd`) is first compiled to Markdown (`*.md`) through the **knitr** package, and then Markdown is compiled to other output formats (such as LaTeX or HTML) through Pandoc.\index{Pandoc} This process is automated by the **rmarkdown** package. You do not need to install **knitr** or **rmarkdown** separately, because they are the required packages of **bookdown** and will be automatically installed when you install **bookdown**. However, Pandoc is not an R package, so it will not be automatically installed when you install **bookdown**. You can follow the installation instructions on the Pandoc homepage (http://pandoc.org) to install Pandoc, but if you use the RStudio IDE, you do not really need to install Pandoc separately, because RStudio includes a copy of Pandoc. The Pandoc version number can be obtained via:


```r
rmarkdown::pandoc_version()
## [1] '1.19.2.4'
```

If you find this version too low and there are Pandoc features only in a later version, you can install the later version of Pandoc, and **rmarkdown** will call the newer version instead of its built-in version.

## LaTeX

LaTeX\index{LaTeX} is required only if you want to convert your book to PDF. The typical choice of the LaTeX distribution depends on your operating system. Windows users may consider MiKTeX (http://miktex.org), Mac OS X users can install MacTeX (http://www.tug.org/mactex/), and Linux users can install TeXLive (http://www.tug.org/texlive). See https://www.latex-project.org/get/ for more information about LaTeX and its installation.

Most LaTeX distributions provide a minimal/basic package and a full package. You can install the basic package if you have limited disk space and know how to install LaTeX packages later. The full package is often significantly larger in size, since it contains all LaTeX packages, and you are unlikely to run into the problem of missing packages in LaTeX.

LaTeX error messages may be obscure to beginners, but you may find solutions by searching for the error message online (you have good chances of ending up on [StackExchange](http://tex.stackexchange.com)). In fact, the LaTeX code converted from R Markdown should be safe enough and you should not frequently run into LaTeX problems unless you introduced raw LaTeX content in your Rmd documents. The most common LaTeX problem should be missing LaTeX packages, and the error may look like this:

```latex
! LaTeX Error: File `titling.sty' not found.

Type X to quit or <RETURN> to proceed,
or enter new name. (Default extension: sty)

Enter file name: 
! Emergency stop.
<read *> 
         
l.107 ^^M

pandoc: Error producing PDF
Error: pandoc document conversion failed with error 43
Execution halted
```

This means you used a package that contains `titling.sty`, but it was not installed. LaTeX package names are often the same as the `*.sty` filenames, so in this case, you can try to install the `titling` package. Both MiKTeX and MacTeX provide a graphical user interface to manage packages. You can find the MiKTeX package manager from the start menu, and MacTeX's package manager from the application "TeX Live Utility". Type the name of the package, or the filename to search for the package and install it. TeXLive may be a little trickier: if you use the pre-built TeXLive packages of your Linux distribution, you need to search in the package repository and your keywords may match other non-LaTeX packages. Personally, I find it frustrating to use the pre-built collections of packages on Linux, and much easier to install TeXLive from source, in which case you can manage packages using the `tlmgr` command. For example, you can search for `titling.sty` from the TeXLive package repository:

```bash
tlmgr search --global --file titling.sty
# titling:
#	 texmf-dist/tex/latex/titling/titling.sty
```

Once you have figured out the package name, you can install it by:

```bash
tlmgr install titling  # may require sudo
```

LaTeX distributions and packages are also updated from time to time, and you may consider updating them especially when you run into LaTeX problems. You can find out the version of your LaTeX distribution by:



```r
system('pdflatex --version')
## pdfTeX 3.14159265-2.6-1.40.18 (TeX Live 2017)
## kpathsea version 6.2.3
## Copyright 2017 Han The Thanh (pdfTeX) et al.
## There is NO warranty.  Redistribution of this software is
## covered by the terms of both the pdfTeX copyright and
## the Lesser GNU General Public License.
## For more information about these matters, see the file
## named COPYING and the pdfTeX source.
## Primary author of pdfTeX: Han The Thanh (pdfTeX) et al.
## Compiled with libpng 1.6.29; using libpng 1.6.29
## Compiled with zlib 1.2.11; using zlib 1.2.11
## Compiled with xpdf version 3.04
```

<!--chapter:end:400-apendice.Rmd-->

# Referencias {-}




<!--chapter:end:500-references.Rmd-->

