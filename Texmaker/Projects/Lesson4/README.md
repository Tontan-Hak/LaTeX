## How to write (Tabular, Graph, trigon, v)
- lesson 4 

```
\documentclass[12pt,a4paper]{article}
\usepackage[left=1cm,right=1cm,top=2cm,bottom=2cm]{geometry}
\usepackage{tikz}
\usepackage{tkz-tab}
\usepackage{amsmath,amsfonts,amssymb}
\usepackage[no-math]{fontspec}
\setmainfont{Khmer OS Siemreap}
\setmathrm{Times New Roman}
\newcommand{\kml}{\fontspec{Khmer OS Muol Light}\selectfont}
\usepackage{enumitem}
\usepackage{cancel}
\usepackage{xcolor}
\usepackage{rotating}
%\usepackage{mathptmx}

\everymath{\displaystyle}
\usepackage{fancyhdr}
\pagestyle{fancy}
\fancyhf{}
\lhead{Tontan Hak}
\chead{ Latex}
\rhead{Assignment}
\lfoot{E2stem education, Cambodia}
\cfoot{High School}
\rfoot{\thepage}
\renewcommand{\headrulewidth}{2pt}
\renewcommand{\footrulewidth}{2pt}
\renewcommand{\headrule}{\color{blue!50}\hrulefill}
\renewcommand{\footrule}{\color{gray}\hrulefill}
\begin{document}
\begin{center}
\underline{\underline{Lesson1}}
\end{center}
\begin{enumerate}
\item  Sum of {\color{blue}sequence} $\begin{aligned}[t]
 \sum_{k=1}^nk&=1+2+3+\cdots+n\\
 &=\frac{n(n+1)}{2}
 \end{aligned}$
\item Sum of sequence \begin{align*}
\sum_{k=1}^n k^2&=1^2+2^2+3^+\cdots+n^2\\
&=\frac{n(n+1)(2n+1)}{6} 
\end{align*}
\item  $\begin{aligned}[t]
\int (x^2+2x+3)dx&=\int x^2 dx+2\int xdx+3\int dx\\
&=\frac{x^3}{3}+\bcancel{ 2}\frac{x^2}{\bcancel{ 2}}+3x+c\\
&=\frac{x^3}{3}+\frac{x^2}{2}+3x+c,c\in \mathbb{R}
\end{aligned}  $ 
\item ប្រអប់ {\kml ប្រអប់}
  \begin{center}
  \begin{tabular}{lc|c|c|c}
%  \hline 
ម៉ោង  & \kml ចន្ទ័ & \kml អង្គារ&\kml ពុធ&\kml ព្រហស្បហ៍ \\ 
  \hline 
  7:30-8:30am &\multicolumn{2}{c|}{គណិត} & &ជីវះ \\ 
  \cline{1-3}\cline{5-5} 
\tikz\node at (1.2,-0.1)[overlay]{  8:30-9:30am}; & រូប & \tikz\node at (0,-0.1)[overlay]{ គណិត};&ខ្មែ&ផែនដី \\ 
%  \hline 
  \cline{2-2}\cline{5-5}
   & ខ្មែ &  &  &ភូមិ\\
  \hline
  10:00-11:00am &\multicolumn{1}{c}{រូប}  &\multicolumn{1}{c}{ ផែនដី} & \multicolumn{1}{c}{ជីវះ}  &\multicolumn{1}{c}{គណិត}\\
  \cline{1-1}
  \end{tabular} 
  \end{center}

\item សញ្ញានៃពហុធា $f(x)=ax^2+bx+c$ 
\begin{center}
  \begin{tikzpicture}
  \tkzTabInit{$x$/1,$f(x)$/1.5}{$-\infty$, $\alpha$,$\beta$,$+\infty$}
  \tkzTabLine{ , \text{សញ្ញាដូច $a$} , z ,\text{សញ្ញាផ្ទុយ$a$} ,z , \text{សញ្ញាដូច $a$} , }
  \end{tikzpicture}
\end{center}
\item សិក្សាសញ្ញានៃ $\frac{x+1}{x-2}$
  \begin{center}
    \begin{tikzpicture}
  \tkzTabInit{$x$/1,$x+1$/1,$x-2$/1,$\frac{x+1}
  {x-2}$/1.5,$f(x)$/2}{$-\infty$,$-1$,$2$,$+\infty$}
  \tkzTabLine{,-,z,+,t,+, }
  \tkzTabLine{,-,t,-,z,+, }
  \tkzTabLine{,+,z,-,d,+, }
  \tkzTabVar{-/$a$ ,+/$b$,-D-/ $c$/$d$,+/$c$  }
  \end{tikzpicture}
  \end{center}
\item សិក្សាសញ្ញានៃ $f'(x)=x^2+2x-3$
  \begin{center}
    \begin{tikzpicture}
  \tkzTabInit{$x$/1,$f'(x)$/1,$f(x)$/2}{$-\infty$,$-3$,$1$,$+\infty$}
  \tkzTabLine{,-,z,h,z,-, }
  \tkzTabVar{+/\color{blue} $a$ ,-/\color{red} $b$,+/\color{blue} $c$,-/$d$  }
  \end{tikzpicture}
  \end{center}
\item ក្រាប $y=e^x$
\begin{center}
\begin{tikzpicture}
\fill [fill=gray!40,draw](0,0)--(4,0)--(4,3)--(0,0);
\draw [shift={(4,3)}](0,0)--(-143.1:0.7) arc (-143.1:-90:0.7)--cycle;
\fill[fill=blue!40](0,0)--(0.:0.7) arc (0.:36.86:0.7)--cycle;
%\draw [dashed](0,0)--(4,0)--(4,3)--(0,0);
\draw (3.5,0)--(3.5,0.5)--(4,0.5);
\node at (0,0)[left]{$A$};
\node at (4,0)[right]{$B$};
\node at (4,3)[above]{$C$};
\node at (2,0)[below]{$4\text{cm}$};
\node at (4,1.5)[right]{$3 \text{cm}$};
\node at (1.8,1.3)[above]{\begin{turn}{40}$5\text{cm}$ \end{turn}};
\draw (0.7,0)--(0,0)--(0.55,0.4);
\end{tikzpicture}
\end{center}
\item ក្រាប
\begin{center}
\begin{tikzpicture}[>=latex]
\fill [fill=gray, opacity=0.3,draw](-2,0)--(-2,0.5)--(1,3)--(1,0)--cycle;
\fill [samples=50,domain=-3:1.5), fill=white,] plot (\x,2.71^\x)--cycle;
\draw [samples=50,domain=-3:1.5)] plot (\x,2.71^\x);
\draw [->](-4,0)--(4,0) node[right]{$x$};
\draw [->](0,-4)--(0,4) node[above]{$y$};
\foreach \x in {-3,-2,-1,1,2,3}
\draw [shift={(\x,0)}](0pt,2pt)--(0pt,-2pt) node [below] {$\x$};
\foreach \y in {-3,-2,-1,1,2,3}
\draw [shift={(0,\y)}](2pt,0pt)--(-2pt,0pt)node [right] {$\y$};
%\draw [samples=50,domain=-2:2)] plot (\x,{(\x)^2 -3});
%\draw [samples=50,domain=-2:2)] plot (\x,\x);
\node at (1.7,3.5){\begin{turn}{70} $y=e^x$ \end{turn}};
\node at (-0.3,-0.3){$0$};
\end{tikzpicture}
\end{center}
\item ផ្ទៃក្រលា
\begin{center}
\begin{tikzpicture}
 \fill [samples=50,domain=(-2.36:0.73),fill=gray,opacity=0.3] plot(\x,{sin((\x)*180/pi)})--cycle;
 \fill [samples=50,domain=(-2.35:0.8),fill=gray,opacity=0.3] plot(\x,{cos((\x)*180/pi)})--cycle;
 \draw [samples=50,domain=(-3:1.5)] plot(\x,{sin((\x)*180/pi)});
 \draw [samples=50,domain=(-3:1.5)] plot(\x,{cos((\x)*180/pi)});
\end{tikzpicture}
\end{center}
\end{enumerate}
\end{document}
```
