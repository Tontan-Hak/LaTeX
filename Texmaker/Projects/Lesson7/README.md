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

```
\documentclass[11pt]{beamer}
\usepackage{media9}
\usepackage{tikz}
\everymath{\displaystyle}
\usepackage{multicol}
\usefonttheme{serif}
\usefonttheme{professionalfonts}
\usetikzlibrary{arrows.meta,calc,chains,positioning,shadows,shapes.callouts}
\usepackage{amsmath,amsthm,amssymb,amsfonts}
\usepackage{cancel}
\usepackage{mathpazo}
\usetheme{Frankfurt}
\XeTeXlinebreaklocale ''km''
\XeTeXlinebreakskip = 0.5pt plus 1pt minus 1pt
\usepackage[no-math]{fontspec}
\setmainfont{Khmer OS Siemreap}
\setmathrm{Times New Roman}
\newcommand{\kml}{\fontspec{Khmer M1}\selectfont}
\newcommand{\kbk}{\fontspec{Khmer OS Bokor}\selectfont}
\newtheorem{notation}{\kml សំគាល់}
\newtheorem{Def}{\kml និយមន័យ}
\newtheorem{Ex}{\kml ឧទាហរណ៍}
\newtheorem{exercise}{\kml លំហាត់}
\newtheorem{formula}{\kml រូបមន្ត}
\newtheorem{remark}{\kml សំគាល់}
\newtheorem{general}{\kml ជាទូទៅ}
\author{\kbk​ បង្រៀនដោយ៖ \kml ហាក់​ តុនតាន}
\title{\kml 4. លីមីតរាងមិនកំណត់}
%\setbeamercovered{transparent} 
%\setbeamertemplate{navigation symbols}{} 
%\logo{} 
%\institute{} 
%\date{} 
%\subject{} 
\newcommand{\Answer}{{\kml ចម្លើយ៖\;}}
\newcommand{\N}{\mathbb{N}}
\begin{document}
\begin{frame}
\titlepage
\end{frame}
%\begin{frame}
%\tableofcontents
%\end{frame}
\begin{frame}{\kml 5.លីមីតនៃអនុគមន៍ត្រីកោណមាត្រ}
\Large
\begin{theorem}
\begin{enumerate}
\begin{multicols}{2}
\item $\lim_{x\to 0}\dfrac{\sin x}{x}=1$
\item $\lim_{x\to 0}\dfrac{\sin ax}{ax}=1$
\end{multicols}
\end{enumerate}
\vspace{0.1cm}
\end{theorem}
\begin{Ex}
គណនា
$\lim_{x\to 0}\dfrac{\sin 3x}{x}$
 រាងមិនកំណត់ $\frac{0}{0}$\\ 
គេបាន $\begin{aligned}[t]
\lim_{x\to 0}\dfrac{\sin 3x}{x}&=\lim_{x\to 0}\dfrac{\sin 3x}{{\color{blue}3}x}\times {\color{blue}3}\\
&=1\times 3\\
&=3
\end{aligned}$
\end{Ex}
\end{frame}
\begin{frame}
\Large
\begin{Ex}
គណនា $\lim_{x\to \frac{\pi}{4}}\dfrac{\cos x-\sin x}{\cos 2x}$ រាងមិនកំណត់ $\dfrac{0}{0}$\\
គេបាន $\begin{aligned}[t]
&\lim_{x\to \frac{\pi}{4}}\dfrac{\cos x-\sin x}{\cos^2 x-\sin^2 x}\\
&=\lim_{x\to \frac{\pi}{4}}\dfrac{\cos x-\sin x}{(\cos x-\sin x)(\cos x+\sin x)}\\
&=\lim_{x\to \frac{\pi}{4}}\dfrac{1}{\cos x+\sin x}\\
&=\dfrac{1}{\cos \frac{\pi}{4}+\sin \frac{\pi}{4}}
=\dfrac{1}{\frac{\sqrt{2}}{2}+\frac{\sqrt{2}}{2}}
=\frac{1}{\sqrt{2}}
=\frac{\sqrt{2}}{2}
\end{aligned}$
\end{Ex}
\end{frame}
\begin{frame}
\Large
\begin{Ex}
គណនា $\lim_{x\to 0}\dfrac{1-\cos 2x}{x}$ រាងមិនកំណត់ $\dfrac{0}{0}$\\
គេបាន $\begin{aligned}[t]
\lim_{x\to 0}\dfrac{1-\cos 2x}{x}&=\lim_{x\to 0}\dfrac{2\sin^2 \frac{2x}{2}}{x}\\
&=\lim_{x\to 0}\left(\dfrac{\sin^2 x}{x^2}\times 2x\right)\\
&=1\times 0\\
&=0
\end{aligned}$
\end{Ex}
\end{frame}
\begin{frame}
\Large
\begin{Ex}
គណនា $\lim_{x\to 0} \dfrac{\sqrt{1+x}-\sqrt{1-x}}{\sin 3x}$ រាងមិនកំណត់ $\frac{0}{0}$\\
 គេបាន $\begin{aligned}[t]
&\lim_{x\to 0}\dfrac{(\sqrt{1+x}-\sqrt{1-x})(\sqrt{1+x}-\sqrt{1-x})}{\sin 3x .(\sqrt{1+x}+\sqrt{1-x})}\\
&=\lim_{x\to 0}\dfrac{1+x-1+x}{\sin 3x .(\sqrt{1+x}+\sqrt{1-x})}\\
&=\lim_{x\to 0}\dfrac{2x}{\sin 3x .(\sqrt{1+x}+\sqrt{1-x})}\\
&=\lim_{x\to 0}\left(\frac{3x}{\sin 3x}\times \frac{2}{3(\sqrt{1+x}+\sqrt{1-x})} \right)= \frac{1}{3}
\end{aligned}$
\end{Ex}
\end{frame}
\begin{frame}
\Large
\begin{Ex}
គណនា $\lim_{x\to 0}\dfrac{\sin 4x}{\sin 3x}$ រាងមិនកំណត់ $\frac{0}{0}$\\

គេបាន $\begin{aligned}[t]
&\lim_{x\to 0}\left(\dfrac{\sin 4x}{4x}\times \dfrac{3x}{\sin 3x} \right)\times \frac{4}{3}\\
&=\frac{4}{3}
\end{aligned}$
\end{Ex}
\end{frame}
\begin{frame}{\kml 6. លីមីតនៃអនុគមន៍អ៊ិចស្ប៉ូណង់ស្យែល}
\Large
\begin{formula}
 បើ $n>0$ នោះគេបាន
\begin{itemize}
\begin{multicols}{2}
\item $\lim_{x\to +\infty}e^x=+\infty$

\item $\lim_{x\to -\infty}e^x=0$

\item $\lim_{x\to 0}\dfrac{e^x-1}{x}=1$

\item $\lim_{x\to +\infty}\dfrac{e^x}{x^n}=+\infty$

\item $\lim_{x\to +\infty}\dfrac{x^n}{e^x}=0$

\item $\lim_{x\to +\infty}x^ne^x=+\infty$
\end{multicols}
\end{itemize}
\end{formula}
\end{frame}
\begin{frame}
\Large
\begin{Ex}
គណនា $\lim_{x\to +\infty}(2^x+x^2-1)
$ 
\end{Ex}
\pause
\Answer
គេបាន $\begin{aligned}[t]
&\lim_{x\to +\infty}(2^x+x^2-1)\\\pause
&=\lim_{x\to +\infty}2^x+\lim_{x\to +\infty}x^2-\lim_{x\to +\infty} 1\\\pause
&=+\infty+\infty-1\\\pause
&=+\infty
\end{aligned}$
\end{frame}
\begin{frame}
\Large
\begin{Ex}
គណនា $\lim_{x\to -\infty}(e^x+x+2)$ 
\end{Ex}
\pause
\Answer គេបាន\\
$\begin{aligned}[t]
\lim_{x\to -\infty}(e^x+x+2)&\pause=\lim_{x\to -\infty}e^x+\lim_{x\to -\infty}x+\lim_{x\to -\infty}2\\\pause
&=0-\infty+2\\\pause
&=-\infty\pause
\end{aligned}$
\end{frame}
\begin{frame}
\Large
\begin{Ex}
គណនា $\lim_{x\to +\infty}(x^3+x)e^{-x}$
\end{Ex}
\pause
\Answer គេបាន\\
 $\begin{aligned}[t]
 \lim_{x\to +\infty}(x^3+x)e^{-x}\pause
 &=\lim_{x\to +\infty}\dfrac{x^3+x}{e^x}\\\pause
 &=\lim_{x\to +\infty}\dfrac{x^3}{e^x}+\lim_{x\to +\infty}\dfrac{x}{e^x}\\\pause
 &=0+0=0\pause
 \end{aligned}$
\end{frame}
\begin{frame}
\Large
\begin{formula}
\begin{itemize}
\item $\lim_{x\to +\infty}\left( 1+\frac{1}{x}\right)^x=e$
\pause
\item $\lim_{x\to 0}(1+x)^{\frac{1}{x}}=e$
\pause
\item $\lim_{x\to +\infty}\left(1+\frac{1}{u(x)} \right)^{u(x)}=e$
\pause
\item $\lim_{x\to 0}[1+u(x)]^{\frac{1}{u(x)}}=e$
\end{itemize}
\pause
បើ $x\to +\infty \Rightarrow u(x)\to +\infty\;,\;x\to 0 \Rightarrow u(x)\to 0$ 
\end{formula}
\end{frame}
\begin{frame}
\Large
\begin{formula}
\begin{itemize}
\item $\lim_{x\to 0}\dfrac{e^x-1}{x}=1$
\pause
\item $ \lim_{x\to 0}\dfrac{e^{ax}-1}{ax}=1 $ ដែល $a$ ជាចំនួនពិត
\pause
\item $\lim_{x\to 0}\dfrac{e^{u(x)}-1}{u(x)}=1$ បើ $x\to 0 \Rightarrow u(x)\to 0$
\pause
\item $\lim_{x\to 0 }\dfrac{a^x-1}{x}=\ln a$ ដែល $a$ ជាចំនួនពិតវិជ្ជមាន ។ 
\end{itemize}
\end{formula}
\pause
\begin{remark}
$\lim_{x\to a}\ln [f(x)]=\ln [\lim_{x\to a}f(x)]$
\end{remark}
\end{frame}

\begin{frame}
\begin{Ex}
គណនា $\lim_{x\to +\infty}\left( 1+\frac{2}{x}\right)^x$ 
\end{Ex}
\pause
\Answer
 $\lim_{x\to +\infty}\left( 1+\frac{2}{x}\right)^x$ \pause
  រាងមិនកំណត់ $1^{\infty}$\\\pause
$ \begin{aligned}[t]
\lim_{x\to +\infty}\left( 1+\frac{2}{x}\right)^x\pause
&=\lim_{x\to +\infty}\left( 1+\dfrac{1}{\frac{x}{2}}\right)^{\frac{x}{2}\times 2}\\\pause
&=\lim_{x\to +\infty}\left[\left(1+\dfrac{1}{\frac{x}{2}} \right)^{\frac{x}{2}} \right]^2\\\pause
&=e^2
\end{aligned} $
\end{frame}
\begin{frame}
\large

\begin{Ex}
គណនា
$\lim_{x\to +\infty}\left(\dfrac{x+3}{x-1} \right)^{x+2}$\pause រាងមិនកំណត់ $1^{+\infty}$\\\pause
គេបាន $\begin{aligned}[t]
&\lim_{x\to +\infty}\left(\dfrac{x+3}{x-1} \right)^{x+2}\pause=\lim_{x\to +\infty}\left(\frac{ x-1+4}{x-1} \right)^{x+2}\\\pause
&=\lim_{x\to +\infty}\left(1+\frac{4}{x-1} \right)^{x+2}\\\pause
&=\lim_{x\to +\infty}\left[\left(1+\frac{1}{\frac{x-1}{4}}\right)^{\frac{x-1}{4}}\right]^{ \frac{4(x+2)}{x-1} }=e^4
\end{aligned}$\\\pause
ព្រោះ $\lim_{x\to +\infty}\frac{4(x+2)}{x-1}=4$

\end{Ex}
\end{frame}
\begin{frame}
\Large
\begin{Ex}
គណនា $\lim_{x\to 0}(1+3\tan ^2 x)^{\cot^2 x}$
\end{Ex}
\Answer
 $\lim_{x\to 0}(1+3\tan ^2 x)^{\cot^2 x}$\pause រាងមិនកំនត់ $1^{\infty}$\\\pause
គេបាន $\begin{aligned}[t]
&\lim_{x\to 0}(1+3\tan^2 x )^{\cot^2 x}\\\pause
&=\lim_{x\to 0}(1+3\tan^2 x )^{\frac{1}{3\tan^2 x}\times 3}\\\pause
&\lim_{x\to 0}\left[(1+3\tan^2 x)^{\frac{1}{3\tan^2 x}}\right]^{3}=e^2
\end{aligned}$
\end{frame}
\begin{frame}
\Large

\begin{Ex}
គណនា $\lim_{x\to +\infty}\left( \dfrac{x^2-5x+8}{x^2-6x+3}\right)^x$\pause រាងមិនកំណត់ $1^{\infty}$
\end{Ex}
\pause
\Answer
$\begin{aligned}[t]
&\lim_{x\to +\infty}\left(1+\frac{x+5}{x^2-6x+3} \right)^x\\\pause
&=\lim_{x\to +\infty}\left[\left(1+\dfrac{1}{\frac{x^2-6x+3}{x+5}} \right)^{\frac{x^2-6x+3}{x+5}}\right]^{\frac{x(x+5)}{x^2-6x+3}}\\\pause
&=e \quad \text{ព្រោះ }\lim_{x\to +\infty}\dfrac{x(x+5)}{x^2-6x+3}=1
\end{aligned}$
\end{frame}
\begin{frame}
\Large
\begin{Ex}
គណនា $\lim_{x\to 0}\dfrac{\ln (1+ax)}{x}$\pause រាងមិនកំណត់ $1^{\infty}$
\end{Ex}
\pause
\Answer 
$ \begin{aligned}[t]
\lim_{x\to 0}\frac{1}{x}\ln (1+ax)\pause&=\lim_{x\to 0}\ln (1+ax)^{\frac{1}{x}}\\\pause
&=\ln \left[\lim_{x\to 0}(1+ax)^{\frac{1}{ax}\times a}   \right]\\\pause
&=\ln e^a\\\pause
&=a\ln e \\\pause
&=a
\end{aligned} $
\end{frame}
\begin{frame}{7. លីមីតនៃអនុគមន៍លោកការីតនេពែ}
\Large
\begin{formula}
ចំពោះ $a,n>0$ គេបាន 
\begin{itemize}
\begin{multicols}{2}
\item $\lim_{x\to 0^+}\ln x=-\infty$
\item $\lim_{x\to +\infty}\ln x=+\infty$
\item $\lim_{x\to 0^+} \ln (ax)=-\infty$
\item $\lim_{x\to +\infty} \ln (ax)=+\infty$
\item $\lim_{x\to +\infty}\dfrac{x}{\ln x}=+\infty$
\item $\lim_{x\to +\infty}\dfrac{x^n}{\ln x}=+\infty$
\item $\lim_{x\to 0^+}x\ln x=0$
\item $\lim_{x\to 0^+}x^n \ln x=0$
\end{multicols}
\end{itemize}
\end{formula}
\end{frame}
\begin{frame}
\Large
\begin{Ex}
គណនា
\begin{enumerate}
\item  $\begin{aligned}[t]
 \lim_{x\to +\infty}(x^3+3+\ln x)\pause=+\infty+3+\infty=+\infty
  \end{aligned}$
  \pause
 \item $\begin{aligned}[t]
 \lim_{x\to 0^+}[\ln x (\ln x-3)]\pause=+\infty (+\infty)=+\infty
 \end{aligned}$
 \pause
\item $\begin{aligned}[t]
\lim_{x\to +\infty}(x\ln x-x^2+5)  &\pause=(+\infty)(-\infty)-(+\infty)+5\\\pause
&=-\infty
\end{aligned} $
\pause
\item $\lim_{x\to +\infty} \dfrac{\ln x}{x^2-x}\pause=\lim_{x\to +\infty} \dfrac{\ln x}{x^2(1-\frac{1}{x})}=0\times 1=0$
 \end{enumerate}
 \end{Ex}
\end{frame}
\end{document}
```
