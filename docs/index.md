<script src="https://cdn.datacamp.com/datacamp-light-latest.min.js"></script>

--- 
title: "Introducción al análisis funcional y a la teoría de la medida"
subtitle: "Ciencia de los Datos Financieros"
author: "Synergy Vision"
date: "2019-02-27"
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

Pero... tenemos 2 problemas:
\begin{itemize}
\item Necesitamos una manera cómoda con la que construir $\tlps$.
\item ¿Utilizando otra parametrización llegamos al mismo resultado?
\end{itemize}

Vamos a reventar 2 pajaros de un tiro.

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

Bueno, esto cumple lo que la sabíamos de selectividad. El área de un paralelogramo 2 dimensional en $\real^3$ es la raiz cuadrada del módulo del producto vectorial.

\textbf{Aplicación:} Vamos a aplicar esto para hallar el área de una $k-variedad$ en $\real^N$.

\todo{Dibujo}
\begin{itemize}
\item $\Phi(\gs_0) = \gx_0 \in M$
\item $\Phi(\gs_0 + h_j\gor{e}_j) = \Phi(\gs_0) + \dpa{\Phi}{s_j}(\gs_0)\cdot h_j + err(h)$
Aplicando taylor, en el que cada alargamiento $h$ depende de la dirección.
\end{itemize}

\textbf{Idea:} $Area(\Phi(Q_k)) = Area(P_k) + err(h)$ donde $Area(P_k) = \left(\det (\pesc{v_i,v_j})\right)^{\frac{1}{2}}, \{v_j\}$ genera $P_k$.

\todo{Me he perdido porque $v_i = \dpa{\Phi}{s_j}(\gs_0)\cdot h_j$}

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

\textbf{Idea:} Vamos a dedicarnos a jugar con los vectores de la base aplicandoles una deformación continua para ver que pasa con la discontinuidad de la orientación en $\pi$ a ver que encontramos.

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

Aunque podríamos llevar $e_3 \to \gu$ y $e_1 \to \gw$... ¿Entonces?

Mal! Porque no estamos manteniendo el orden, tendríamos la base $\mathcal{C}* = \{\gw,\gv,\gu\}\neq\mathcal{C}$.


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

Curioso: esta parametrización que no cubre el segmento con el que se empieza. Esta parametrización tiene una propiedad curiosa, al empezar, el vector normal apunta hacia dentro y al final, apunta hacia fuera. Es imposible cubrirla del todo con una parametrización.

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
## [1] '2.5'
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

