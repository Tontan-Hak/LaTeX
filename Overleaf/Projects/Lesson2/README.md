## How to do Beamer
- code 

```
\documentclass[11pt]{beamer}
\usetheme{Berlin}
\usepackage[utf8]{inputenc}
\usepackage[english]{babel}
\usepackage{amsmath}
\usepackage{amsfonts}
\usepackage{amssymb}
\usepackage{graphicx}
\usepackage{fontspec}
\usefonttheme{Serif}
\setmainfont{Khmer OS}
\newcommand{\kml}{\fontspec{Khmer M1} \selectfont}
\newcommand{\kbk}{\fontspec{Khmer OS Bokor} \selectfont}
\newcommand{\ksr}{\fontspec{Khmer OS Siemreap} \selectfont}
\setmathrm{Times New Roman}
\everymath{\displaystyle}
%\usepackage[no-math]{fontspec}
\author{\kbk ហាក់​ តុនតាន}
\title{\kml ធ្វើបទបង្ហាញ}
%\setbeamercovered{transparent} 
%\setbeamertemplate{navigation symbols}{} 
%\logo{} 
\institute{E2stem education, Cambodia} 
\date{\today} 
\subject{Math} 
\newcommand{\Answer}{\kml ដំណោះស្រាយ}
\begin{document}

\begin{frame}
\titlepage
\end{frame}

%\begin{frame}
%\tableofcontents
%\end{frame}

\begin{frame}[t]{\kml មាតិការ}
\begin{enumerate}
\item<1-> This is my first item 
\item<2-> I love coding
\item<3-> Limits $\lim_{x\to \infty}{(x^2-e^x)}$
\item<4-> \ksr លំហាត់
\end{enumerate}
\end{frame}
\begin{frame}{\kml ផ្ទៀងស្លាយទី២}
\begin{example}
ដោះស្រាយសមីការ​ $x^2 -3x +2 =0$
\end{example}
\Answer 
$x=1, x=2$
\end{frame}
\begin{frame}{ផ្ទៀងស្លាយទី៣}
\begin{definition}
និយមន័យ
\end{definition}
\end{frame}
\end{document}
```