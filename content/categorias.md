+++
date = '2025-03-26T19:24:58-06:00'
draft = true
title = 'Categorias'
+++

La siguiente consisteseminario de categorias organizado por estudiantes de la maestría en m-áticas básicas en CIMAT, México.


##Sesión 1: Introducción a las Categorías por [Luis](https://luisquijanosegura.wordpress.com/)



###Categorías
Una *categoría* C consiste de
-Una clase de *objetos* $\mathrm{Ob}(\mathrm{C})= $   $X,Y,...$
-Una clase de \textbf{morfismos} \hspace{0.1cm} $\mathrm{Mor}(\mathrm{C})=$ $f,g,...$ 
Que cumplen:
    - Dominio y codominio son *objetos* en C.
    - *Existencia* del morfismo identidad

    - En caso de estar bien definida, *existencia* de la composición

    $$ f:X\to Y, \; g:Y\to Z \quad \rightsquigarrow\quad g\circ f: X\to Z$$

###Axiomas de las categorías
-  $f:X\to Y$ cumple que $1_Y \circ f =f=f\circ 1_X$
-$(f,g,h)$: $h(gf)  $ y $(hg)f$ son equivalentes.


*Notación:* Dados $f,g$ que permitan $f\circ g$, la denotaremos como $fg$ .

###Ejemplos de Categorías
    - *Set*:  (Conjuntos, funciones)

    - *Top* (Esp. Top, fun. cont.)

    - *Group* y *Ring* (Grupos/Anillos, homomorfismos)

    - *Man* (Variedades suaves, fun. suaves)


Una  *Subcategoría* $D\subset C$ es una subcolección de (*obj*,*hom*) tal que todo *hom* en $D$ está bien definido.

###Casos particulares:

Decimos que *C* es *pequeña* si $\text\textbf{mor(C)} \in \text{\textbf{Set}}$.




\begin{definition}
      *C* es *localmente pequeña* si:

        Dado (X,Y):   $\mathrm{Hom} (X,Y)\in \mathrm{Set}$:

\end{definition}

###Tipos de Morfismos:
    \begin{definition}
         - $f$ *isomorfismo* tal que $\exists g $ con $fg=\mathds{1}$, $gf=\mathds{1}$ 


        - 
$f$ *endomorfismo* tal que $f:X\to X$ 


        -  $f$ *automorfismo*   unión de las 2 anteriores.
\end{definition}

\begin{block}{Notación:}
\end{block}




###Más tipos
\begin{definition} $f:X\to Y$ 
    - *monomorfismo* Dados $h,k:W\rightrightarrows X$ 
    
    $fh=fk \Leftrightarrow h=k $

    
        $f:X\rightarrowtail Y $


    - *epimorphismo*
    Dados $h,k:Y\rightrightarrows Z$ 

    $hf=kf \Leftrightarrow h=k $


    $f:X\twoheadrightarrow Y$
    
\end{definition}

###Propiedad
    \begin{corollary}
            - $f: X\rightarrowtail Y ,g: Y\rightarrowtail Z \Rightarrow gf: X\rightarrowtail Z$

            - $g,f$ tales que $gf: X\rightarrowtail Z \Rightarrow f:X\rightarrowtail Y$ 
            
    \end{corollary}


  


###Grupoide

\begin{definition}
     *Grupoide*:
     
     *Cat* tal que: todo $ f:X\to Y$ es *iso*


\end{definition}

\begin{lemma}
    Toda categoría C contiene un *grupoide maximal*
\end{lemma}

Demo:


"Remplazamos" la clase *morfismos*, por la clase *isomorfismos*.
    

###Dualidad

\begin{definition}
    Dada una categoría C, una *categoría opuesta* ($\mathrm{C}^{\mathrm{op}}$ incluye  

        - Objetos iguales pero:

        - dirección de la "flecha"  *opuesta*


        $f^{op}:X\to Y\leftrightsquigarrow  f:Y\to X$
\end{definition}



###Axiomas y ejemplos
        - Existencia $\mathds{1}_X^{op}$

        - Existencia de la *composición*:


*Ejemplo:*

$\mathrm{Vect}_{\mathbb{F}}^{\mathrm{op}}$

###Usando la dualidad
    \begin{lemma} 
    $C$, $x,y$ objetos, son equivalentes:
        \begin{enumerate}
            - $f:x\to y$ isomorfismo

            - $f_* :\mathrm{Hom}(c,x)\xrightarrow{f\circ ()} \mathrm{Hom}(c,y)$ biyección

            - $f^* :\mathrm{Hom}(y,c)\xrightarrow{()\circ f}\mathrm{Hom}(x,c)$ biyección
            
        \end{enumerate}
    \end{lemma}

###Demostración
    \begin{block}{1 = 2}
            - Por (1) $\exists g$ inv. de $f$, def:
            $ g_* :\mathrm{Hom}(y,c)\xrightarrow{g \circ()}\mathrm{Hom}(x,c)$

            $$ f_* g_* :\mathrm{Hom}(c,x)\xrightarrow{f g\circ()} \mathrm{Hom}(c,x)$$


            $$g_* f_* :\mathrm{Hom}(c,y)\xrightarrow{ gf\circ()} \mathrm{Hom}(c,y)$$


            - $$(f_*)_{c=y}: \mathrm{Hom}(y,x)\xrightarrow{f\circ ()} \mathrm{Hom}(y,y)$$
            
            $\exists g , $ tal que $f_*(g)=\mathds{1}_Y$

    $$(f_*)_{c=x}: \mathrm{Hom}(x,x)\xrightarrow{f\circ ()} \mathrm{Hom}(x,y)  $$

    $f_*(gf)=f_*(\mathds{1}_X)$

    \end{block}


###3

$f$ es iso $\Leftrightarrow  f^{\mathrm{op}}$ es iso

    $$f_* :\mathrm{Hom}(c,x)\rightarrow \mathrm{Hom}(c,y) $$
    
    $$(f^{\mathrm{op}})_*:\mathrm{Hom}^{\mathrm{op}}(c,y) \to \mathrm{Hom}^{\mathrm{op}}(c,x)$$

    $$f^* :\mathrm{Hom}(y,c)\rightarrow\mathrm{Hom}(x,c) $$



###Dualidad
        \begin{corollary}
            - $f: X\rightarrowtail Y ,g: Y\rightarrowtail Z \Rightarrow gf: X\rightarrowtail Z$

            - $g,f$ tales que $gf: X\rightarrowtail Z \Rightarrow f:X\rightarrowtail Y$ 
            
    \end{corollary}


    Dualmente:


    \begin{corollary}
            - $f: X\twoheadrightarrow Y ,g: Y\twoheadrightarrow Z \Rightarrow gf: X\twoheadrightarrow Z$

        - $g,f$ tales que $gf: X\twoheadrightarrow Z \Rightarrow g:X\twoheadrightarrow Y$ 
    \end{corollary}


###Funtores
\begin{definition}
    *Funtor* (covariante) $F:C\to D$

    
    - $Fc\in D \quad \forall c\in C$

    - $Ff:Fc\to Fc' \quad \forall f: c\to c' $
    
\end{definition}

    

###Axiomas y Ejemplos

*Axiomas:*
    - $ Fg\circ Ff =F(g\circ f)$
    
- $F(\mathds{1}_c)= \mathds{1}_{Fc}$

*Ejemplos*

(Algún) funtor olvido 

    - $F: \mathrm{Top \to \mathrm{Set}}$


    - $\pi_1 : \mathrm{Top}_* \to \mathrm{Group}$
    

###Contravariante

\begin{definition}
    *Funtor contravariante*
\end{definition}


*Axiomas:*

    - $Ff\circ Fg =F(g\circ f)$

    - $F\mathds{1}_c=1_{Fc}$

\begin{tikzcd}[ampersand replacement=\&, column sep=small]
C^{op} \arrow[rrr, "F"] \&                       \&    \& D                    \\
c \arrow[dd, "f"]       \& {} \arrow[r, maps to] \& {} \& Fc                   \\
                        \& {} \arrow[r, maps to] \& {} \&                      \\
c'                      \& {} \arrow[r, maps to] \& {} \& Fc' \arrow[uu, "Ff"]
\end{tikzcd}
    

###Axiomas y ejemplos
*Axiomas:*

    - $Ff\cdot Fg=F(g\cdot f)$
    - $F(1_c)=1_{Fc}$


    *Ejemplos*

    -    $(- )^{*}: \mathrm{Vect}_{\mathbb{F}}^{\mathrm{op}}\to \mathrm{Vect}_{\mathbb{F}}$

    - $P:\mathrm{Set}^{\mathrm{op}}\to \mathrm{Set}$
 





###Una propiedad útil
    \begin{lemma}
        Funtores preservan isomorfismos
    \end{lemma}

*Idea demo*
    $F:C\to D$

    Por axiomas de funtores 
    
        - $F(g)\circ F(f)=F(g\circ f ) $

        -     $F(f)\circ F(g)= F(f\circ g)$



###Funtores especiales

\begin{definition}
    Dados C localmente pequeña y c objeto en C:
\end{definition}



###Transformaciones Naturales
C,D 

$F,G : C\rightrightarrows D$

\begin{definition}
    *Transformación natural*

    $\alpha:F\Rightarrow G$

    $c\mapsto \alpha_c :Fc \to Gc$
\end{definition}


###Isomorfismo natural

\begin{definition}
    *Isomorfismo natural*

    $\alpha_c$ biyectivo
\end{definition}




###Ejemplos
        - $\mathrm{ev}: 1_{\mathrm{Vect}_{\mathbb{F}}} \Rightarrow (-)^{**} $



-
$\eta: 1_{\mathrm{Set}}\Rightarrow P$


$\eta_A (a)\mapsto \{a\} $


