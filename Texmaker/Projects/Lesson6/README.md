## ដាក់ក្បាលវិញ្ញាសា

```
\documentclass[12pt,a4paper]{article}
\usepackage[utf8]{inputenc}
\usepackage{amsmath}
\usepackage{nicematrix}
\usepackage{amsfonts}
\usepackage{mathptmx}
\usepackage{rotating}
\usepackage{tkz-tab}
\usepackage{multicol}
\usepackage{amssymb}
\XeTeXlinebreaklocale ''km''
\XeTeXlinebreakskip = 0pt plus 0.5pt minus 0.25pt
\usepackage[no-math]{fontspec}
\setmainfont{Khmer OS Siemreap}
\setmathrm{Times New Roman}
\newcommand{\kml}{\fontspec{Khmer OS Muol Light}\selectfont}
\newcommand{\kbk}{\fontspec{Khmer OS Bokor}\selectfont}
\usepackage[left=1cm,right=1cm,top=1.5cm,bottom=1.5cm]{geometry}
\everymath{\displaystyle}
\usepackage{enumitem}
\SetEnumitemKey{I}{label= \Roman*.}
\SetEnumitemKey{1}{label= \arabic*.}
%\SetEnumitemKey{1}{label= \knum*.}
\SetEnumitemKey{a}{label= \kalph*.}
\SetEnumitemKey{A}{label= \Alph*:}
\SetEnumitemKey{c}{label= \alph*.}
% This macro is to produce khmer numbering by
%%%%%--------------------------------

\makeatletter
\def\@khmernum#1{\expandafter\@@khmernum\number#1\@nil} 
\def\@@khmernum#1{%
\ifx#1\@nil 
\else 
\char\numexpr#1+"17E0\relax 
\expandafter\@@khmernum\fi
} 
\def\knum#1{\expandafter\@khmernum\csname c@#1\endcsname}
\def\khmernumeral#1{\@@khmernum#1\@nil}
\AddEnumerateCounter{\knum}{\@knum}{}
\makeatother
\makeatletter
\newcommand*{\kalph}[1]{%
\expandafter\@kalph\csname c@#1\endcsname%
}
\newcommand*{\@kalph}[1]{%
\ifcase#1\or ក\or ខ\or គ\or ឃ\or ង\or ច\or ឆ\or ជ\or ឈ\or ញ\or  ដ\or ឋ\or ឌ%
\or ឍ\or ណ\or ត\or ថ\or ទ\or ធ\or ន\or ប\or ផ\or ព\or ភ\or ម\or យ\or រ\or ល%
\or វ\or ស\or ហ\or ឡ\or អ%
\else\@ctrerr\fi%
}
\AddEnumerateCounter{\kalph}{\@kalph}{}
\makeatother

\begin{document}
\begin{tikzpicture}[overlay]
\node at (0,1)[anchor=north west]{\kml ក្រសួងអប់រំ យុវជន និងកីឡា};
\node at (15,1){លេខបន្ទប់\tikz \draw [overlay,dashed](0,0)--(2.5,0); };
\node at (0,0)[anchor=north west]{ប្រឡង៖ \kml សញ្ញាបត្រមធ្យមសិក្សាទុតិយភូមិ};
\node at (15,0){លេខតុ៖ \tikz \draw [overlay,dashed](0,0)--(2.5,0); };
\node at (0,-1)[anchor=north west] {សម័យប្រឡង៖............................................... មណ្ឌុលប្រឡង៖.........................................};
\end{tikzpicture}
\vspace{2cm}
\begin{enumerate}[I]
\item គណនាលីមីត៖ 
  \begin{enumerate}[a]
  \begin{multicols}{3}
  \item $\lim_{x\to 3} \sqrt{3x^2-11}$
  \item $\lim_{x\to \frac{\pi}{3}} \dfrac{\sqrt{3}\sin \left( x-\frac{\pi}{3}\right)}{\left( \frac{\pi}{3}-x\right) }$
  \item $\lim_{x\to +\infty} (2x-7-11\ln x) $
  \end{multicols}
  \end{enumerate}
\item ក្នុងថង់មួយមានឃ្លីពណ៌ក្រហមចំនួន២ ឃ្លីពណ៌ខៀវចំនួន៣  និងឃ្លីពណ៌ចំនួន ៤ ។ គេចាប់យកឃ្លីចំនួន៣ពីក្នុងថង់ដោយចៃដន្យ។ គណនាប្រូបាបនៃព្រឹត្តការណ៍ខាងក្រោម៖
  \begin{enumerate}[A]
  \begin{multicols}{2}
  \item ឃ្លីទាំង៣មានពណ៌ស
  \item ឃ្លីទាំង៣មានពណ៌ខុសគ្នា។
  \end{multicols}
  \end{enumerate}
\item \begin{enumerate}[a]
    \item គេមានចំនួនកុំផ្លិច $z_1=\sqrt{2}+i\sqrt{2}$ ។ រក $\bar{z_1} (\bar{z_1} \text{ ជាចំនួនកុំផ្លិចឆ្លាស់នៃចំនួនកុំផ្លិច $z_1$} )$ ។
    \item រកម៉ូឌុល និង អាគុយម៉ង់នៃចំនួនកុំផ្លិច $z_1$ ។ សរសេរ $z_1$ ជាទម្រង់ត្រីកោណមាត្រ។
    \item បង្ហាញថា : $\bar{z_1}$ ជាឬសរបស់សមីការ $z^2=2(z\sqrt{2}-2)$ ។
    \end{enumerate}
\item គណនាអាំងតេក្រាល: $I=\int_0^1(3x^2-2x+1)dx \quad ;\quad J=\int_0 ^1 \left( \frac{e^x}{e^x+1}\right)dx\quad ; \quad K=\int_{\frac{\pi}{4}}^{\frac{\pi}{2}}(\sin ^3 x\cos x)dx $ ។
\item \begin{enumerate}[1]
    \item ក្នុងលំហប្រដាប់ដោយតម្រុយអរតូណរម៉ាល់ $(o,\vec{i},\vec{j},\vec{k})$ គេមានចំនុច $A(0,-2,0),B(-4,1,2),C(0,3,7)$ និង $D(4,0,5)$ ។ រកវ៉ិចទ័រ $\overrightarrow{AB},\overrightarrow{BC},\overrightarrow{CD}$ និង $\overrightarrow{AD}$ រួចបង្ហាញចតុកោណ $ABCD$ ជាចតុកោណកែង តែមិនមែនជាការ៉េ។
    \item គេមានសមីការ $9y^2=25(3-x)(3+x)$ ។ បង្ហាញថាសមីការនេះជាសមីការអេលីប។ រកប្រវែងអក្ស័ធំ អ័ក្សតូច កូអរដោនេកំពូលទាំងពីរ និងកូអរដោនេកំណុំទាំងពីររបស់អេលីបនេះ។ សង់អេលីបនេះ។ សង់អេលីបនេះ។
    \end{enumerate}
\item គេមានសមីការឌីផេរ៉ង់ស្យែល $(E):\quad y''=-4y$ ។
  \begin{enumerate}[c]
  \item បង្ហាញថា: $y=\lambda \cos 2x +\mu \sin 2x $  ដែល $\lambda, \mu$ ជាចំនួនពិត ជាចម្លើយរបស់សមីការឌីផេរ៉ង់ស្យែល $(E)$។
  \item រកចម្លើយពិសេសរបស់សមីការឌីផេរ៉ង់ស្យែល $(E)$ ដែល $y''(0)=1$ និង $y'(0)=0$ ។
  \end{enumerate}
\item គេមានអនុគមន៍ $f$ ដែល $f(x)=x-2+\frac{2(x+1)}{e^x}$ ។ យើងតាង $(C)$ ក្រាបរបស់អនុគមន៍ $f$ នៅក្នុងប្លង់ប្រដាប់ដោយតម្រុយអរតូណរម៉ាល់ $(o,\vec{i},\vec{j})$ ។ 
  \begin{enumerate}[1]
  \item រកដែនកំណត់នៃអនុគមន៍ $f$ ។ គណនា $\lim_{x\to +\infty} f(x)$ (យើងដឹងថា $\lim_{x\to +\infty}\frac{x}{e^x}=0$) ។
  \item បង្ហាញថាបន្ទាត់ $(D)$ ដែលមានសមីការ $y=x-2$ ជាអាស៊ីមតូតទ្រេតនៃ $(C)$ ត្រង់ $+\infty$ ។ បញ្ជាក់ទីតាំងនៃក្រាប $(C)$ ធៀបនិងបន្ទាត់ $(D)$ ។
  \item យើងតាង $f'(x)$ ដេរីវេនៃ $f(x)$ ។ បង្ហាញថា $:f'(x)=\frac{e^x-2x}{e^x}$ ។ គេដឹងថាគ្រប់ $x$ ជាធាតុរបស់ $\mathbb{R}; e^x-2x>0$ ។ ប្រើលទ្ធផលនេះដើម្បីទាញយកការសិក្សាអថេរភាពនៃអនុគមន៍ $f$ ។
  \item បង្ហាញថាបន្ទាត់ប៉ះ $(\Delta)$ ទៅនឹង $(C)$ ត្រង់ចំណុចដែលមានអាប់ស៊ីស$0$ ស្របទៅនឹងបន្ទាត់ $(D)$ ។ សង់បន្ទាត់ $(D),(\Delta)$ និងក្រាប $(C)$ ។
  \end{enumerate}
\end{enumerate}
\end{document}
```
