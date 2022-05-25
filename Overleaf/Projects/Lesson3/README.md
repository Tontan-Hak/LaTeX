## How to write document 
- code 

```
\documentclass[12pt,a4paper]{article}
\usepackage[utf8]{inputenc}
\usepackage{amsmath}
\usepackage{nicematrix}
\usepackage{amsfonts}
\usepackage{mathptmx}
\usepackage{rotating}
\usepackage{tkz-tab}
\usepackage{amssymb}
\XeTeXlinebreaklocale ''km''
\XeTeXlinebreakskip = 0pt plus 0.5pt minus 0.25pt
\usepackage[no-math]{fontspec}
\setmainfont{Khmer OS Siemreap}
\setmathrm{Times New Roman}
\newcommand{\kml}{\fontspec{Khmer OS Muol Light}\selectfont}
\newcommand{\kbk}{\fontspec{Khmer OS Bokor}\selectfont}
\usepackage[left=1cm,right=1cm,top=2cm,bottom=2cm]{geometry}
\everymath{\displaystyle}
\usepackage{enumitem}
\SetEnumitemKey{I}{label= \Roman*.}
\SetEnumitemKey{1}{label= \arabic*.}
\SetEnumitemKey{a}{label= \kalph*.}
\SetEnumitemKey{A}{label= \Alph*:}
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
\begin{enumerate}[I]
\item គណនាលីមីត៖ 
  \begin{enumerate}[a]
  \item $\lim_{x\to 3} \sqrt{3x^2-11}$
  \item $\lim_{x\to \frac{\pi}{3}} \dfrac{\sqrt{3}\sin \left( x-\frac{\pi}{3}\right)}{\left( \frac{\pi}{3}\right) }$
  \item $\lim_{x\to +\infty} (2x-7-11\ln x) $
  \end{enumerate}
\item ក្នុងថង់មួយមានឃ្លីពណ៌ក្រហមចំនួន២ ឃ្លីពណ៌ខៀវចំនួន៣  និងឃ្លីពណ៌ចំនួន ៤ ។ គេចាប់យកឃ្លីចំនួន៣ពីក្នុងថង់ដោយចៃដន្យ។ គណនាប្រូបាបនៃព្រឹត្តការណ៍ខាងក្រោម៖
  \begin{enumerate}[A]
  \item ឃ្លីទាំង៣មានពណ៌ស
  \item ឃ្លីទាំង៣មានពណ៌ខុសគ្នា។
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
\end{enumerate}
\end{document}
```