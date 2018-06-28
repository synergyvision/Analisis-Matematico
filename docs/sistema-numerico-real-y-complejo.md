--- 
title: "Introducción al análisis funcional y a la teoría de la medida"
subtitle: "Ciencia de los Datos Financieros"
author: "Synergy Vision"
date: "2018-06-28"
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

## Definición y ejemplos

##  El teorema del valor medio

## Funciones convexas

## Funciones inversas

## Regla de L'Hospital

## Teorema de Taylor en $\mathbb{R}$

## Método de Newton

<!--chapter:end:104-diferenciacionR.Rmd-->

# Integración de Riemann

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


# (APPENDIX) Apéndice {-}

Placeholder

# Software Tools

Placeholder


## R and R packages
## Pandoc
## LaTeX

<!--chapter:end:400-apendice.Rmd-->

# Referencias {-}




<!--chapter:end:500-references.Rmd-->

