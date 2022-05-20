## How to write maths exercises and font khmer
- Lesson 1
## Example
```
\documentclass[12pt,a4paper]{article}
\usepackage[utf8]{inputenc}
\usepackage{amsmath}
\usepackage{amsfonts}
\usepackage{amssymb}
\usepackage{graphicx}
\usepackage[no-math]{fontspec}
\setmainfont{Khmer OS Siemreap}
\everymath{\displaystyle}
\setmathrm{Times New Roman}
\newcommand{\kml}{\fontspec{Khmer OS Muol Light}\selectfont}
\newcommand{\kbk}{\fontspec{Khmer OS Bokor}\selectfont}
\usepackage[left=2cm,right=2cm,top=2cm,bottom=2cm]{geometry}
\begin{document}
\begin{center}
 \kml កិច្ចការផ្ទះ
 \end{center} 
\begin{enumerate}
\item ដោះស្រាយសមីការនីមួយៗខាងក្រោម៖
  \begin{enumerate}
  \item $x^2 +2x +1=0$
  \item $x^2 - 4 =0$
  \end{enumerate}
\item {\kml គណនា}អាំងតេក្រាលខាងក្រោម៖
  \begin{enumerate}
  \item $\int xdx$
  \item $\int \sin x. \cos x dx$
  \item $\int_{0}^{\infty} \cos x dx$
  \end{enumerate}
\item \kbk តារាងកាលវិភាគប្រចាំថ្ងៃ៖
\begin{center}
\begin{tabular}{|c|c|c|}
\hline 
   \multicolumn{3}{|c|}{ព្រឹក} \\
\hline 
៧ - ៨ & \multicolumn{2}{|c|}{គណិត} \\ 
\hline 
១០  - ១១ & ខ្មែរ  & រូប  \\
\hline 
\end{tabular} 
\end{center}
\end{enumerate}
\end{document}
```
