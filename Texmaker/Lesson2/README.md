## How to write (Maths, Table, Graph,...)
- Lesson 2

```
\documentclass[12pt,a5paper]{article}
\usepackage[utf8]{inputenc}
\usepackage[left=1cm,right=1cm,top=2cm,bottom=2cm]{geometry}
\usepackage{amsmath}
\usepackage{amssymb}
\everymath{\displaystyle}
\usepackage{multicol}
\usepackage{enumitem}
\usepackage{xcolor}
\usepackage{fancyhdr}
\pagestyle{fancy}
\lhead{This is my name}
\rhead{this is page \thepage}
\cfoot{center of the footer!}
\renewcommand{\headrulewidth}{0.2pt}
\renewcommand{\footrulewidth}{0.2pt}
\SetEnumitemKey{I}{label=\color{blue}\Roman*.}
\SetEnumitemKey{1}{label=\color{red} \arabic*.}
%\SetEnumitemKey{1}{label= \knum*.}
\SetEnumitemKey{a}{label=\color{red} \kalph*.}
\SetEnumitemKey{A}{label= \Alph*:}
\SetEnumitemKey{c}{label= \alph*.}
\usepackage{fancyhdr}
\pagestyle{fancy}
\lhead{Tontan}
\rhead{Hak}
\lfoot{Tex}
\rfoot{Marker}
\cfoot{\thepage}
\renewcommand{\headrulewidth}{2pt}
\renewcommand{\footrulewidth}{2pt}
\usepackage{mathfont}
\usepackage{dutchcal}
\usepackage[no-math]{fontspec}
\setmainfont{Khmer OS Siemreap}
%-------------- newcomand---------
\newcommand{\N}{\mathbb{N}}
\newcommand{\R}{\mathbb{R}}
\newcommand{\Z}{\mathbb{Z}}
\newcommand{\C}{\mathbb{C}}
\setmainfont{Khmer OS Siemreap}
\setmathrm{Times New Roman}
\newcommand{\kml}{\fontspec{Khmer OS Muol Light}\selectfont}
\newcommand{\kbk}{\fontspec{Khmer OS Bokor}\selectfont}
\usepackage{tkz-tab}
\usepackage {tikz}
\usepackage{pgfplots}
\begin{document}
\begin{center}
\underline{\underline{Homework}}
\end{center}
\begin{enumerate}[I]
\item equation $ax^2+bx+c=0 \text{ that } a\neq 0$\\
 Let $\Delta=b^2-4ac $
   \begin{itemize}
   \item If $\Delta >0$ than $x=\dfrac{-b\pm \sqrt{\Delta}}{2a}$
   \item If $\Delta =0$ than $x=-\dfrac{b}{2a}$
   \end{itemize}
 \item Integral 
  \begin{enumerate}[1]
  \begin{multicols}{3}
  \item $\int xdx$
  \item $\int x^2dx $
  \item $\int \sqrt{x}dx$
  \item $\int \sqrt[3]{\sin x}dx$
  \item $\int \frac{1}{x}dx $
  \item $\int \cos xdx$
  \end{multicols}
    \end{enumerate}   
 
 \item Sum of Sequence $S_n =\sum_{k=1}^{n}k$
 \item Limit  
 \begin{enumerate}
 \begin{multicols}{2}
 \item $\lim_{x \to 0}\dfrac{\sin x}{x}=1 $
 \item $\sum_{k=1}^{n}x$
 \item $\int xdx$
 \item $\sqrt[3]{x^3 -1}$
 \end{multicols}
 \end{enumerate}
 \item Solution 
 \begin{itemize}
 \begin{multicols}{2}
 \item $\sin x - \cos x = 1$
 \item $n\in \mathbb{N}$
 \item $t\in \mathcal{R}$
 \item $z\in \mathbcal{Z}$
 \item $\C$
 \item $\R$
 \end{multicols}
 \end{itemize}
\end{enumerate}
\newpage
\begin{center}
\underline{\underline{Solution}}
\end{center}
\begin{enumerate}
\item Simplify: $(3\sqrt{5}-5\sqrt{2})(4\sqrt{5}+3\sqrt{2}) $.\\
Solution: $\begin{aligned}[t]
(3\sqrt{5}-5\sqrt{2})(4\sqrt{5}+3\sqrt{2})&=2\times 5-20\sqrt{2}\times \sqrt{5}+9\sqrt{5}\times \sqrt{2}-15\times 2\\
&=60-20\sqrt{10}-30\\
&=30-11\sqrt{10}
\end{aligned} $
\item Simplify: $\left[5\left( 8^{\frac{1}{3}}+27^{\frac{1}{3}} \right)^3   \right]^{\frac{1}{4}} $\\
Solution: 
\begin{align*}
\left[5\left(8^{\frac{1}{3}}+27^{\frac{1}{3}}  \right)^3 \right]^{\frac{1}{4}}&=\left[5\left((2^3)^{\frac{1}{3}}+(3^3)^{\frac{1}{3}}  \right)^3  \right]^{\frac{1}{4}}\\
&=[5(2+3)^3]^{\frac{1}{4}}\\
&=[5(5)^3]^{\frac{1}{4}}\\
&=(5^4)^{\frac{1}{4}}\\
&=5
\end{align*}
\item Plot the point $(x,y)$ given by the following table. Use scale $1\text{cm}=0.25$ units
\begin{center}
$\begin{array}{|c|c|c|c|c|}
\hline
x & 1.25 & 0.25 & 1.5 & -1.75 \\ 
\hline
y & -0.5 & 1 & 1.5 & -0.25\\
\hline
\end{array}$ 
\end{center}
\end{enumerate}
\newpage
\begin{center}
\kml កិច្ចការផ្ទះ
\end{center}
\begin{enumerate}
\item ដោះស្រាយ{\kbk សមីការ}នីមួយៗខាងក្រោម៖
 \begin{enumerate}
 \item $x^2+2x+1=0$
 \item $x^2-4=0$
 \end{enumerate}
\item គណនាអាំងតេក្រាល៖
  \begin{enumerate}
  \item $\int xdx$
  \item $\int \sin x.\cos xdx$
  \end{enumerate}
  \item កាលវិភាគប្រចាំថ្ងៃ
\begin{center}
\begin{tabular}{|c|c|c|}
\hline 
 \multicolumn{3}{|c|}{ព្រឹក}   \\ 
\hline
7-8 & \multicolumn{2}{|c|}{គណិត} \\ 
\hline
8-9 & ខ្មែរ & រូប \\ 
\hline 
\end{tabular} 
\end{center}
\item តារាង
\begin{center}
$\begin{array}{|c|c|c|c|c|c|}
\hline
\multicolumn{2}{|c|}{} & \multicolumn{3}{|c|}{\text{ X}} &  \\ 
\cline{3-5}
\multicolumn{2}{|c|}{f(x,y)}& 0 & 1 & 2 & h(y) \\ 
\hline 
 & 1 & 2 & 3 & 4 & 5 \\ 
y & a & b & c & d & e \\ 
 & 5 & 10 & 15 & 0 & 20 \\ 
\hline 
\multicolumn{2}{|c|}{g(x)}& 2 & 4 & 1 & 1 \\
\hline
\end{array}$ 
\end{center}
\item តារាងអថេរភាព៖
\begin{center}
\tikz \tkzTabInit{$x$ /.8 , $f(x)$ /.8}{$0$ , $+\infty$};
\end{center}
\end{enumerate}
\newpage
\begin{enumerate}
\item តារាងអថេរភាព៖
\begin{center}
\begin{tikzpicture}
\tkzTabInit[color,espcl=1.5]
{$x$ / 1,$g(x)$ / 1}
{$0$,$1$,$2$,$3$}%
\tkzTabLine{z, + , d , h , d , - , t}
\end{tikzpicture}
\end{center}
\item color
\begin{center}
\begin{tikzpicture}
\tkzTab[lgt=2,espcl=3]{ $x$ / 1,
$f'(x)$ / 1,
 $f$ / 2}
{ $-5$ , $0$ ,$7$}
{ ,-,z,+,}
{ +/$25$ , -/$0$ , +/ $49$}%
\end{tikzpicture}

\end{center}
\item តារាងទ្វេធា
\begin{center}
\begin{tikzpicture}
\tkzTabInit
{$x$ /1,
$f(x)$ /1,
$g(x)$ /1}
{$0$,$e$,$+\infty$}
\tkzTabLine{,\text{សញ្ញាផ្ទុយ},d,\text{សញ្ញាដូច},}
\tkzTabLine{,-, z ,+,}
\end{tikzpicture}
\end{center}
\item តារាងត្រីធា
\begin{center}
\begin{tikzpicture}
\tkzTabInit[espcl=3]
{$x$ /1, $f''{x}$ /1,$f'(x)$ /2, $f(x)$ /2}%
{$0$ , $1$ , $+\infty$ }%
\tkzTabLine{d,+,z,-, }%
\tkzTabVar {D-/ /$1$,+/ $\frac{2}{3}$ /,-/ $0$ /}%
\tkzTabVar {D-/ /$-\infty$ ,R/ $0$ /, +/ $+8$ /}
\end{tikzpicture}
\end{center}
\newpage
\item ក្រាប
\begin{center}
\begin{tikzpicture}
%\foreach \x in {-3,-2,-1,1,2,3}
%\draw [shift={(\x,0)} (0,-2pt)--(0,-2pt) node {below}{\scriptsize $\x$};
%\foreach \y in {-3,-2,-1,1,2,3}
%\draw [shift={(\x,0)} (-2pt,0)--(2pt,0) node {below}{\scriptsize $\y$};
\draw [->] (-4,0)--(4,0) node [right]{$x$};
\draw [->] (0,-2)--(0,5) node [right]{$y$};
\draw [samples=100,domain=-3.5:1.5] plot (\x, {2.718^(\x)});
\end{tikzpicture}
\end{center}
\end{enumerate}
\end{document}
```
