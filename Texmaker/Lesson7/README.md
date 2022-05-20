## Beamer
- How to do slide presentation
```
\documentclass{beamer}
%\usepackage[none]{hyphenat}
\usepackage{multicol}

\usetheme[progressbar=frametitle]{metropolis}
\setbeamertemplate{frame numbering}[fraction]
\useoutertheme{metropolis}
\useinnertheme{metropolis}
\usefonttheme{metropolis}
\usecolortheme{spruce}
\setbeamercolor{background canvas}{bg=white}

\definecolor{mygreen}{rgb}{.125,.5,.25}
\usecolortheme[named=mygreen]{structure}
\everymath{\displaystyle}

\title[Short title]{The Function of Logarithms}
%\subtitle{Subtitle Here}
\author{Tontan Hak}
\institute{E2stem education, Cambodia}
\date{\today}
\subject{Math}
\setbeamercovered{transparent=15}

\begin{document}
\metroset{block=fill}
\begin{frame}
\titlepage

\end{frame}

\begin{frame}[t]{Functions, Limits, Derivativ} \vspace{10pt}
\begin{definition}
What is Function? How to apply function in real-life.
\end{definition}
\begin{enumerate}
\item This is my first lesson.
\item Integral $\int xdx$
\item $\int_{0}^{\infty}\cos x \sin x dx$
\end{enumerate}
\end{frame}
\begin{frame}[t]{Content} \vspace{4pt}
\begin{example}
Solve that $x^2 -3x +2 =0$
\end{example}
\end{frame}
\begin{frame}[t]{Functions} \vspace{10 pt}
\begin{block}{Definition of Function}  
\vspace{0.5 em}
A \textbf{function} $f$ is a rule that assigns to each element $x$ in a set $D$ exactly one element, called $f(x)$, in a set $E$.
\vspace{0.5 em}
\end{block}
\vspace{10pt}
Set $D$ is called the 
\only<1>{ \line(1,0){50} }
\only<2>{\textcolor{magenta}{domain}}
 \, of the function.\\[10pt]

Set $E$ is called the 
\only<1>{ \line(1,0){50} }
\only<2>{\textcolor{magenta}{range}}
\, of the function.
\end{frame}
\begin{frame}[t]{Your very first flash card} \vspace{10pt}
$\sqrt{x^2}=$\\[10pt]
\begin{enumerate}[(A)]
\item $x$
\item $-x$
\item $|x|$
\item Undefined
\end{enumerate}
\end{frame}

\begin{frame}[t]{Your very first flash card} \vspace{10pt}
\begin{columns}[onlytextwidth]
\column{0.4 \textwidth}
$\sqrt{x^2}=$\\[10pt]
\begin{enumerate}[(A)]
\item $x$
\item $-x$
\item $|x|$
\item Undefined
\end{enumerate}
\column{0.6 \textwidth}
\only<2>{
\includegraphics[scale=0.45]{xsquared}
}
\only<3>{
$\sqrt{x^2}=
\begin{cases}
-x, & x<0 \\
x, & x> \geq 0
\end{cases}$ \\[10pt]}
\end{columns}
\end{frame}
\begin{frame}{Parent Function} \vspace{4pt}
You should be able to define function and parent of function.
\begin{enumerate}
\begin{multicols}{3}
\item $y=x$
\item $y=|x|$
\item $y=x^2$
\item $y=x^3$
\item $y=x^b$
\onslide<2->{
\item $y=\sqrt{x}$
\item $y=\sqrt[3]{x}$
\item $y=\frac{1}{x}$
\item $y=2^x$
\item $y=e^x$
}
\onslide<3->{
\item $y=\ln x$
\item $y=\frac{1}{1+e^{-x}}$
\item $y=\sin x$
\item $y=\cos x$
\item $y=\tan x$ }
\end{multicols}
\end{enumerate}
\end{frame}
\begin{frame}{Standout}
\flushleft
Homework
\end{frame}

\end{document}
```
