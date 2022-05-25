## How to do slide
- code 

```
\documentclass[serif,12pt]{beamer}
\usetheme{Madrid}
\usefonttheme[onlylarge]{structurebold}
\usepackage{polyglossia}
\newcommand{\kml}{\fontspec{Khmer M1} \selectfont}
\newcommand{\kbk}{\fontspec{Khmer OS Bokor} \selectfont}
\newcommand{\ksr}{\fontspec{Khmer OS Siemreap} \selectfont}
\setmathrm{Times New Roman}
\newfontfamily\khmerfont{Khmer OS}[%
Ligatures=TeX,%
BoldFont={Khmer OS Bokor},%
ItalicFont=*,%
ItalicFeatures={FakeSlant=.23,Color=blue}]
\setmainlanguage[numerals=khmer]{khmer}
\title[BacII]{Preparation Fot BacII exam}
\author[]{\kml ហាក់ តុនតាន}
\institute[\kml E2stem education, Cambodia]{\kml E2stem education, Cambodia}
\date{\kbk \today}
\begin{document}
 \section{ស្វាគមន៏}
 \begin{frame}{ស្វាគមន៏}
  \titlepage
 \end{frame}
 \section{មាតិកា}
 \begin{frame}{\insertsection}
  \tableofcontents
 \end{frame}
 \section{ចំណងជើងផ្នែក១}
 \begin{frame}
  \frametitle{\insertsection}
  សរសេរអត្ថបទនៅទីនេះ។
 \end{frame}
 \section{ចំណងជើងផ្នែក២}
 \begin{frame}{\insertsection}
  សរសេរអត្ថបទនៅទីនេះ។
 \end{frame}
\end{document}
```
