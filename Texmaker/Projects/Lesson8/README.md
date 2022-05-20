# How to write Thesis
- code 

```
\documentclass[12pt]{article}

\usepackage[margin=1 in]{geometry}
\usepackage{amsfonts, amsmath, amssymb}
\usepackage[none]{hyphenat}
\usepackage{fancyhdr}
\usepackage{graphicx}
\usepackage{float}
\usepackage[nottoc, notlot, notlof]{tocbibind}

\pagestyle{fancy}
\fancyhead{}
\fancyfoot{}
\fancyhead[L]{\slshape \MakeUppercase{Place Title Here}}
\fancyhead[R]{\slshape Student Name}
\fancyfoot[C]{\thepage}
%\renewcommand{\headrulewidth}{0pt}
\renewcommand{\footrulewidth}{0pt}
\parindent 0ex
\setlength{\parindent}{4em}
\setlength{\parskip}{1 em}
\renewcommand{\baselinestretch}{1.5}

\begin{document}
\begin{titlepage}
\begin{center}
\begin{center}
\vspace*{1 cm}
\large {\textbf{E2stem Mathematics}}\\
\large {\textbf{Assignment 4a}}
\vfill 
\line(1,0){400}\\ [1 mm]
\huge{\textbf{This is a sample of the title}}\\ [3mm]
\Large{\textbf{- This is a Subtitle - }}\\[1mm]
\line(1,0){400}\\ [1 mm]
\vfill
By the student Name\\
Candidate \# \\
\today\\
\end{center}
\end{center}
\end{titlepage}
\tableofcontents
\thispagestyle{empty}
\clearpage

\setcounter{page}{1}

\section{Introduction}
When Rebecca Goldin spoke to a recent class of incoming freshmen at George Mason University, she relayed a disheartening statistic: According to a recent study, 36 percent of college students don’t significantly improve in critical thinking during their four-year tenure. “These students had trouble distinguishing fact from opinion, and cause from correlation,” Goldin explained.
\section{Scoring Criteria}
She went on to offer some advice: “Take more math and science than is required. And take it seriously.” Why? Because “I can think of no better tool than quantitative thinking to process the information that is thrown at me.” Take, for example, the study she had cited. A first glance, it might seem to suggest that a third of college graduates are lazy or ignorant, or that higher education is a waste. But if you look closer, Goldin told her bright-eyed audience, you’ll find a different message: “Turns out, this third of students isn’t taking any science.”
Goldin, a professor\footnote{He teaches math} of mathematical sciences at George Mason, has made it her life’s work to improve quantitative literacy. In addition to her research and teaching duties, she volunteers as a coach at math clubs for elementary- and middle-school students. \\
In 2004, she became the research director of George Mason’s Statistical Assessment Service, which aimed “to correct scientific misunderstanding in the media resulting from bad science, politics or a simple lack of information or knowledge.” The project has since morphed into STATS (run by the nonprofit Sense About Science USA and the American Statistical Association), with Goldin as its director. Its mission has evolved too: It is now less of a media watchdog and focuses more on education. Goldin and her team run statistics workshops for journalists and have advised reporters at publications including FiveThirtyEight, ProPublica and The Wall Street Journal.
\subsection{Mathematical Introduction}
When Quanta first reached out to Goldin, she worried that her dual “hats” — those of a mathematician and a public servant — were too “radically different” to reconcile in one interview. In conversation, however, it quickly became apparent that the bridge between these two selves is Goldin’s conviction that mathematical reasoning and study is not only widely useful, but also pleasurable. Her enthusiasm for logic — whether she’s discussing the manipulation of manifolds in high-dimensional spaces or the meaning of statistical significance — is infectious. “I love, love, love what I do,” she said. It’s easy to believe her — and to want some of that delight for oneself.
\subsection{Personal Engagement}
Where does your passion for mathematics and quantitative thought come from?
As a young person I never thought I liked math. I absolutely loved number sequences and other curious things that, in retrospect, were very mathematical. At the dinner table, my dad, who is a physicist, would pull out some weird puzzle or riddle that sometimes only took a minute to solve, and other times I’d be like, “Huh, I have no idea how that one works!” But there was an overall framework of joy around solving it.
\subsection{Reflection}
When did you recognize you could apply that excitement about puzzles to pursuing math professionally?
Actually very late in the game. I was always very strong in math, and I did a lot of math in high school. This gave me the false sense that I knew what math was about: I felt like every next step was a little bit more of the same, just more advanced. It was very clear in my mind that I didn’t want to be a mathematician.
\subsection{Use of Mathematics}
But when I went to college at Harvard, I took a course in topology, which is the study of spaces. It wasn’t like anything I’d seen before. It wasn’t calculus; it wasn’t complex calculations. The questions were really complicated and different and interesting in a way I had never expected. And it was just kind of like I fell in love.

\subsection{Real life Application}
Why Do We Learn Math?
I cringe when hearing "Math teaches you to think".

It's a well-meaning but ineffective appeal that only satisfies existing fans (see: "Reading takes you anywhere!"). What activity, from crossword puzzles to memorizing song lyrics, doesn't help you think?

Math seems different, and here's why: it's a specific, powerful vocabulary for ideas.

Imagine a cook who only knows the terms "yummy" and "yucky". He makes a bad meal. What's wrong? Hrm. There's no way to describe it! Too mild? Salty? Sweet? Sour? Cold? These specific critiques become hazy variations of the "yucky" bucket. He probably wouldn't think "Needs more umami".

Words are handholds that latch onto thoughts. You (yes, you!) think with extreme mathematical sophistication\cite{E2stem}. Your common-sense understanding of quantity includes concepts refined over millennia: base-10 notation, zero, decimals, negatives.

What we call "Math" are just the ideas we haven't yet internalized.
Let's explore our idea of quantity. It's a funny notion, and some languages only have words for one, two and many. They never thought to subdivide "many", and you never thought to refer to your East and West hands.
\section{Conclusion}
One way I might describe it is to say that I study symmetries of mathematical objects. This comes about when you’re interested in things like our universe, where the Earth is rotating, and it’s also rotating around the sun, and the sun is in a larger system that is rotating. All those rotations are symmetries. There are a lot of other ways symmetries come up, and they can get really, really complicated. So we use neat mathematical objects to think about them, called groups. This is useful because if you’re trying to solve equations, and you know you have symmetries, you can essentially find a way mathematically to get rid of those symmetries and make your equations simpler.
\section{Using LaTex}
LaTeX is a high-quality typesetting system; it includes features designed for the production of technical and scientific documentation. LaTeX is the de facto standard for the communication and publication of scientific documents. LaTeX is available as free software.

\pagebreak
\begin{thebibliography}{}

\bibitem{E2stem}
Youk kunthur, High school.
``Cambodia."
\texttt{The e2stem education, Cambodia}
\today
\texttt{<https://e2stem.org.kh/>}
\end{thebibliography}
\end{document}

E2STEM (https://e2stem.org.kh/)
E2STEM | Transforming Cambodia Through E2STEM Education
We train young Cambodians to become STEM (Science, Technology, Engineering, Mathematics) professionals with competencies in 21st century skills.
```