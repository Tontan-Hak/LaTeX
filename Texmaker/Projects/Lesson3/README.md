## Math exercises 
- lesson 3

```
\documentclass[12pt,a5paper]{article}
\usepackage[utf8]{inputenc}
\usepackage{amsmath}
\usepackage{nicematrix}
\usepackage{amsfonts}
\usepackage{rotating}
\usepackage{tkz-tab}
\usepackage{amssymb}
\usepackage[no-math]{fontspec}
\setmainfont{Khmer OS Siemreap}
\setmathrm{Times New Roman}
\newcommand{\kml}{\fontspec{Khmer OS Muol Light}\selectfont}
\newcommand{\kbk}{\fontspec{Khmer OS Bokor}\selectfont}
\usepackage[left=2cm,right=2cm,top=2cm,bottom=2cm]{geometry}
\everymath{\displaystyle}
\begin{document}
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
 \multicolumn{3}{|c|}{ ព្រឹក}   \\ 
\hline
7-8 & \multicolumn{2}{|c|}{គណិត} \\ 
\hline
8-9 & ខ្មែរ & រូប \\ 
\hline 
\end{tabular} 
\end{center}
\item តារាង
\begin{center}
$\begin{array}{c|c|ccc|c}
\hline 
\multicolumn{2}{c|}{} & \multicolumn{3}{c|}{\text{ X}} &  \\ 
\cline{3-5}
\multicolumn{2}{c|}{f(x,y)}& 0 & 1 & 2 & h(y) \\ 
\hline 
 & 1 & 2 & 3 & 4 & 5 \\ 
y & a & b & c & d & e \\ 
 & 5 & 10 & 15 & 0 & 20 \\ 
\hline 
\multicolumn{2}{l|}{g(x)}& 2 & 4 & 1 & 1 
\end{array}$ 
\end{center}
\item តារាងអថេរភាព១ 
\begin{center}
\tikz \tkzTabInit{$x$ /1 , $f(x)$ /1.5, $g(x)$/1.5}{$0$ , $e$ , $+\infty$};
\end{center}
\item តារាងអថេរភាព២
\begin{center}
\begin{tikzpicture}
\tkzTabInit{ $x$/1,$f(x)$/1.5,$g(x)$/1.5}
{$-\infty$, $e$ , $+\infty$}
\tkzTabLine{ , - , z , + , }
\tkzTabVar{+/$5$ , -/ $1$, +/ $2$}%
\end{tikzpicture}
\end{center}
\item តារាងអរថេរភាព
\begin{center}
\begin{tikzpicture}
\tkzTabInit[espcl=2]%
{$x$ / 1,$f'(x)$ / 1, $f(x)$/2}%
{$0$,$e$,$+\infty$}%
\tkzTabLine{d,+,z,-,}
\tkzTabVar{D-/$-\infty$ , +/ $1.7$, -/$1$}%
\end{tikzpicture}
\end{center}
\item តារាងអរថេរភាព
\begin{center}
\begin{tikzpicture}
\tkzTabInit[espcl=2]%
{$x$ / 1,$f'(x)$ / 1, $f(x)$/2}%
{$-\infty$,$-1$, $0$, $1$ , $+\infty$}%
\tkzTabLine{,-,z,+,d,+,z,-,}
\tkzTabVar{+/$+\infty$,-/$2$,+D-/$+\infty$/$-\infty$,+/$3$,-/$-\infty$ }
\end{tikzpicture}
\end{center}
\item រូបត្រីកោណ
 \begin{center}
 \begin{tikzpicture}
  \fill[fill=gray!40,draw](0,0)--(4,0)--(4,3)--(0,0);
 \draw[blue] (0,0) -- (0.:0.7) arc (0.:36.86:0.7) -- cycle;
 \draw (3.5,0)--(3.5,0.5)--(4,0.5);
 \node at (0,0)[left]{$A$};
 \node at (4,0)[right]{$B$};
 \node at (4,3)[above]{$C$};
 \node at (2,0)[below]{$4\text{cm}$};
 \node at (4,1.5)[right]{$3\text{cm}$};
 \node at (1.8,1.7){\begin{turn}{40} $5\text{cm}$\end{turn} };
 \draw (0.7,0)--(0,0)--(0.55,0.4);
 \draw [shift={(4,3)}] (0,0) -- (-143.1:0.7) arc (-143.1:-90.:0.7) -- cycle;
 \end{tikzpicture}
 \end{center}
\end{enumerate}
\newpage
\begin{enumerate}
 \item ក្រាប
 \begin{center}
   \begin{tikzpicture}
   \draw [->](-4,0)--(4,0) node [right]{$x$};
   \draw [->](0,-4)--(0,4) node [above]{$y$};
   \foreach \x in {-3,-2,-1,1,2,3}
   \draw[shift={(\x,0)}](0pt,2pt)--(0pt,-2pt) node [below]{$\x$} ;
   \foreach \y in {-3,-2,-1,1,2,3}
   \draw[shift={(0,\y)}](2pt,0)--(-2pt,0)node [right,blue]{$\y$};
   \draw [samples=50,domain=(-2:2)] plot (\x,{(\x)^2-3});
   \draw [samples=50,domain=(-3:1.5)] plot (\x,{2.718^\x});
   \node at (-0.4,-0.4){$0$};
   \end{tikzpicture}
 \end{center}
\end{enumerate}
\end{document}
```
