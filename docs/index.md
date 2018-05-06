# Introducción al análisis funcional y a la teoría de la medida
Synergy Vision  
`r Sys.Date()`  
<script src="https://cdn.datacamp.com/datacamp-light-latest.min.js"></script>

--- 
title: "Introducción al análisis funcional y a la teoría de la medida"
subtitle: "Ciencia de los Datos Financieros"
author: "Synergy Vision"
date: "2018-05-06"
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

# Conjuntos

## Operaciones

## Relaciones

## Funciones

## Cardinalidad

<!--chapter:end:011-Conjuntos.Rmd-->

# Sistema numérico real y complejo

## Introducción

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
## [1] '1.19.2.1'
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
## MiKTeX-pdfTeX 2.9.6354 (1.40.18) (MiKTeX 2.9.6350)
## 2.9.6354 (1.40.18)
## TeX is a trademark of the American Mathematical Society.
## using bzip2 version 1.0.6, 6-Sept-2010
## compiled with curl version 7.54.0; using libcurl/7.54.0 WinSSL
## compiled with expat version 2.2; using expat_2.2.0
## compiled with jpeg version 9.2
## compiled with liblzma version 50020032; using 50020032
## compiled with libpng version 1.6.29; using 1.6.29
## compiled with libressl version LibreSSL 2.5.3; using LibreSSL 2.5.3
## compiled with MiKTeX Application Framework version 1.6334; using 1.6334
## compiled with MiKTeX Core version 1.6344; using 1.6344
## compiled with MiKTeX Archive Extractor version 1.6300; using 1.6300
## compiled with MiKTeX Package Manager version 1.6353; using 1.6353
## compiled with poppler version 0.55.0
## compiled with uriparser version 0.8.4
## compiled with zlib version 1.2.11; using 1.2.11
```

<!--chapter:end:400-apendice.Rmd-->

# Referencias {-}




<!--chapter:end:500-references.Rmd-->

